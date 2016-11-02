PyCon CZ 2016 workshop
=======================


V prvom kroku si nainštalujeme virtuálne prostredie, v ktorom budeme našu aplikáciu vyvíjať a spúštať. Virtuálne prostredie slúži k oddeleniu rôznych inštalácií balíčkov, verzií Pythonu na jednom počítači. Taktiež ak sa niečo v projekte pokazí, ktorý je vytvorený v rámci daného virtuálneho prostedia, neohrozí to ďalšie projekty na počítači.

Úlohy:

1. Otvor si príkazový riadok (terminál - Mac OS, Linux)

2. Zvoľ si adresár, v ktorom budeš mať vytvorený projekt a následne pracovať.

3. Naviguj sa do adresára

4. Vytvor novú složku a vstúp do novo-vytvorej zložky

5. Vytvor virtuálne prostredie. Príkazy pre vytvorenie virtuálneho prostredia sa líšia podľa operačného systému:

Windows:

<pre><code>> py 3 -m venv venv </code></pre>

Linux/Mac OS:

<pre><code>$ python3 -m venv venv </code></pre>

Po vytvorení virtuálneho prostredia je potrebné ho **spustiť.** . Spustenie virtuálneho prostredia sa taktiež líši podľa operačného systému:

Windows:

<pre><code>>\venv\Scripts\activate</code></pre>

Linux/Mac OS:

<pre><code>$ source /venv/bin/activate </code></pre>

Po spustení by malo ukázať pred <code> > </code> alebo <code>$</code> slovo <code>(venv)</code>.

<pre><code>(venv) MacBook-Pro:pyconworkshop svetlanamargetova$ </code></pre>

## Inštalácia potrebných knižníc

Na inštaláciu budeme využívať [pip](https://pypi.python.org/pypi/pip). 

## Inštalácia cez Anacondu
[Anaconda](https://www.continuum.io/downloads) - obsahuje všetky potrebné balíčky pre prácu. Tí, čo anacondu inštalovať nechcú, pokračujte pokynmi nižšie.

### Inštalácia Jupyter Notebook

[Jupyter](http://jupyter.org/) notebook je webová aplikácia, ktorá umožňuje zdielať a vytvárať dokumenty obsahujúce "živý" kód, vizualizácie, markdown system, HTML kód a mnoho iného.

<pre><code>$ pip install jupyter </code></pre>

### Inštalácia pandas

[Pandas](http://pandas.pydata.org/) je knižnica umožňujúca prácu s dátovými štruktúrami rôznych formátov v Pythone.

<pre><code>$ pip install pandas</code></pre>

V rámci Pandas sa nám naištalovala aj potrebná knižnica numpy. 

### Inštalácia matplotlib

[Matplotlib](http://matplotlib.org/) je knižnica vykresľujúca 2D vizualizácie v Pythone v rôznych formátoch. Umožňuje vykreslovať rôzne druhy grafov, ukladať výstupy v rôznych formátoch.

<pre><code>$ pip install matplotlib</code></pre>

### Inštalácia scipy

[Scipy](https://www.scipy.org/) je knižnica obsahujúca rôzne štatistické a iné funkcie.

<pre><code>$ pip install scipy</code></pre>

## Spustenie Jupyter notebooku

Po nainštalovaní potrebných knižníc si môžeme spustiť na localhoste Jupyter notebook pomocou príkazu:

<pre><code>$ jupyter notebook</code></pre>


Dátové sety
--------------
Vytvor zložku "csv" v hlavnom adresári projektu. Následne stiahni dátové sety a ulož do složky "csv".

1. Dátový set [Instagramu](https://www.dropbox.com/s/otpw5i51y7ugr95/martinus_sk.csv?dl=0)
2. Dátový set [kníh](https://www.dropbox.com/s/evqcgmdh6xzyemj/martinus_db.csv?dl=0)
3. Dátový set [používatelia](https://www.dropbox.com/s/l07zudw93wzkiq9/users.csv?dl=0)


Instagram skript
--------------------
Skript na sťiahnutie dát z rôznych Instagram účtov - [InstagramToCsv](https://github.com/SvetlanaM/InstagramToCsv)

ToDo
--------------------
1. Sťahovať vždy na začiatku práce aktuálne dáta z Instagramu 
2. Zautomatizovať spracovanie clusterov bez nutnosti zadávať hodnoty ručne používateľom
3. Rozpoznávanie názvu kníh z obrázku, kde nie je hashtag (nice to have)
4. Poslať výstup priamo cez API na server 

