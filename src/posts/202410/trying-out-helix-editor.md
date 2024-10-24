# Trying out Helix Editor

Hey everyone! Time for the (basically monthly) blog!

I've been using Visual Studio Code as my editor of choice since my senior year of undergrad. It's my favorite editor by far, and I've not really thought about changing it since; however, I recently decided to take some time to learn a different way of coding, a way that a lot of people really stand by. The modal way.

I spent some time looking around at modal editors. I considered NeoVim, but I kinda wanted something new, hip and fresh. I came across the [Helix Editor](https://helix-editor.com). Not only is it modal, but it describes itself as a "Post-Modern **Text Editor**" (And it's written in Rust!).

On Tuesday, I opened up the Helix Editor and tried to figure out how it works. I've never used modal text editors, and my only experience with one is learning how to `:q` on Vim. I don't even know if I'd like the modal style of things, since all the editors I've used just are always `Insert` mode with CTRL+\<KEY\> hotkeys.

I noticed that Helix encourages _not_ using the arrow keys, rather, you should use the `H`, `J`, `K`, and `L` keys to move left, down, up, and right. The arrow keys are supported, but they say if you want a more 'modal' experience, you should disable the arrow keys in insert mode and learn to move outside of insert mode. I'm not sure if I'm quite ready to give up my arrow keys, especially because the mouse is not an option.

The tutorial in Helix can be accessed by using the `:tutor` command when you're in the normal mode, helpfully depicted as `NOR`. The tutorial is pretty long, but it does a good job of telling you helpful hotkeys in order to move around.

One silly thing I like about Helix is the built-in themes. I can just type `:theme <THEME>` and turn one of these on. Since I'm coming from Visual Studio Code, the `dark_plus` theme is just like VSCode, so it feels like home.

So far, I used it yesterday and today, and here are my thoughts. I'm still learning hotkeys for everything, but here are my biggest gripes so far (nothing I can't work around eventually, just getting used to the workflow).

- There's a bug with the C# language server, where if I want to `goto definition` of a type that's not in my project (through a nuget package, for example), it fails to process the URI. This appears to be a problem of Helix using a URL resolver crate, not a URI resolver crate: <https://github.com/helix-editor/helix/issues/11334>

- When I'm in insert mode, I still want better movement abilities, and I find myself instinctively using `CTRL` + `Left arrow` to move back a word in insert mode. I'll have to replace that muscle memory with `ESC` + `b`. The only problem with that is that other text editors (non-modal) use those `CTRL` + `Arrow keys` quite a bit, and I don't want to lose that muscle memory either. It might not matter that much, we will see.

- When you use `p` to paste something from the integrated clipboard, it pastes after the cursor, not before. This is different from most of the commands in the editor, and it doesn't make sense why this is different. This is something we can work around thankfully, we just need to use `P`, but I really feel like those should be switched.

- Not only that, copying and pasting from the system clipboard (`Space + y` and `Space + {p|P}`) is broken on my KDE system. I'm not sure why, and I don't have a bug report here to link. Might look into it later, but running `hx --health` didn't provide any useful information, it claims the clipboard provider is present.

- Soft wrapping is not enabled by default, making long lines annoying to deal with when writing Markdown, for example. Luckily, you can enable this in your config by adding these lines:

```toml
[editor.soft-wrap]
enable = true
```

For some reason, however, I don't like editing the config too much, even though they make it way easier than any other editor I've used (simply just `config-open`, make your edits, then `config-reload`). Maybe it's some of that philosophy of good defaults that I can clearly see coming from the Helix editor. My config is only the theme, and the soft wrap functionality.

Overall, I do enjoy the helix editor, and over time I will probably get good at it. For now, I'm just okay at it, and that's okay. I'm already pretty fast considering how I only learned it yesterday.

I will provide an update if I continue to use it and end up daily driving it!
