# Bilgisayar Bilimini Kendi Kendinize Öğrenin 

> This document is a Turkish translation of [TeachYourselfCS](https://teachyourselfcs.com), written by [Ozan Onay](https://twitter.com/oznova_) and [Myles Byrne](https://twitter.com/quackingduck). For more information about this translation, please refer to [the end of this document](#bunu-kim-çevirdi).


Eğer kendi kendini eğitmiş bir mühendis ya da eğitim kampı mezunuysanız, bilgisayar bilimi öğrenmeyi kendine borçlusun. Neyse ki, bir lisansa yıllar ve kendine küçük bir servet harcamadan birinci sınıf bir Bilgisayar Bilimi eğitimi verebilirsiniz 💸.

İnternet üzerinde birçok kaynak var, ancak bazıları diğerlerinden daha iyi. Başka bir “200+ Ücretsiz Çevrimiçi Kurslar” listesi veren kısa yazıya ihtiyacınız yok. Bu soruların cevaplarına ihtiyacınız var:

* Hangi konuyu öğrenmelisin, ve neden?
* Her konu için en iyi kitap ve video ders serisi hangisi?

Bu kılavuz bu sorulara kesin cevaplar bulabilmek için girişimimizdir.

## TL;DR: (Özet)

Önerilen ders kitabını veya video dersleri, ancak tercihen her ikisini de kullanarak aşağıdaki dokuz konuyu kabaca verilen sırayla çalışınız. Her konuyu 100-200 saat çalışmayı hedefleyiniz, sonra kariyeriniz boyunca tekrar ele alınız 🚀.



| Konu                                           | Neden öğrenmeliyim?                                                                                                                                | Kitap                                               | Videolar                       |
|---------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------|-----------------------------------|
| **[Programlama](#Programlama)**                   | Özyineleme gibi bir şeyi “Asla tam olarak anlamayan” kişi olmayın.                                                                | _Structure and Interpretation of Computer Programs_     | Brian Harvey Berkeley CS 61A    |
| **[Bilgisayar Mimarisi](#bilgisayar-mimarisi)**  | Bir bilgisayarın gerçekte nasıl çalıştığına dair sağlam bir zihinsel modelin yoksa, tüm üst düzey soyutlamaların kırılgan olacaktır.           | _Computer Systems: A Programmer's Perspective_                      | Berkeley CS 61C                   |
| **[Algoritmalar ve Veri Yapıları](#algoritmalar-ve-veri-yapıları)**| Yığınlar, kuyruklar, ağaçlar ve grafikler gibi her yerde bulunan veri yapılarını nasıl kullanacağını bilmiyorsan, zorlu sorunları çözemezsin. | _The Algorithm Design Manual_                           | Steven Skiena’s lectures          |
| **[Bilgisayar Bilimi(CS) için Matematik](#bilgisayar-bilimi(CS)-için-matematik)**                   | Bilgisayar Bilimi aslında uygulamalı matematiğin kaçak bir dalı, bu yüzden matematik öğrenmek sana rekabetçi bir üstünlük verecektir.                                 | _Mathematics for Computer Science_                      | Tom Leighton MIT 6.042J         |
| **[İşletim Sistemleri](#işletim-sistemleri)**   | Yazdığın çoğu kod bir işletim sistemi tarafından çalıştırılıyor, bu yüzden nasıl etkileşime geçeceğini bilmelisin.                                          | _Operating Systems: Three Easy Pieces_                  | Berkeley CS 162                   |
| **[Bilgisayar Ağı](#bilgisayar-ağı)**           | İnternet büyük bir mesele haline geldi: tam potansiyelini ortaya çıkarmak için nasıl çalıştığını anlayın.                                           | _Computer Networking: A Top-Down Approach_              | Stanford CS 144                   |
| **[Veri tabanları](#veri-tabanları)**                 | Veri birçok önemli programın temelindedir ama çok az kişi veri tabanlarının nasıl çalıştığını anlar.                                 | _Readings in Database Systems_                          | Joe Hellerstein Berkeley CS 186 |
| **[Diller ve Derleyiciler](#diller-ve-derleyiciler)**       | Dillerin ve derleyicilerin aslında nasıl çalıştığını anlarsan, daha iyi bir kod yazarsın ve yeni dilleri daha kolay öğrenirsin.               | _Crafting Interpreters_           | Alex Aiken’s course on edX   |
| **[Dağıtık Sistemler](#dağıtık-sistemler)** | Bu günlerde çoğu sistem dağıtık sistemdir.                                                   | _Designing Data-Intensive Applications by Martin Kleppmann_ | MIT 6.824                         |
                     

## Hala çok mu fazla?

Yıllarca 9 konu üzerinde kendi kendine çalışma fikri bunaltıcı hissettiriyorsa, şu iki kitap üzerinde durmanı öneriyoruz: Computer Systems: A Programmer's Perspective ve Designing Data-Intensive Applications. Tecrübelerime göre, bu iki kitap ağ tabanlı uygulamalar üzerinde çalışan özellikle kendi kendini yetiştiren mühendisler ve eğitim kampı mezunları için yatırılan zamandan oldukça getiri sağlar. Ayrıca yukarıda listelenen diğer konular ve kaynaklar için bir “geçiş maddesi” olabilir.

> The global SMS system does around 20bn messages a day. WhatsApp is now doing 42bn. With 57 engineers. [pic.twitter.com/zZrtSIzhlR](https://t.co/zZrtSIzhlR)

> — Benedict Evans (@BenedictEvans) [Feb 2, 2016](https://twitter.com/BenedictEvans/status/694342874729545729)

## Neden bilgisayar bilimi öğrenmelisin?
İki tip yazılım mühendisi vardır: bilgisayar bilimini zorlu ve yenilikçi işi yapabilecek kadar anlayabilen ve birkaç yüksek seviye araçlarla aşina oldukları için sadece idare edenler.

Her ikisi de kendilerine yazılım mühendisi diyor ve ikisi de kariyerlerinin başlarında benzer maaş almaya eğilimli. Ancak Tip 1 mühendisler, değerli ticari işler veya çığır açan açık kaynaklı projeler, teknik liderlik veya yüksek kaliteli bireysel katkılar olsun, zamanla daha tatmin edici ve emeğinin karşılığını iyi veren işlere doğru ilerler.

Tip 1 mühendisleri, ister geleneksel yollarla ister kariyerleri boyunca durmaksızın öğrenerek bilgisayar bilimini derinlemesine öğrenmenin yollarını bulur. Tip 2 mühendisler genellikle yüzeyde kalır, belirli araçları öğrenir ve altında yatan temeller yerine teknolojileri öğrenir ve sadece teknik moda yön değiştirdiğinde yeni beceriler kazanır.

Şu anda, Bilgisayar Bilimi mezun sayısı değişmez iken bu endüstriye giren insanların sayısı hızla artıyor. Tip 2 mühendislerinin fazlalığı onların istihdam fırsatlarını azaltmaya başladı ve endüstrinin daha tatmin edici işlerinin dışında tuttu. İster Tip 1 mühendis olmak için mücadele edin ister basitçe daha güvenli bir iş arayın, bilgisayar bilimi öğrenmek tek güvenli yol.


> Lol oh but they were….[pic.twitter.com/XVNYlXAHar](https://t.co/XVNYlXAHar)

>

> — Jenna Bilotta (@jenna) [4 Mar, 2017](https://twitter.com/jenna/status/838161631662092289)

## Konu rehberleri

### Programlama

Çok Bilgisayar Bilimi lisans programları, bilgisayar programlamaya bir “giriş” ile başlıyor. Bu kursların en iyileri, sadece acemiler için değil aynı zamanda kod yazmayı öğrenmeye ilk başladıklarında yararlı kavramları ve programlama modellerini kaçıranlar için.

Bu içerik için genel tavsiyemiz, hem [kitap](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html) hem de [MIT video dersleri](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/) çevrimiçi ve ücretsiz olan klasik Structure and Interpretation of Computer Programs’dır. Bu dersler harikayken bizim asıl önerimiz Brian Harvey’s SICP dersleridir (Berkeley’deki 61A dersi). Bunlar MIT derslerinden daha arıtılmış ve yeni öğrenci odaklı.

SICP’nin en az ilk üç bölümü üzerinde detaylı incelemeni ve alıştırmaları yapmanı tavsiye ediyoruz. Ek alıştırma için, [exercism](http://exercism.io)’dekiler gibi bir takım programlama problemlerini detay ile ele alın.

Bu kılavuz ilk defa 2016 yılında yayınlandığı için sıklıkla karşılaştığımız sorulardan biri, John DeNero’nun ders verdiği 61A’nın daha yakın zamandaki bir kayıtı ve/veya “SICP’ye benzeyen” ama Python kullanılan [Composing Programs](https://composingprograms.com/)’nın yerini tutabilecek bir kitap olup olmadığı. DeNero’nun kaynakları da iyi olduğunu düşünüyoruz ve bazı öğrenciler onu tercih edebilir ancak denemek için kaynaklardan ilk takımı olarak biz hala SICP, Scheme ve Brian Harvey’in derslerini öneriyoruz.

Neden mi? Çünkü SICP en azından imkanlar dahilinde bilgisayarlar ve programlama hakkında temel inançlarını değiştirme yeteneği açısından eşsiz. Herkes bunu tecrübe etmeyecek. Bazıları kitaptan nefret ederken diğerleri ilk birkaç sayfayı geçmeyecek. Ancak olası ödül onu denemeye değer kılıyor.

Eğer SICP’den hoşlanmadıysan, Composing Programs’ı deneyin. Hala sana uymadıysa [How to Design Programs](http://htdp.org/)’ı deneyin. Eğer bunlardan herhangi biri çabanı ödüllendirecek gibi gözükmüyorsa, belki bir süre için başka konular üzerine odaklanman için bir işarettir ve birkaç yıl içinde programlama bilimini tekrar ziyaret et.

Sonunda bir açıklama: bu kılavuz programlamaya tamamen yeni başlamışlar için değil. Bilgisayar biliminde altyapısı olmayan ve bazı konulardaki bilgi boşluklarını doldurmayı uman yetkin bir programcı olduğunu varsayıyoruz. Gerçek şu ki “programlama” bölümünü dahil etmemiz, konu hakkında öğrenilecek daha çok şeyin olabileceğini basitçe hatırlatmaktır. Daha önceden hiç kod yazmamış ama yazmak isteyen böyle bir [kılavuzu](https://www.reddit.com/r/learnprogramming/wiki/faq#wiki_getting_started) tercih edebilirler.

### Bilgisayar Mimarisi

Bazen “bilgisayar sistemleri” ya da “bilgisayar örgütleşimi” diye adlandırılan Bilgisayar Mimarisi, program yüzeyinin altında önemli bir ilk bakıştır. Deneyimimize göre kendini eğiten yazılım mühendisleri arasında en çok ihmal edilen alandır.

[Computer Systems: A Programmer's Perspective](http://csapp.cs.cmu.edu/3e/home.html) tercih ettiğimiz giriş kitabımızdır ve kitabı kullanan normal bir  bilgisayar mimarisine giriş dersi birden altıncı bölüme kadar çoğu kısmı kapsar.

CS:APP’i pratik, yazılımcıya yönelik yaklaşımı için seviyoruz. Bilgisayar mimarisine dair kitabın içerdiğinden çok daha fazla şey olduğu halde, ilk olarak daha hızlı, etkili ve güvenilir bir yazılım yazmak için bilgisayar sistemlerini anlamak isteyenler için çok iyi bir başlangıç noktası işlevini görüyor.

Hem daha hafif bir başlangıcı hem de donanım ve yazılım dengesini tercih edenler için “Nand2Tetris” olarak da bilinen “The Elements of Computing Systems”ı öneriyoruz. Size bir bilgisayardaki her şeyin nasıl çalıştığına dair tutarlı bir anlayış vermeye çalışan iddialı bir kitap. Her bölüm, HDL’de temel mantık kapılarının yazımından, işlemci ve çevirici yoluyla bir Tetris oyununun boyutundaki bir uygulamaya, tüm sistemin bir parçasını kurumunu içeriyor.

Kitabın ilk altı bölümünü okumanızı ve ilişkin projeleri tamamlamanızı öneriyoruz. Makinenin mimarisi ile onda çalışan yazılım arasındaki ilişkinin anlayışınızı geliştirecek.

Kitabın ilk yarısı (ve tüm projeleri), [Nand2Tetris’in internet sitesinde](http://www.nand2tetris.org/) ücretsiz olarak mevcut. Ek videolarla birlikte [Coursera](https://www.coursera.org/learn/build-a-computer) kursu olarak da mevcut. Basitlik ve tutarlılık arayışında, Nand2Tetris derinlikten fedakârlık eder. Özellikle modern bilgisayar mimarilerindeki iki önemli kavram pipelining ve bellek hiyerarşisidir ancak ikisi de çoğunlukla metinlerde mevcut değildir.

Nand2Tetris içeriğiyle rahat hissettiğinizde, ya CS:APP’a geri dönmenizi ya da Patterson ve Hennessy’nin harika ve bir klasik eser olan [Computer Organization and Design](https://smile.amazon.com/Computer-Organization-Design-Fifth-Architecture/dp/0124077269)’ını göz önünde bulundurmanızı öneriyoruz. Kitaptaki her bölüm esas değildir, özel okumalar için Berkeley’in [CS61C](http://inst.eecs.berkeley.edu/~cs61c/sp15/) “Great Ideas in Computer Architecture” dersini takip etmenizi öneriyoruz. Ders notları ve laboratuvar dersleri çevrimiçi olarak ve eski dersler [İnternet Arşivinde](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iCl2-D-FS5mk0jFF6cYSJs_) mevcuttur.

[![Elements of Computing Systems](https://teachyourselfcs.com/elements-computing-systems.jpg)](http://www.nand2tetris.org)

### Algoritmalar ve Veri Yapıları

Yaygın algoritma ve veri yapılarına aşinalığın bilgisayar bilimi eğitiminin en güçlendirici taraflarından biri olduğu konusunda onlarca yıllık süren ortak bilgeliğe katılıyoruz.

Yüzlerce kitap mevcut ancak bizim gözdemiz Steven Skiena’nın _[The Algorithm Design Manual](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/)._Açıkla algoritmik problem çözmeyi seviyor ve genellikle öğrencileri ve okuyucuları arasında benzer bir coşku uyandırmayı başarıyor. Bize göre, daha yaygın iki önerilen metin (CLRS ve Sedgewick) öncelikle pratik problem çözmeye yardımcı olmak için materyali öğrenenler için ispat kısmı biraz daha ağır basma eğilimindedir. 

[Skiena](https://www.youtube.com/watch?v=A2bFN3MyNDA&list=PLOtl7M3yp-DX32N0fVIyvn7ipWKNGmwpp), video dersleri tercih edenler için cömertçe çevrimiçi olarak sağlar. Ayrıca Tim Roughgarden’in [Coursera](https://www.coursera.org/specializations/algorithms)’da ve [başka yerlerde](http://timroughgarden.org/videos.html) mevcut olan kursunu da çok seviyoruz.Skiena's veya Roughgarden’ın ders stilini tercih edip etmediğiniz kişisel tercih meselesi olacaktır. Aslında, düzinelerce iyi alternatif var, bu yüzden hoşunuza giden başka bir alternatif bulursanız, ona bağlı kalmanızı öneririz!

Uygulama için tercih ettiğimiz yaklaşım, öğrencilerin Leetcode üzerindeki problemleri çözmesidir. Bu problemler, eşlik eden uygun çözümler ve tartışmalar ile ilginç problemler olma eğilimindedir. Ayrıca, daha rekabetçi yazılım şirketlerinde teknik mülakatlarda yaygın olarak kullanılan sorulara karşı ilerlemeyi test etmenize yardımcı olurlar. Çalışmalarınızın bir parçası olarak yaklaşık 100 rastgele leetcode problemini çözmenizi öneririz.

Son olarak şiddetle [How to Solve It](https://www.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/)’i genel problem çözmeye konusu için mükemmel ve özgün bir kılavuz olarak öneririz, matematiğe olduğu gibi bilgisayar bilimine de uygulanabilir. 

[![The Algorithm Design Manual](https://teachyourselfcs.com/skiena.jpg)](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/) [![How to Solve It: A New Aspect of Mathematical Method (Princeton Science Library)](https://teachyourselfcs.com/polya.jpg)](https://www.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/) 

> Geniş ölçüde önerdiğim tek bir yöntemim var, sanırım yazmadan önce düşün denebilir.
>
>— Richard Hamming

### Bilgisayar Bilimi için Matematik

Bazı açılardan bilgisayar bilimi, uygulamalı matematiğin aşırı gelişmiş bir dalıdır. Pek çok yazılım mühendisi bunu görmezden gelmek için çabalar ve çeşitli derecelerde başarılı olurken, biz sizi doğrudan çalışmayla kucaklamanızı öneririz. Bunu başarılı bir şekilde yapmak, başaramayanlara göre size muazzam bir rekabet avantajı sağlayacaktır.

Bilgisayar bilimi için matematiğin en ilgili alanı, genel olarak "ayrık matematik" olarak adlandırılır. Burada "ayrık", "sürekli"nin zıttıdır ve genel hatlarıyla Kalkülüs dışındaki ilginç uygulamalı matematik konularının bir derlemesidir. Belirsiz tanım göz önüne alındığında, "ayrık matematiğin" tüm genişliğini kapsamaya çalışmak anlamsızdır. Mantığın, kombinatoriğin ve olasılığın, kümeler teorisinin, çizge teorisinin ve biraz da kriptografi hakkında bilgilendiren sayılar teorisinin çalışan bir anlayışını inşa etmek daha gerçekçi bir hedeftir. Bilgisayar grafikleri ve makine öğrenmesindeki önemi göz önünde bulundurulduğunda doğrusal cebir zahmete değer ek bir çalışma alanıdır.


Ayrık matematik için önerdiğimiz başlama noktası [László Lovász’ın ders notlarıdır](http://www.cs.elte.hu/~lovasz/dmbook.ps). Profesör Lovász, içeriği ulaşılabilir ve anlaşılması kolay hale getirme konusunda iyi bir iş çıkardı, bu nedenle daha resmi metinlerden daha iyi bir başlangıç noktası.

Daha ileri seviye bir yaklaşım için aynı yazarın kitap uzunluğundaki ders notları olan [Mathematics for Computer Science](https://courses.csail.mit.edu/6.042/spring17/mcs.pdf)’ı öneriyoruz. Ayrıca video dersleri ücretsiz olarak mevcuttur ve ayrık matematik için önerdiğimiz video derslerdir.

Doğrusal cebir için [Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) videolarıyla başlamanızı, ardından Gilbert Strang’in [kitap](https://www.amazon.com/Introduction-Linear-Algebra-Gilbert-Strang/dp/0980232775/) ve [video derslerini](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/video-lectures/) öneririz.

> Eğer insanlar matematiğin kolay olduğuna inanmıyorlarsa, sadece hayatın ne kadar karmaşık olduğunu fark etmedikleri içindir.
>
>— John von Neumann

### İşletim Sistemleri

_[Operating System Concepts](https://www.amazon.com/dp/1118063333/)_ ve _[Modern Operating Systems](https://www.amazon.com/dp/013359162X/)_ klasik işletim sistemleri kitaplarıdır. Her ikisi de açık olmadıkları ve genel olarak öğrenci tarafından anlaşılmaması nedeniyle eleştirildi.

_Operating Systems: Three Easy Pieces_ [ücretsiz ve çevrimiçi mevcut](http://pages.cs.wisc.edu/~remzi/OSTEP/) olan iyi bir alternatiftir. Özellikle kitabın yapısı ve okunabilirliğini beğeniyoruz ve alıştırmaların faydalı olduğunu hissediyoruz.

OSTEP’ten sonra belirli işletim sistemlerinin dizayn kararlarını “{İşletim sistemi adı} Internals” -[Lion's commentary on Unix](https://www.amazon.com/Lions-Commentary-Unix-John/dp/1573980137/)_, _[The Design and Implementation of the FreeBSD Operating System](https://www.amazon.com/Design-Implementation-FreeBSD-Operating-System/dp/0321968972/) ve _[Mac OS X Internals](https://www.amazon.com/Mac-OS-Internals-Systems-Approach/dp/0321278542/)_ gibi kitaplarla keşfetmenizi destekliyoruz.

İşletim sistemleri anlayışınızı pekiştirmenin harika bir yolu, küçük bir çekirdeğin kodunu okumak ve özellikler eklemektir. ANSI C için bir unix V6 portu olan [xv6](https://pdos.csail.mit.edu/6.828/2016/xv6.html) ve MIT'deki bir kurs için muhafaza edilen x86 bir seçenektir. OSTEP potansiyel projeler için harika fikirlerle dolu olası [xv6 laboratuvarlarının](http://pages.cs.wisc.edu/~remzi/OSTEP/lab-projects-xv6.pdf) bir ekine sahiptir.

### Bilgisayar Ağı

Yazılım mühendisliğinin büyük bir kısmının web sunucularında ve istemcilerde olduğu düşünüldüğünde, bilgisayar biliminin en değerli alanlarından biri bilgisayar ağıdır. Ağ kurmayı metodik olarak inceleyen ve kendi kendini yetiştiren öğrencilerimiz, sonunda yıllardır içinde bulundukları terimleri, kavramları ve protokolleri anladıklarını fark ediyorlar.

Konuyla ilgili favori kitabımız _[Computer Networking: A Top-Down Approach](https://smile.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/)_’dır. Kitaptaki küçük projeler ve alıştırmalar yapmaya değer ve özellikle [cömertçe çevrimiçi olarak sağladıkları](http://www-net.cs.umass.edu/wireshark-labs/) “Wireshark labs”ları beğeniyoruz.

Video dersleri tercih edenler için daha önceden Standford’un MOOC platformu Lagunita üzerinde mevcut olan _[Introduction to Computer Networking course](https://www.youtube.com/playlist?list=PLvFG2xYBrYAQCyz4Wx3NPoYJOFjvU7g2Z)_’u öneriyoruz ama şu an üzücü şekilde sadece Youtube’daki resmi olmayan oynatma listesinde mevcut. 

>Kristal küreye bakıp geleceği göremezsin. Gelecekte internet, toplumun yonttuğu şekilde olacaktır.  
>
>— Bob Kahn

[![Computer Networking: A Top-Down Approach](https://teachyourselfcs.com/top-down.jpg)](https://www.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/) 

### Veri tabanları

Diğer birçok konuya kıyasla, veri tabanı sistemleri hakkında kendi kendine öğrenmek daha fazla çalışma gerektirir. Fikirlerin kapalı kapılar ardında kalmasına yönelik güçlü ticari teşviklere sahip nispeten yeni (yani 1970 sonrası) bir çalışma alanıdır. Ek olarak, olası mükemmel birçok yazar ders kitabı yazmak yerine şirketlere katılmayı veya kurmayı tercih etti.

Koşullar göz önüne alındığında kendi kendine öğrenenleri genel olarak ders kitaplarından kaçınmaya ve Joe Hellerstein’ın Berkeley’deki veri tabanları dersi CS 186’nın kayıtlarıyla başlamaya ve sonrasında makale okumaya devam etmeye teşvik ediyoruz.

Yeni öğrenciler için özellikle bahsetmeye değer bir makale, ilişkisel veri tabanı yönetim sistemlerinin (RDBMS) nasıl çalıştığına ilişkin benzersiz bir şekilde yüksek düzeyde bir görünüm sağlayan [“Architecture of a Database System”](http://db.cs.berkeley.edu/papers/fntdb07-architecture.pdf) yeni öğrenciler için özellikle bahsetmeye değer bir makaledir. Bu ileri çalışma için bir taslak görevi görecek.

Readings in Database Systems daha çok bilinen adıyla [veri tabanları “Red Book”,](http://www.redbook.io/) Peter Bailis, Joe Hellerstein ve Michael Stonebraker tarafından derlenmiş ve düzenlenmiş makalelerin bir koleksiyonudur. CS 186 içeriğinin seviyesinin üstünde olan kişilerin bir sonraki durağı Red Book olmalı. Eğer tanıtıcı kitap kullanmakta ısrarcı iseniz, Ramakrishan ve Gehrke’nin _[Database Management Systems](https://smile.amazon.com/Database-Management-Systems-Raghu-Ramakrishnan/dp/0072465638/)_’i öneririz. Daha ileri seviye öğrenciler için Jim Gray’in klasik _[Transaction Processing: Concepts and Techniques](https://www.amazon.com/Transaction-Processing-Concepts-Techniques-Management/dp/1558601902)_ zahmete değer ancak ilk kaynak olarak kullanmanızı desteklemiyoruz.

Son olarak, veri modelleme, veri tabanları ile çalışmanın ihmal edilen ve yeterince öğretilmemiş bir yönüdür. Konu hakkında önerdiğimiz kitap: _[Data and Reality: A Timeless Perspective on Perceiving and Managing Information in Our Imprecise World.](https://www.amazon.com/Data-Reality-Perspective-Perceiving-Information/dp/1935504215)_

[![Reading in Database Systems](https://teachyourselfcs.com/redbook.jpg)](http://www.redbook.io/) [![Data and Reality: A Timeless Perspective on Perceiving and Managing Information in Our Imprecise World](https://teachyourselfcs.com/data-reality.jpg)](https://www.amazon.com/Data-Reality-Perspective-Perceiving-Information/dp/1935504215)

### Diller ve Derleyiciler

Çoğu programcı dil öğrenirken çoğu bilgisayar bilimcisi diller hakkında bilgi edinir. Bu, bilgisayar bilimcisine, programlama alanında bile programcıya göre belirgin bir avantaj sağlar! Bilgileri genelleşir; yeni bir dilin işleyişini, yalnızca belirli dilleri öğrenmiş olanlardan daha derin ve hızlı bir şekilde anlayabilirler.

Önerdiğimiz tanıtıcı metnimiz Bob Nystrom’un mükemmel _[Crafting Interpreters](https://craftinginterpreters.com/contents.html)_’ı, ayrıca ücretsiz olarak çevrimiçi mevcut. İyi organize edilmiş, oldukça eğlenceli ve birincil amacı sadece dillerini ve dil araçlarını daha iyi anlamak olanlara çok uygun. Metinin tamamı üzerinde çalışmak için zaman ayırmanızı, "zorluklardan" hangisi ilginizi çekiyorsa onu denemenizi öneririz.

Daha geleneksel bir öneri ise _[Compilers: Principles, Techniques & Tools](https://smile.amazon.com/Compilers-Principles-Techniques-Tools-2nd/dp/0321486811)_ daha yaygın adıyla “Dragon Book”. Ne yazık ki, kendi başımıza çalışmak yerine eğitmenlerin dersleri için 1-2 dönemlik konu seçmeleri için tasarlanmıştır.

Dragon Book’u kullanmayı seçerseniz, tercihen bir akıl hocasının yardımıyla konuları özenle seçmeniz önemlidir. Aslında Dragon Book’u kullanmak için önerdiğimiz yol, video dersler için ek bir referans niteliğindedir. Önerdiğimiz ise [Alex Aiken’in edX’teki](https://www.edx.org/course/compilers) video dersleridir.

[![Compilers: Principles, Techniques, and Tools](https://teachyourselfcs.com/dragon.jpg)](https://www.amazon.com/Compilers-Principles-Techniques-Tools-2nd/dp/0321486811) 

> Basmakalıp bir yazılımcı olmayın. Yerine kullanıcılar ve diğer yazılımcılar için araçlar yapın. Tarihi tekstil ve çelik endüstrilerinden örnek alın: makine ve araçlar mı inşa etmek istiyorsun, yoksa o makinelerde iş görmek mi?
>
>— Ras Bodik derleyiciler dersinin başında

### Dağıtık Sistemler

Bilgisayarların sayısı arttıkça yaygınlaştılar. İşletmeler daha önce daha büyük ve daha büyük ana bilgisayarlar satın alırken, artık çok küçük uygulamaların bile birden çok makinede çalışması normaldir. Dağıtık sistemler bunu yaparken dahil olan değiş tokuş hakkında nasıl mantık yürütüleceğinin incelenmesidir.

Kendi kendinize çalışmanız için önerdiğimiz kitap Martin Kleppmann’ın _[Designing Data-Intensive Applications](https://smile.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable-ebook/dp/B06XPJML5D/)_’ıdır. Geleneksel bir ders kitabından çok daha iyi olan DDIA, uygulayıcılar için tasarlanmış ve bir şekilde derinlik veya titizlikten ödün vermekten kaçınan oldukça okunabilir bir kitaptır.

Daha geleneksel bir metin arayanlar ya da çevrimiçi ücretsiz mevcut olanı tercih edenler için Maarten van Steen ve Andrew TanenBaum’un _[Distributed Systems, 3rd Edition](https://www.distributed-systems.net/index.php/books/ds3/)_’ını tavsiye ediyoruz.

Video tercih edenler için Robert Morris tarafından [MIT’s 6.824](https://www.youtube.com/watch?v=cQP8WApzIQQ&list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB) adlı okumalarıyla [bu bağlantıda](https://pdos.csail.mit.edu/6.824/schedule.html) mevcut olan mükemmel bir ders.

Ders kitabı veya diğer ikincil kaynakların seçimi ne olursa olsun, dağıtık sistemlerin incelenmesinde makale okumak kesinlikle zorunludur. [Bu bağlantıda](http://dsrg.pdos.csail.mit.edu/papers/) iyi bir liste mevcut ve yerel [Papers We Love](http://paperswelove.org/) bölümünüze katılmanızı şiddetle tavsiye ederiz.


## Sıklıkla sorulan sorular 

### Bu kılavuzun hedef kitlesi kimdir?

Kendi kendini yetiştiren bir yazılım mühendisi, eğitim kampı mezunu veya erken gelişmiş bir lise öğrencisi veya resmi eğitiminizi kendi kendine çalışma ile tamamlamak isteyen bir üniversite öğrencisi olduğunuzu aklımızda tutuyoruz. Bu yolculuğa ne zaman başlanacağı sorusu tamamen kişisel bir sorudur, ancak çoğu insan bilgisayar bilimi teorisine çok derin dalmadan önce bazı profesyonel deneyimlerden yararlanma eğilimindedir. Örneğin, öğrenciler veri tabanlarıyla zaten profesyonel olarak çalışmışlarsa veri tabanı sistemleri hakkında ya da birkaç web projesi üzerinde çalışmışlarsa bilgisayar ağları hakkında bilgi edinmeyi sevdiklerini fark ettik.

### Peki yapay zeka/grafikler/konu X?

Listemizi, uzmanlık veya endüstriye bakmaksızın, her pratik yazılım mühendisinin bilmesi gerektiğini düşündüğümüz bilgisayar bilimleri konularıyla sınırlamaya çalıştık, ancak sistemlere odaklanarak. Deneyimlerimize göre, bu konular kendi kendini yetiştiren mühendislerin ve eğitim kampı mezunlarının ezici çoğunluğu için en çok geri dönütü olacak ve daha ileri çalışmalar için sağlam bir temel oluşturacak. Daha sonra, çok fazla rehberlik olmadan ders kitaplarını veya makaleleri toplamak ve temel kavramları öğrenmek için çok daha iyi bir konumda olacaksınız. Birkaç ortak “seçmeli” ders için önerdiğimiz başlangıç noktaları:

*   Yapay zeka için: Videoları izleyerek ve mükemmel Pacman projelerini tamamlayarak [Berkeley’s intro to AI course](http://ai.berkeley.edu/)’u tamamlayın. Ders kitabı olarak Russell ve Norvig’in Artificial Intelligence: A Modern Approach’u kullanın.

*   Makine öğrenimi için: Andrew Ng’nin Coursera kursunu tamamlayın. Sabırlı olun ve derin öğrenme gibi çekici yeni denizlere yelken açmadan önce temel ilkeleri anladığınızdan emin olun. 

*   Bilgisayar grafikleri için: [Berkeley’s CS 184](http://inst.eecs.berkeley.edu/~cs184/fa12/onlinelectures.html)’ü çalışın ve [Computer Graphics: Principles and Practice](https://www.amazon.com/Computer-Graphics-Principles-Practice-3rd/dp/0321399528)’i ders kitabı olarak kullanın.
 
### Önerilen sıralama ne kadar katı?

Gerçekçi bir şekilde, tüm bu konular önemli miktarda örtüşür ve döngüsel olarak birbirlerine atıfta bulunurlar. Örneğin, ayrık matematik ve algoritmalar arasındaki ilişkiyi ele alalım: Önce matematiği öğrenmek, algoritmalarınızı daha derinlemesine analiz etmenize ve anlamanıza yardımcı olur, ancak algoritmaları önce öğrenmek, ayrık matematik için daha fazla motivasyon ve bağlam sağlar. En iyi şekilde, kariyeriniz boyunca bu iki konuyu da birçok kez tekrar ziyaret edersiniz.

Önerdiğimiz sıralamamız çoğunlukla başlamanıza yardımcı olmak için… Farklı bir diziyi tercih etmek için zorlayıcı bir nedeniniz varsa, o zaman devam edin. Bize göre en önemli "ön koşullar": işletim sistemleri veya veri tabanlarından önce bilgisayar mimarisi ve dağıtılmış sistemlerden önce ağ ve işletim sistemleridir.

### Open Source Society veya freeCodeCamp müfredatıyla arasındaki fark nedir?

Bu kılavuz ilk 2016 yılında yazıldığında [OSS kılavuzu](https://github.com/open-source-society/computer-science) çok fazla konu içeriyordu, bunların çoğu için yetersiz kaynaklar önerdi ve belirli kursların neden veya hangi yönlerinin değerli olduğuna dair hiçbir mantık veya rehberlik sağlamadı. İhtisasınıza bakmaksızın derslerimizi bir yazılım mühendi olarak gerçekten bilmeniz gerekenlerle sınırlandırmaya ve her dersin neden eklendiğini anlamanıza yardımcı olmak için çabaladık. Sonraki yıllarda OSS rehberi geliştiriIdi ama hala freeCodeCamp’in daha açık ve bağlı bir yol sağladığını düşünüyoruz.

freeCodeCamp bilgisayar bilimine değil çoğunlukla yazılıma odaklıdır. Neden bilgisayar bilimini öğrenmek isteyeceğinizi, [yukarıda](https://teachyourselfcs.com/#why) göz atabilirsiniz. Programlamada yeniyseniz, buna öncelik vermenizi ve bir veya iki yıl içinde bu kılavuza dönmenizi öneririz. 

### Ya X dili?

Belirli bir programlama dilini öğrenmek, bilgisayar biliminin bir alanını öğrenmek için tamamen farklı bir düzlemdedir. Bir dil öğrenmek çok daha kolaydır ve çok daha az değerlidir. Zaten birkaç dil biliyorsanız, kılavuzumuzu takip etmenizi ve boşluklara dil edinimini uygun hale getirmenizi veya daha sonra bırakmanızı şiddetle öneririz. Programlamayı iyi öğrendiyseniz (örneğin Bilgisayar Programlarının Yapısı ve Yorumlanması yoluyla) ve özellikle derleyicileri öğrendiyseniz, yeni bir dilin temellerini öğrenmeniz bir hafta sonundan biraz daha uzun sürmeli, ardından işteki kütüphaneler/araçlar/ekosistem hakkında bilgi edinebilirsiniz.

### Güncel ve revaçta olan teknoloji X ne olacak?

Tek bir teknoloji, onu kullanmayı öğrenmenin eğitiminizin temel bir parçası olması gerekecek kadar önemli değildir. Öte yandan, o şeyi öğreneceğiniz için heyecanlı olmanız harika. İşin püf noktası, belirli teknolojiden temel alan veya konsepte doğru geriye doğru çalışmak ve modaya uygun teknolojinizin daha büyük resme nasıl uyduğunu görmeden önce bunu derinlemesine öğrenmektir. 

### Neden hala SICP'yi öneriyorsunuz?

Bak, sadece dene. Bazıları SICP’nin insanın aklını başından aldığını ve çok az kitabın paylaştığı bir özellik olduğunu söylüyor. Beğenmezseniz, her zaman başka bir şey deneyebilir ve belki daha sonra SICP'ye dönebilirsiniz.

### Neden hala “Dragon kitabını” öneriyorsunuz?

Dragon kitabı hala derleyiciler için en eksiksiz tek kaynaktır. Ayrıştırma (parsing) gibi günümüzde ayrıntılı olarak kapsamanın revaçta olmadığı bazı konuların üzerinde genellikle çok durduğu için adı kötüye çıkıyor. Mesele şu ki, kitap baştan başa çalışılması asla istenmedi, sadece eğitmenin bir ders oluşturabilmesi için yeterli kaynak sağlamaktı. Benzer olarak kendi kendine öğrenen biri kitapta kendi macerasını seçebilir ya da daha iyisi herkese açık derslerin öğretmenlerinin ders taslaklarındaki önerilerini takip edebilir.


### Ders kitaplarını ucuza nasıl edinebilirim?

Yazarlarının cömertliği sayesinde önerdiğimiz ders kitaplarının çoğu çevrimiçi olarak ücretsiz olarak mevcuttur. Olmayanlar için, eski sürümlerin kullanılmış kopyalarını satın almanızı öneririz. Genel bir kural olarak, bir ders kitabının birkaç basımı varsa, eski bir baskının tamamen yeterli olması oldukça muhtemeldir. Fiyat farkı 10 kat olsa bile, en yeni sürümün eski sürümden 10 kat daha iyi olma ihtimali kesinlikle düşüktür!

### Bunu kim hazırladı?

Bu kılavuz, [Oz Nova](https://twitter.com/oznova_) ve [Myles Byrne](https://twitter.com/quackingduck) tarafından 2020 güncellemeleri ile yazılmıştır. San Francisco'daki küçük grup ortamlarında ve çevrimiçi canlı olarak 1000'den fazla kendi kendini yetiştirmiş mühendis ve eğitim kampı mezunu kişilere temel bilgisayar bilimlerini öğretme deneyimimize dayanmaktadır. Kendi kendine öğretme kaynakları hakkındaki sürekli geri bildirimleriniz için tüm öğrencilerimize teşekkür ederiz.
Yeterli zaman ve motivasyon verildiğinde yukarıdaki her şeyi kendinize öğretebileceğinizden çok eminiz. Ancak yoğun, yapılandırılmış, eğitmen tarafından yönetilen bir programı tercih ediyorsanız, [Computer Science Intensive](https://bradfieldcs.com/csi/) programımızla ilgilenebilirsiniz. Yüksek lisans derecesi almanızı [önermiyoruz](https://ozwrites.com/masters/).

### Bunu kim çevirdi?

Herkese selam, ben Tolga Barış Pınar. IEU (İzmir Ekonomi Üniversitesi) tercümanlık mezunuyum. Birkaç Coursera kursu ve harcadığım saatler dışında yazılım geçmişim yok. Hatta bugüne kadar bu çeviriyi GitHub'a yüklemeyi bilmiyordum. Ancak yazılım hakkında gelecekte planlarım var. Bu metinle karşılaşmam ve çevirmeme de vesile olan neden buydu. Dil bariyerinin ne kadar büyük bir sorun olduğunu bildiğim için bu kapsamlı rehberin ihtiyacı olan herkese ulaşmasını sağlamakta bir adım atmak istedim. Umarım bunu her kim okuyorsa yardımcı olabilmişimdir.

Öneri, düzeltme veya herhangi bir neden için bana ulaşmaktan çekinmeyin. 

Sağlıklı günler!
 
