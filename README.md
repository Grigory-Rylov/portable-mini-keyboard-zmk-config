# ZMK прошивка для самодельной переносной клавиатуры


Combo:

```
     combos {
                compatible = "zmk,combos";

                combo_enter {
                    timeout-ms = <50>;
                    key-positions = <16 21>;
                    bindings = <&kp ENTER>;
                };

                combo_esc {
                    timeout-ms = <50>;
                    key-positions = <4 9>;
                    bindings = <&kp ESCAPE>;
                };

                combo_backspace {
                    timeout-ms = <50>;
                    key-positions = <10 15>;
                    bindings = <&kp BACKSPACE>;
                };

                combo_slash {
                    timeout-ms = <50>;
                    key-positions = <16 9>;
                    bindings = <&kp SLASH>;
                };

                combo_boot {
                    timeout-ms = <50>;
                    key-positions = <0 3 16 21>;
                    bindings = <&bootloader>;
                };
            };
```
