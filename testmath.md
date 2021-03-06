


# MathJax Notes

[MathJax Tutorial on StackExchange](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)

<ol>
<li><p>To see how any formula was written in any question or answer, including this one, right-click on the expression it and choose "Show Math As > TeX Commands". (When you do this, the '$' will not display. Make sure you add these. See the next point.)</p></li>
<li><p><strong>For inline formulas, enclose the formula in <code>$...$</code>.  For displayed formulas, use <code>$$...$$</code>.</strong><br>
These render differently. For example,
type<br>
<code>$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$</code><br>
to show <span class="math-container">$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$</span> (which is inline mode) or  type<br>
<code>$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$</code><br>
to show
<span class="math-container">$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$</span>
(which is display mode).</p></li>
<li><p>For <strong>Greek letters</strong>, use <code>\alpha</code>, <code>\beta</code>, …, <code>\omega</code>: <span class="math-container">$\alpha, \beta, … \omega$</span>.  For uppercase, use <code>\Gamma</code>, <code>\Delta</code>, …, <code>\Omega</code>: <span class="math-container">$\Gamma, \Delta, …, \Omega$</span>.</p></li>
<li><p>For <strong>superscripts and subscripts</strong>, use <code>^</code> and <code>_</code>.  For example, <code>x_i^2</code>: <span class="math-container">$x_i^2$</span>, <code>\log_2 x</code>: <span class="math-container">$\log_2 x$</span>.</p></li>
<li><p><strong>Groups</strong>. Superscripts, subscripts, and other operations apply only to the next “group”. A “group” is either a single symbol, or any formula surrounded by curly braces <code>{</code>…<code>}</code>.  If you do <code>10^10</code>, you will get a surprise: <span class="math-container">$10^10$</span>. But <code>10^{10}</code> gives what you probably wanted: <span class="math-container">$10^{10}$</span>. Use curly braces to delimit a formula to which a superscript or subscript applies: <code>x^5^6</code> is an error;  <code>{x^y}^z</code> is <span class="math-container">${x^y}^z$</span>, and <code>x^{y^z}</code> is <span class="math-container">$x^{y^z}$</span>. Observe the difference between <code>x_i^2</code> <span class="math-container">$x_i^2$</span> and <code>x_{i^2}</code> <span class="math-container">$x_{i^2}$</span>.</p></li>
<li><p><strong>Parentheses</strong> Ordinary symbols <code>()[]</code> make parentheses and brackets <span class="math-container">$(2+3)[4+4]$</span>. Use <code>\{</code> and <code>\}</code> for curly braces <span class="math-container">$\{\}$</span>.</p>

<p>These do <em>not</em> scale with the formula in between, so if you write <code>(\frac{\sqrt x}{y^3})</code> the parentheses will be too small: <span class="math-container">$(\frac{\sqrt x}{y^3})$</span>.    Using <code>\left(</code>…<code>\right)</code> will make the sizes adjust automatically to the formula they enclose: <code>\left(\frac{\sqrt x}{y^3}\right)</code> is <span class="math-container">$\left(\frac{\sqrt x}{y^3}\right)$</span>.</p>

<p><code>\left</code> and<code>\right</code> apply to all the following sorts of parentheses: <code>(</code> and <code>)</code> <span class="math-container">$(x)$</span>, <code>[</code> and <code>]</code> <span class="math-container">$[x]$</span>, <code>\{</code> and <code>\}</code> <span class="math-container">$\{ x \}$</span>, <code>|</code> <span class="math-container">$|x|$</span>, <code>\vert</code> <span class="math-container">$\vert x \vert$</span>, <code>\Vert</code> <span class="math-container">$\Vert x \Vert$</span>, <code>\langle</code> and <code>\rangle</code> <span class="math-container">$\langle x \rangle$</span>,  <code>\lceil</code> and <code>\rceil</code> <span class="math-container">$\lceil x \rceil$</span>, and <code>\lfloor</code> and <code>\rfloor</code> <span class="math-container">$\lfloor x \rfloor$</span>. <code>\middle</code> can be used to add additional dividers. There are also invisible parentheses, denoted by <code>.</code>: <code>\left.\frac12\right\rbrace</code> is <span class="math-container">$\left.\frac12\right\rbrace$</span>.</p>

