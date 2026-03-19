<div align = center>

# My [Everforest](https://everforest.vercel.app/) rice of [dwl](https://codeberg.org/dwl/dwl)

<br>
</div>
<img width="640" height="360" alt="rice" src="https://github.com/user-attachments/assets/859e9091-1918-4a57-a2d6-dce13a57cb1e" />

### Patches applied
1. [bar](https://codeberg.org/dwl/dwl-patches/patch/bar/bar-0.7.patch)
2. [autostart](https://codeberg.org/dwl/dwl-patches/patch/autostart/autostart-0.7.patch)
3. [sticky](https://codeberg.org/dwl/dwl-patches/patch/sticky/sticky.patch)
4. [swapandfocusdir](https://codeberg.org/dwl/dwl-patches/patch/swapandfocusdir/swapandfocusdir.patch)
5. [bottomstack](https://codeberg.org/dwl/dwl-patches/patch/bottomstack/bottomstack.patch)
6. [shiftview](https://codeberg.org/dwl/dwl-patches/patch/shiftview/shiftview.patch)(Modifed for bar-0.7.patch)
7. [pertag](https://codeberg.org/dwl/dwl-patches/patch/pertag/pertag.patch)(Modifed for bar-0.7.patch)
8. [genericgaps](https://codeberg.org/dwl/dwl-patches/patch/genericgaps/genericgaps-0.7.patch)
9. [alwayscenter](https://codeberg.org/dwl/dwl-patches/patch/alwayscenter/alwayscenter.patch)

#### Changes that've been made to [bar](https://codeberg.org/dwl/dwl-patches/patch/bar) patch:
- Reduce `lrpad` to 0.75, for paddings around tag names
- Draw bar status on unfocused outputs, unlike the default `dwm` bar

patch involes manual patch for some other patches, due to the changes:
```diff
--- TAGSCOUNT
+++ LENGTH(tags)
```


### Building dwl v0.7
dwl has the following dependencies:
- libinput
- wayland
- wlroots0.18 (compiled with the libinput backend)
- xkbcommon
- wayland-protocols (compile-time only)
- pkg-config (compile-time only)

Also you need these dependencies because XWayland support is enabled:
- libxcb
- libxcb-wm
- wlroots0.18 (compiled with X11 support)
- Xwayland (runtime only)
