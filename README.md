
<h1 align=center><font size = 5>Building Software to Calculate Legendre Differential Equations</font></h1>

<img  src="https://www.generic-mapping-tools.org/remote-datasets/_images/GMT_geoid.jpg"  alt="generic-mapping-tools.org">

<small>Picture Source:<a  href="https://www.generic-mapping-tools.org/remote-datasets/"> Wine Generic Mapping Tools</a></small>

<br>

<h2>Statement</h2>

<p>The aim of the project, as can be understood from the title, is to developing an application that can calculate <i>legendre differential equations with Python 3.7</i> and save them in <i>excel table</i>. These operations were carried out through the <i>PyQt5</i> library and the <i>Designer</i> application. In addition, you can find variations of the program (with graph, without graph) in the branch.</p>

<h2>Methodology</h2>

<h3>Unnormalized function</h3>

$$P_{nm}(t) = 2^{-m} \cdot (1-t^{2})^{\frac{m}{2}} \cdot \sum_{k=0}^{r} (-1)^{k} \cdot \frac{(2n - 2k)! \cdot t^{n-m-2k}}{k!(n-k)!(n-m-2k)!}$$

<br>

<h3>Normalized function</h3>

$$P_{nm}(t) = 2^{-m} \cdot (1-t^{2})^{\frac{m}{2}} \cdot \sum_{k=0}^{r} (-1)^{k} \cdot \frac{(2n - 2k)! \cdot t^{n-m-2k}}{k!(n-k)!(n-m-2k)!} \cdot \sqrt{\frac{2^{2(n+1)} \cdot (n-m)!}{(n+m)!}}$$

<br>

<p>In mathematics, the associated legendre polynomials are the canonical solutions of the general <i>legendre equation</i>. This equation has nonzero solutions that are nonsingular on <i>(−1, 1)</i> only if n and m are integers with <i>0≤m≤n</i>, or with trivially equivalent negative values. When in addition <i>m</i> is even, the function is a <i>polynomial</i>. When <i>m</i> is zero and n integer, these functions are identical to the <i>legendre polynomials</i>.</p>

In this part of work we are going to calculate the values of the $P_{nm}$ normalized values. <i>normalized.png</i> is the mathematical equation of normalized legendre equation and <i>unnormalized.jpg</i>  is the mathematical equation of <i>unnormalized legendre equation</i>. <b>Normalized values  were calculated in project.</b>

<br>

<h2>UI Overview:</h2>

![UI](UI.jpg)

<br>

<h2>Analysis</h2>

<p>You can examine the excel output, where <i>n</i> and <i>m</i> values ​​are <i>10</i>, on the <i>output.xlsx</i> file. The same output is also shown in the application interface. In order for it to be saved as Excel as optional, it must first be written in the relevant field, indicating the name of the file. (for example: '<i>C:\Users\User\Desktop\output.xlsx</i>')</p>

<br>

<h2>File Conversions</h2>

<p>Before doing these operations, <b>you need to go to the location on command prompt where the Calculating_Pnm_excel.ui and <i>Calculating_Pnm_excel.py</i> files are located.</b> These procedures were done by myself. You are free to make <code>.exe</code> file from <code>.py</code> file. Those who are curious about how it is made or who want to learn can try this section on their own.</p>

<h3>.ui to .py</h3>

    python -m PyQt5.uic.pyuic -x Calculating_Pnm_excel.ui -o Calculating_Pnm_excel.py

<br>

<h3>.py to .exe</h3>

    pyinstaller.exe --onefile --windowed --icon=app.ico Calculating_Pnm_excel.py

<br>

<h2>Contact Me</h2>

<p>If you have something to say to me please contact me:</p> 

<ul>
	<li>Twitter: <a  href="https://twitter.com/Doguilmak">Doguilmak</a></li>
	<li>Mail address: doguilmak@gmail.com</li>
</ul>
