set wrapmargin to 1 when line width is 80
:set wm=1

(command)(number)(text object) or (number)(command)(text object)
command(or their captials):
  w(word), b(back), a(append), c(change), d(delete), y(yank), p(put), r(replace)
  s(substitute), ~(change case), x(delete one), U(undo edits on current line)
  c2b(c 2 word backwards), c0, (c$, D), de, dE, o(open blank line), e(end)
  (change current line): cc, S, dd,

^D(down half screen), ^U(up half screen), ^E(down one line), ^Y(up one line)
z<Enter>(scroll to top), z.(scroll to center), z-(scroll to bottom)

H(move to top), M(move to middle), L(move to last line), nH, nL, +, -, <Enter>
()(sentence), {}(paragraph), [[, ]](section), n|,
d/<pattern>(delete search found), f,F,t,T(search in current line), ;,(repeat)
return to previous position ``, ''
:set nowrapscan # search forward only

$ vi +n file # +n: to line n; +: to last line; +/pattern
:pre(:preserve), "1p.u.u(search through numbered buffer)
buffer names: 0-9, a-z, A-Z(append to a-z)
Q(ex mode), d(delete), m(move), t, co(copy), m,n#, :=, :.=, :/patten/=, (=print)
.(current line), %(every line), :.,/pattern/m23, :/pattern/;+10 p, :g/pattern,
:g/pattern/p, :n1,n2g/pattern/nu, :1,3d | s/old/new, :x(write if modified exit)
:3,$w >>newfile(append line 3 to end of buffer to newfile), ar(gs), :rewind
:last, :e %(current filename), :e #(alternative filename), ^^(switch to prev f)
:g!, :v(not match)

"f4yy(yank 4 lines into buffer f), :160,224ya(nk) a, :pu(t) a, :1,30s/his/the/gc
:g/pattern/s/old/new/g

Regular Expression:
\< \>(beginning or end of a word), ~(last search used regexp)
POSIX: Character classes[: :], Collating symbols[. .], Equivalence classes[= =]
metachar in replacement string: \u(uppercase) \l(lowercase), \U \L and \e \E(end)
:%&g(Repeat the last substitution everywhere), &(:&), :~

EXINIT, .exrc, :set ic(ignore case), :set window=20, :set all, :set option?
:n1,n2!command, !)command, !10+(10!+), !!command, :ab abbr phrase, :unab abbr
:j(join), "(ex comment), ^T(>>), ^D(<<), :sfind, zn<enter>(:resize n), :windo
:bufdo[!], :buffer [n], :sbuffer [n], ^Wgf, ^Wq(:quit), ^Wo(:only), :hide