<p>If manual size adjustments are required:
<code>\Biggl(\biggl(\Bigl(\bigl((x)\bigr)\Bigr)\biggr)\Biggr)</code> gives
<span class="math-container">$\Biggl(\biggl(\Bigl(\bigl((x)\bigr)\Bigr)\biggr)\Biggr)$</span>.</p></li>
<li><p><strong>Sums and integrals</strong> <code>\sum</code> and <code>\int</code>; the subscript is the lower limit and the superscript is the upper limit, so for example <code>\sum_1^n</code> <span class="math-container">$\sum_1^n$</span>. Don't forget <code>{</code>…<code>}</code> if the limits are more than a single symbol.  For example, <code>\sum_{i=0}^\infty i^2</code> is <span class="math-container">$\sum_{i=0}^\infty i^2$</span>. Similarly, <code>\prod</code> <span class="math-container">$\prod$</span>, <code>\int</code> <span class="math-container">$\int$</span>, <code>\bigcup</code> <span class="math-container">$\bigcup$</span>, <code>\bigcap</code> <span class="math-container">$\bigcap$</span>, <code>\iint</code> <span class="math-container">$\iint$</span>, <code>\iiint</code> <span class="math-container">$\iiint$</span>, <code>\idotsint</code> <span class="math-container">$\idotsint$</span>.</p></li>
<li><p><strong>Fractions</strong> There are <a href="https://math.meta.stackexchange.com/q/12978/3111">three ways to make these</a>. <code>\frac ab</code> applies to the next two groups, and produces <span class="math-container">$\frac ab$</span>; for more complicated numerators and denominators use <code>{</code>…<code>}</code>: <code>\frac{a+1}{b+1}</code> is <span class="math-container">$\frac{a+1}{b+1}$</span>. If the numerator and denominator are complicated, you may prefer <code>\over</code>, which splits up the group that it is in: <code>{a+1\over b+1}</code> is <span class="math-container">${a+1\over b+1}$</span>.
Using <code>\cfrac{a}{b}</code> command is useful for continued fractions <span class="math-container">$\cfrac{a}{b}$</span>, more details for which <a href="https://math.meta.stackexchange.com/a/5058/3111">are given in this sub-article</a>.</p></li>
<li><p><strong>Fonts</strong> </p>

