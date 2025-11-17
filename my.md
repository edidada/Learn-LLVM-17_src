# my

Basic
CodeGen
Lexer
Parser
Sema

sudo apt install -y llvm-17 llvm-17-dev clang-17 libllvm-17-ocaml-dev

## Chapter02 calc
llvm::StringRef

```shell
/mnt/d/develops/git/github/cpp/Learn-LLVM-17_src/cmake-build-debug-wsl24/Chapter02/calc/src/calc 1+2
; ModuleID = 'calc.expr'
source_filename = "calc.expr"

define i32 @main(i32 %0, ptr %1) {
entry:
call void @calc_write(i32 3)
ret i32 0
}

declare void @calc_write(i32)

Process finished with exit code 0
```

## 3
/mnt/d/develops/git/github/cpp/Learn-LLVM-17_src/cmake-build-debug-wsl24/Chapter03/tinylang/tools/driver/tinylang Gcd.mod
Tinylang 0.1