# ZMK прошивка для самодельной переносной клавиатуры


## Layout
### Primary layout

```
FPG     UDL
ARS     HNE
CTV     MOK
```
### Alpha layout

```
QW[     ]JY
ZXB     /I;
(-)     ,`.
```

Combo:

```
     combos {
                compatible = "zmk,combos";

                // --- ---
                // -X- X--
                // --- ---
                combo_left_bracket {
                     timeout-ms = <50>;
                     key-positions = <11 13>;
                     bindings = <&kp LEFT_PARENTHESIS>;
                };

                // --- ---
                // -X- --X
                // --- ---
                combo_right_bracket {
                     timeout-ms = <50>;
                     key-positions = <11 15>;
                     bindings = <&kp RIGHT_PARENTHESIS>;
                };

                // --- ---
                // --- ---
                // X-- --X
                combo_enter {
                    timeout-ms = <50>;
                    key-positions = <16 21>;
                    bindings = <&kp ENTER>;
                };

                // X-- --X
                // --- ---
                // --- ---
                combo_esc {
                    timeout-ms = <50>;
                    key-positions = <4 9>;
                    bindings = <&kp ESCAPE>;
                };

                // --- ---
                // X-- --X
                // --- ---
                combo_backspace {
                    timeout-ms = <50>;
                    key-positions = <10 15>;
                    bindings = <&kp BACKSPACE>;
                };

                // --- --X
                // --- ---
                // X-- ---
                combo_slash {
                    timeout-ms = <50>;
                    key-positions = <16 9>;
                    bindings = <&kp SLASH>;
                };

                // X-   -X
                // --- ---
                // --- ---
                // X-- --X
                combo_boot {
                    timeout-ms = <50>;
                    key-positions = <0 3 16 21>;
                    bindings = <&bootloader>;
                };

                // -X   X-
                // --- ---
                // --- ---
                // X-- --X
                combo_bt_clr_all {
                    timeout-ms = <50>;
                    key-positions = <1 2 16 21>;
                    bindings = <&bt BT_CLR_ALL>;
                };
            };
```
