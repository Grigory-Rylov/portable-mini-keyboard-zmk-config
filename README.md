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

                // --- ---
                // --- -X-
                // X-- ---
                combo_cmd_c {
                    timeout-ms = <50>;
                    key-positions = <16 14>;
                    bindings = <&kp SLASH>;
                };

                // --- ---
                // --- -X-
                // --V ---
                combo_cmd_v {
                    timeout-ms = <50>;
                    key-positions = <18 14>;
                    bindings = <&kp SLASH>;
                };

                // --- ---
                // X-- -X-
                // --- ---
                combo_cmd_z {
                    timeout-ms = <50>;
                    key-positions = <10 14>;
                    bindings = <&kp SLASH>;
                };

                // --- ---
                // -X- -X-
                // --- ---
                combo_cmd_x {
                    timeout-ms = <50>;
                    key-positions = <11 14>;
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
            };
```
