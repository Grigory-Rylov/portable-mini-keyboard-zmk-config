# ZMK прошивка для самодельной переносной клавиатуры


Combo:

```
     combos {
                compatible = "zmk,combos";

                combo_y {
                    timeout-ms = <50>;
                    key-positions = <9 12>;
                    bindings = <&kp Y>;
                };

                combo_w {
                    timeout-ms = <50>;
                    key-positions = <9 6>;
                    bindings = <&kp W>;
                };

                combo_k {
                    timeout-ms = <50>;
                    key-positions = <3 12>;
                    bindings = <&kp K>;
                };

                combo_v {
                    timeout-ms = <50>;
                    key-positions = <9 18>;
                    bindings = <&kp V>;
                };

                combo_x {
                    timeout-ms = <50>;
                    key-positions = <15 12>;
                    bindings = <&kp X>;
                };

                combo_z {
                    timeout-ms = <50>;
                    key-positions = <9 13>;
                    bindings = <&kp Z>;
                };

                combo_j {
                    timeout-ms = <50>;
                    key-positions = <8 12>;
                    bindings = <&kp J>;
                };

                combo_q {
                    timeout-ms = <50>;
                    key-positions = <9 11>;
                    bindings = <&kp Q>;
                };

                combo_enter {
                    timeout-ms = <50>;
                    key-positions = <14 19>;
                    bindings = <&kp ENTER>;
                };

                combo_esc {
                    timeout-ms = <50>;
                    key-positions = <2 7>;
                    bindings = <&kp ESCAPE>;
                };

                combo_backspace {
                    timeout-ms = <50>;
                    key-positions = <8 13>;
                    bindings = <&kp BACKSPACE>;
                };

                combo_slash {
                    timeout-ms = <50>;
                    key-positions = <14 7>;
                    bindings = <&kp SLASH>;
                };

                combo_boot {
                    timeout-ms = <50>;
                    key-positions = <0 1 14 19>;
                    bindings = <&bootloader>;
                };
            };
```
