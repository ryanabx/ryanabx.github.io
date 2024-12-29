# Ryan's Software Wishlist

This is a list of all sorts of various issues and PRs in software that intrigue me! Will be updated with more as time goes on.

## Support for my hardware

- [Lenovo Legion Linux driver](https://lore.kernel.org/lkml/20241217230645.15027-1-derekjohn.clark@gmail.com/)
- [iPhones](https://www.phoronix.com/news/Apple-DWI-Backlight-Linux-v4)

### NVK - Nouveau Vulkan Drivers

- [General NVK issues](https://gitlab.freedesktop.org/mesa/mesa/-/issues/?label_name%5B%5D=NVK)  
- [General NVK MRs](https://gitlab.freedesktop.org/mesa/mesa/-/merge_requests?label_name%5B%5D=NVK)  
- [gfxstrand's (big NVK contributor) activity](https://gitlab.freedesktop.org/gfxstrand)

- [full vkd3d-proton support](https://gitlab.freedesktop.org/mesa/mesa/-/issues/9479)
- ~~[full zink support](https://gitlab.freedesktop.org/mesa/mesa/-/issues/9477)~~
- ~~[full dxvk support](https://gitlab.freedesktop.org/mesa/mesa/-/issues/9478)~~

### Nvidia open kernel module

- [Nvidia open drivers github](https://github.com/NVIDIA/open-gpu-kernel-modules)

### Nova Nvidia GPU kernel module (rust!!!)

- [Nova GPU driver Website](https://rust-for-linux.com/nova-gpu-driver)

## Image-based Operating Systems

### Flatpaks for my apps

- [Steam](https://github.com/ValveSoftware/steam-for-linux/issues/4473)
  - [new issue](https://github.com/ValveSoftware/steam-for-linux/issues/4512)
- VSCode (issues keep being closed)
- [VirtualBox](https://discourse.flathub.org/t/package-virtualbox/4347)

### Other image-based stuff

- [bootc](https://github.com/containers/bootc>)
- [composefs](https://github.com/containers/composefs)
- [systemd-sysupdate](https://github.com/systemd/systemd/labels/sysupdate)
  - [Pull requests](https://github.com/systemd/systemd/pulls?q=is%3Aopen+is%3Apr+label%3Asysupdate)

## Wayland Adoption

### Chromium/Electron Wayland by default
- [Chromium-Wayland issue tracking](https://issues.chromium.org/issues?q=componentid:1456988%20status:(open%20%7C%20new%20%7C%20assigned%20%7C%20accepted))
  - [Chromium-Wayland big issue](https://issues.chromium.org/issues/40083534)
- [Electron PR](https://github.com/electron/electron/pull/35630)

### winewayland.drv - Wine wayland drivers
- [winewayland.drv MRs](https://gitlab.winehq.org/wine/wine/-/merge_requests?scope=all&search=winewayland&sort=updated_desc&state=opened)

## Wayland Protocols

These are protocols I'm excited about for wayland

- ~~[linux-drm-syncobj-v1](https://gitlab.freedesktop.org/wayland/wayland-protocols/-/merge_requests/90)~~
- ~~[xdg-toplevel-icon-v1](https://gitlab.freedesktop.org/wayland/wayland-protocols/-/merge_requests/269)~~
- ~~[ext-screencopy-v1](https://gitlab.freedesktop.org/wayland/wayland-protocols/-/merge_requests/124)~~
- ~~[ext-workspace](https://gitlab.freedesktop.org/wayland/wayland-protocols/-/merge_requests/40)~~
- [foreign-toplevel-state](https://gitlab.freedesktop.org/wayland/wayland-protocols/-/merge_requests/196)

### Notable MRs that I'm not too interested in

These are protocols I'd rather not see in wayland

- [ext-zones](https://gitlab.freedesktop.org/wayland/wayland-protocols/-/merge_requests/264)
