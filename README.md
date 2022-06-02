# What is Vim?

- Vim is a text editor created in 1976 (vi) and 1991 (Vim)

- It enables you to edit files while using only the keyboard and keeping both hands on the home keys

- This was useful back then since one didn't have a mouse

- This is useful now since not using the mouse and keeping your hands on the home keys enables you to code faster

# See more about Vim

- [https://edwardtanguay.netlify.app/howtos?id=458]

# Vim features to know

## normal mode and insert mode :

    you start in normal mode

    i for insert mode so you can type

    ESC back to normal mode

## normal mode move:

    character: h, j, k, l

      also 5h or 7k

    word: w, e, b

    line start/end: ^, $, 0

    file start/end/all: gg, G, (cie or 1GVG)

## inserting :

    before/after character i, I, a, A

    after word: ea

    before/after line: o, O

## undo/redo

    u, CTRL-r

## move

    matching brace: %

    goto definition: gd

    go back: CTRL-o

    move to similar words: \*

    : (line number)

    move to blocks: {, }

## editing

    character: r

      also: 9r- or 9r\_
      multiple: R

    replace and type: s

      also: 3s

    join: J

    replace whole line: cc

    change word: cw, ciw

      also, rest of word: cw

      till end: C

      till character: c/"

      change camelCase part:
        e.g. 3s

      combine with . (repeat command)

    delete line: dd
      also: 3dd

    delete word: dw, diw
      till end: D
      till character: d/;

    cut: x
      swap: xp

    copy/paste word:
      yiw
      viwp

    repeat: .

    comment/uncomment: gcc

    habit: move by searching: /, ?, n, N

    move line up/down: ddkP, ddp

## visual mode selection

      three ways to select: v, V, CTRL-v
        top/bottom: o
        word: aw
        (): ab
          inner: ib
        {}: aB
          inner: iB

      action on selection
        delete/yank: d, y
        paste before/after: P, p
          at end of line: $p
        case: u, U, ~
        comment/uncomment: gc
        indent: >, <
          also: 3>

## habit: pause and consider fewest strokes possible

## "\*y

## search and replace

      :%s/this/that/g

      visual select
        :s/this/that/g

## past commands: : and arrow-up and arrow-down

## select/change/delete inner text

      change inside two tags
        cit also: dit, vit

      change inside double quotes
        ci" also: di", vi"

      change inside singl quotes
        ci' also: di', vi'

      change inside brackets
        ci) also: di), vi)
        ci} also: di}, vi}
        ci] also: di], vi]

## habit: before moving, "ma" (marker), then come back with 'a

      hop back and forth between two areas of code with ma and ms

## tabs: gt, gT

## repeat character 99 times: i= ESC d99P

## black-hole deleting: "\_dd

## :reg

## connection to operating system clipboard

      copy to: "*y
      paste from: "\*p

## close file: :wq!

## habit: be able to type numbers without looking

## sort: visual mark: :sort

## numbers: :set nu and :set nonu

## macros

      qq - record
      q - stop
      @q - execute
      @@ - execute again