<ul>
<li>Use <code>\mathbb</code> or <code>\Bbb</code> for "blackboard bold": <span class="math-container">$\mathbb{CHNQRZ}$</span>.</li>
<li>Use <code>\mathbf</code> for boldface: <span class="math-container">$\mathbf{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$</span>  <span class="math-container">$\mathbf{abcdefghijklmnopqrstuvwxyz}$</span>.</li>
<li>Use <code>\mathit</code> for italics: <span class="math-container">$\mathit{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$</span> <span class="math-container">$\mathit{abcdefghijklmnopqrstuvwxyz}$</span>.</li>
<li>Use <code>\pmb</code> for boldfaced italics: <span class="math-container">$\pmb{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$</span> <span class="math-container">$\pmb{abcdefghijklmnopqrstuvwxyz}$</span>.</li>
<li>Use <code>\mathtt</code> for "typewriter" font: <span class="math-container">$\mathtt{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$</span> <span class="math-container">$\mathtt{abcdefghijklmnopqrstuvwxyz}$</span>.</li>
<li>Use <code>\mathrm</code> for roman font: <span class="math-container">$\mathrm{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$</span>  <span class="math-container">$\mathrm{abcdefghijklmnopqrstuvwxyz}$</span>.</li>
<li>Use <code>\mathsf</code> for sans-serif font: <span class="math-container">$\mathsf{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$</span>  <span class="math-container">$\mathsf{abcdefghijklmnopqrstuvwxyz}$</span>.</li>
<li>Use <code>\mathcal</code> for "calligraphic" letters: <span class="math-container">$\mathcal{ ABCDEFGHIJKLMNOPQRSTUVWXYZ}$</span> </li>
<li>Use <code>\mathscr</code> for script letters: <span class="math-container">$\mathscr{ABCDEFGHIJKLMNOPQRSTUVWXYZ}$</span></li>
<li>Use <code>\mathfrak</code> for "Fraktur" (old German style) letters: <span class="math-container">$\mathfrak{ABCDEFGHIJKLMNOPQRSTUVWXYZ} \mathfrak{abcdefghijklmnopqrstuvwxyz}$</span>.</li>
</ul></li>
<li><p><strong>Radical signs</strong> Use <code>sqrt</code>, which adjusts to the size of its argument: <code>\sqrt{x^3}</code> <span class="math-container">$\sqrt{x^3}$</span>; <code>\sqrt[3]{\frac xy}</code> <span class="math-container">$\sqrt[3]{\frac xy}$</span>. For complicated expressions, consider using <code>{...}^{1/2}</code> instead.</p></li>
<li><p>Some <strong>special functions</strong> such as "lim", "sin", "max", "ln", and so on are normally set in roman font instead of italic font. Use <code>\lim</code>, <code>\sin</code>, etc. to make these: <code>\sin x</code> <span class="math-container">$\sin x$</span>, not <code>sin x</code> <span class="math-container">$sin x$</span>. Use subscripts to attach a notation to <code>\lim</code>: <code>\lim_{x\to 0}</code> <span class="math-container">$$\lim_{x\to 0}$$</span> Nonstandard function names can be set with <code>\operatorname{foo}(x)</code> <span class="math-container">$\operatorname{foo}(x)$</span>.</p></li>
<li><p>There are a very large number of <strong>special symbols and notations</strong>, too many to list here; see <a href="http://pic.plover.com/MISC/symbols.pdf" rel="nofollow noreferrer">this shorter listing</a>, or <a href="https://www.ctan.org/tex-archive/info/symbols/comprehensive/symbols-a4.pdf" rel="nofollow noreferrer">this exhaustive listing</a>. Some of the most common include: </p>

<ul>
<li><code>\lt \gt \le \leq \leqq \leqslant \ge \geq \geqq \geqslant \neq</code> <span class="math-container">$\lt\, \gt\, \le\, \leq\, \leqq\, \leqslant\, \ge\, \geq\, \geqq\, \geqslant\, \neq$</span>.  You can use <code>\not</code> to put a slash through almost anything: <code>\not\lt</code> <span class="math-container">$\not\lt$</span> but it often looks bad.</li>
<li><code>\times \div \pm \mp</code> <span class="math-container">$\times\, \div\, \pm\, \mp$</span>. <code>\cdot</code> is a centered dot: <span class="math-container">$x\cdot y$</span></li>
<li><code>\cup \cap \setminus \subset \subseteq \subsetneq \supset \in \notin \emptyset \varnothing</code> <span class="math-container">$\cup\, \cap\, \setminus\, \subset\, \subseteq \,\subsetneq \,\supset\, \in\, \notin\, \emptyset\, \varnothing$</span> </li>
<li><code>{n+1 \choose 2k}</code> or <code>\binom{n+1}{2k}</code> <span class="math-container">${n+1 \choose 2k}$</span> </li>
<li><code>\to \rightarrow \leftarrow \Rightarrow \Leftarrow \mapsto</code> <span class="math-container">$\to\, \rightarrow\, \leftarrow\, \Rightarrow\, \Leftarrow\, \mapsto$</span></li>
<li><code>\land \lor \lnot \forall \exists \top \bot \vdash \vDash</code> <span class="math-container">$\land\, \lor\, \lnot\, \forall\, \exists\, \top\, \bot\, \vdash\, \vDash$</span></li>
<li><code>\star \ast \oplus \circ \bullet</code> <span class="math-container">$\star\, \ast\, \oplus\, \circ\, \bullet$</span> </li>
<li><code>\approx \sim \simeq \cong \equiv \prec \lhd \therefore</code> <span class="math-container">$\approx\, \sim \, \simeq\, \cong\, \equiv\, \prec\, \lhd\, \therefore$</span> </li>
<li><code>\infty \aleph_0</code> <span class="math-container">$\infty\, \aleph_0$</span> <code>\nabla \partial</code> <span class="math-container">$\nabla\, \partial$</span> <code>\Im \Re</code> <span class="math-container">$\Im\, \Re$</span></li>
<li>For modular equivalence, use <code>\pmod</code> like this: <code>a\equiv b\pmod n</code> <span class="math-container">$a\equiv b\pmod n$</span>.</li>
<li><code>\ldots</code> is the dots in <span class="math-container">$a_1, a_2, \ldots ,a_n$</span> <code>\cdots</code> is the dots in  <span class="math-container">$a_1+a_2+\cdots+a_n$</span></li>
<li>Some Greek letters have variant forms:
<code>\epsilon \varepsilon</code> <span class="math-container">$\epsilon\, \varepsilon$</span>, <code>\phi \varphi</code> <span class="math-container">$\phi\, \varphi$</span>, and others. Script lowercase l is <code>\ell</code> <span class="math-container">$\ell$</span>.</li>
</ul>

<p><a href="http://detexify.kirelabs.org/classify.html" rel="nofollow noreferrer">Detexify</a> lets you draw a symbol on a web page and then lists the <span class="math-container">$\TeX$</span> symbols that seem to resemble it.  These are not guaranteed to work in MathJax but are a good place to start.  To check that a command is supported, note that MathJax.org maintains a <a href="http://docs.mathjax.org/en/latest/tex.html#supported-latex-commands" rel="nofollow noreferrer">list of currently supported <span class="math-container">$\LaTeX$</span> commands</a>, and one can also check Dr. Carol JVF Burns's page of <a href="http://www.onemathematicalcat.org/MathJaxDocumentation/TeXSyntax.htm" rel="nofollow noreferrer"><span class="math-container">$\TeX$</span> Commands Available in MathJax</a>.</p></li>
<li><p><strong>Spaces</strong> MathJax usually decides for itself how to space formulas, using a complex set of rules. Putting extra literal spaces into formulas  will not change the amount of space MathJax puts in: <code>a␣b</code> and <code>a␣␣␣␣b</code> are  both <span class="math-container">$a    b$</span>. To add more space, use <code>\,</code> for a thin space <span class="math-container">$a\,b$</span>; <code>\;</code> for a wider space <span class="math-container">$a\;b$</span>.  <code>\quad</code> and <code>\qquad</code> are large spaces: <span class="math-container">$a\quad b$</span>, <span class="math-container">$a\qquad b$</span>.</p>

<p>To set plain text, use <code>\text{…}</code>: <span class="math-container">$\{x\in s\mid x\text{ is extra large}\}$</span>. You can nest <code>$…$</code> inside of <code>\text{…}</code>.</p></li>
<li><p><strong>Accents and diacritical marks</strong> Use <code>\hat</code> for a single symbol <span class="math-container">$\hat x$</span>, <code>\widehat</code> for a larger formula <span class="math-container">$\widehat{xy}$</span>. If you make it too wide, it will look silly. Similarly, there are <code>\bar</code> <span class="math-container">$\bar x$</span> and <code>\overline</code> <span class="math-container">$\overline{xyz}$</span>, and <code>\vec</code> <span class="math-container">$\vec x$</span> and <code>\overrightarrow</code> <span class="math-container">$\overrightarrow{xy}$</span> and <code>\overleftrightarrow</code> <span class="math-container">$\overleftrightarrow{xy}$</span>. For dots, as in <span class="math-container">$\frac d{dx}x\dot x =  \dot x^2 +  x\ddot x$</span>,  use <code>\dot</code> and <code>\ddot</code>.</p></li>
<li><p>Special characters used for MathJax interpreting can be escaped using the <code>\</code> character: <code>\$</code> <span class="math-container">$\$$</span>, <code>\{</code> <span class="math-container">$\{$</span>, <code>\_</code> <span class="math-container">$\_$</span>, etc. If you want <code>\</code> itself, you should use <code>\backslash</code> <span class="math-container">$\backslash$</span>, because <code>\\</code> is for a new line. </p></li>
</ol>

<p>(Tutorial ends here.)</p>

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>

<script id="MathJax-script" async="" src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
