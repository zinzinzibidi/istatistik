# Momentler, Çarpıklık ve Basıklık

Momentler, çarpıklık (asimetri) ve basıklık bir serinin ortalamaya göre nasıl dağıldığını belirlemek için kullanılan temel istatistik ölçüleridir.

<table align="center">
  <tr align="center">
    <td><a href="#moment">Moment</a></td>
  </tr>
  <tr align="center">
    <td><a href="#konig">Könik Teoremi</a></td>
  </tr>
  <tr align="center">
    <td><a href="#carpiklik">Çarpıklık</a></td>
  </tr>
  <tr align="center">
    <td><a href="#basiklik">Basıklık</a></td>
  </tr>
  <tr align="center">
    <td><a href="#spss-carpiklik-basiklik">SPSS'te Çarpıklık ve Basıklık</a></td>
  </tr>
</table>

<br>

<span id="moment"></span>

## Moment

Terimlerin sıfırdan veya aritmetik ortalamadan sapmalarının çeşitli kuvvetlerine moment[^1] adı verilmektedir. Moment, bir serideki gözlem değerlerinin sıfırdan veya aritmetik ortalamadan farklarının kuvvetlerinin aritmetik ortalamasıdır.

Momentler 2 gruba ayrılır:

1. Sıfıra Göre Momentler
2. Aritmetik Ortalamaya Göre Momentler
   
### Sıfıra Göre Momentler

<div align="center">Anakütle Sıfıra Göre Momentleri</div>

<table align="center">
  <tr>
    <th>Basit Serilerde</th>
    <th>Frekans Serlerinde</th>
    <th>Gruplandırılmış Serilerde</th>
  </tr>
  <tr align="center">
    <td><pre>$$ \mu = {\Sigma X_i f_i \over N} $$</pre></td>
    <td>$$ M_1 = { \Sigma f_i X_i \over \Sigma f_i } $$</td>
    <td>$$ M_1 = { \Sigma f_i m_i \over \Sigma f_i } $$</td>
  </tr> 
</table>

$$ \begin{center}
    \begin{tabular}{ | m{7em} | m{5em}| m{9em} | } 
            \hline
        Set & operation & Identity \\ 
            \hline
        \(\mathbb{Z}\) & \(+\) & \(0\)    \\
            \hline
        \(\mathbb{Q}\) & \(+\) & \(0\)    \\
            \hline
        \(\mathbb{R}\) & \(+\) & \(0\)    \\ 
            \hline

        \(\mathbb{Z}\) & \(\times \) & \(0\)    \\
            \hline
        \(\mathbb{Q}\) & \(\times\) & \(0\)    \\
            \hline
        \(\mathbb{R}\) & \(\times\) & \(0\)    \\ 
            \hline
    \end{tabular}
\end{center} $$


[^1]: İngilizce adı da momenttir.
