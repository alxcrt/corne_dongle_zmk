# Corn split keyboard firmware
This repo contians the firmware / keymap for the [typeractive corn](https://typeractive.xyz/) split keyboard. 
The preferred way to edit the keymap is to use the [web gui](https://nickcoutsos.github.io/keymap-editor/).

# Lessons learned
- You can use the correctly rendered icons instead of using the round-about way via modifier key. E.g.: Instead of `SHIFT+4`, you can `DOLLAR`. Note: Refering to web gui!
- If the direct firmware upload does not work, you can try to set `CONFIG_ZMK_STUDIO=n` in `config/corne.conf`. This solved it for me :)
- Mod-tap (`&mt`) is awesome! But the default behavior can be bothersome if you mash keys and don't press them 100% correctly. It can be changed to a more noob-friendy way by adding `&mt { flavor = "tap-preferred"; };` to `config/corne.keymap` -> See [here](https://zmk.dev/docs/keymaps/behaviors/hold-tap#flavors) for a super detailed Documentation. Note: This can also be done in the gui under `behaviors -> Reconfigurations`. Yes, this also exists for layers with the `&lt` - layer_tap command :)
