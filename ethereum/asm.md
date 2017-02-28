With the introduction of https://github.com/ethereum/go-ethereum/pull/3686 I want to create:

* General purpose stack
        * An option for a C-like stack
        * Traditional CALL and RET opcodes
* Register

```
jump @main

func:
        push 1
        push 1
        add
        ret

main:
        call @func
```
