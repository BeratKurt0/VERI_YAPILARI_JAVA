# Java'da veri tipleri

->Veri, bilgisayarın işleyebileceği bilgilere denir

->veriler bilgisayarda *input(girdi)* veya *çıktı(output)* konumunda olabilirler

->Veri, özellik olarak üçe ayrılır:

** ilkel(primitive) veri tipleri

** Referans tipleri

** Null veri tipi (referans türlerine dahil.)

# primitive:

** en temel veri tipidir ve diğer karmaşık veri tiplerinin tanımında kullanılırlar

** primitive veri tipleri toplam 8 tanedir:

int     - 32 bit    - *java.lang.Integer*

byte    - 8  bit    - *java.lang.Byte* 

short   - 16 bit    - *java.lang.Short*

long    - 64 bit    - *java.lang.Long*

float   - 32 bit    - *java.lang.Float*

double  - 64 bit    - *java.lang.Double*

boolean - 1  bit    - *java.lang.Boolean*

char    - 16 bit    - *java.lang.Character*

** yukarda ilkel veritiplerinin anahtar kelimesi, bellekte kapladığı alan ve gömülü olduğu sınıf gösterilmiştir.

** ilkel verilerle (byte,long,short,int) tamsayı, (float,double) ondalıklı sayılar, (boolean) mantıksal ifadeler ve 
(char)Unicode standartlarına göre karakterler bellekte tutulabilir.

** yukarıdaki bilgilerden farlklı olarak "void" ve "null" durumlarını da konuşmak gerek.

void(); --> metotlarda kullanılır ve *statement* işlev görür. Amacı yanlızca değer döndürmeden komutları
yürütmektir.

null --> *java.lang.Object* sınıfının bir değişkendir. Tüm referans tipleri ilk tanımlandığında "null" öndeğerlidir.
bir referansın nesneye işaret etmediğini anlamamızı sağlar. Bir referans nesneye işaret etmezse "null" değeri döndürür.

- expr(expression): değer döndüren işlemlere/ifadelere denir.
- stmt(statement): değer döndürmeyen ifadelere/işlemlere denir.

# Değişkenler:

değişkenler,verilerin konulduğu bellek hücrelerine işaret eden *işaretçilere(referanslara)* denir.

--> Java' da referans edilişlerine göre değişkenler 4 gruba ayrılır:

- static değişkenler (sınıfa özgü değişkenler): 

önüne *static* eki alırlar. Değişken sınıfa özgü bulunur ve o anki değerini nesne oluşturmaya
gerek kalmadan görebiliriz. 

Static değişken bellekte bir defa oluşturulur ve her nesne ortak olarak kullanır.

sınıf içindeki her kod ulaşılabilir.

- dinamik değişkenler (nesneye özgü değişkenler):

önüne ek getirilmeyen değişkenlere denir. Sınıftan oluşturulan her nesne için, dinamik değişken;
nesneye özgü olarak değer alır. 

ancak ait olduğu nesne içerisindeki kodlar ulaşabilir. Nesne bellekten silinirse anlık değişken
de yok olur.

- Yerel(Local) Değişkenler:

bildirimi bir blok içinde yapılan değişkenlere denir. Değişken yanlızca ait olduğu blok içinde geçerli olur.

yerel değişkenin kapsama alanı sadece ait olduğu bloktur.

- private değişkenler:

bir sınıf içinde, sadece kendi sınıfının erişebildiği, nesnelerin dahi erişemediği değişkenlere denir.

erişim için getter setter metodları kullanılır.

- Parametreler (Argümanlar):

bir metod oluştururken metodun aldığı girdi değişkenlerine denir.

Argüman içeren bir metod, argüman almadan çağrılamaz. (şayet overloading yapılmamışsa..)

- Sınıf Öğeleri(Class Members):

erişim belirtkenleri değişken ve metodlar için aynen geçerlidir. Bir sınıf içinde static
bir değişken veya metod varsa bunlar sınıfa özgüdür ve *'class members'* olarak adlandırılırlar. 

# Erişim Belirtkenleri (Access Modifiers):

arayüz, soyutlama, program oluşturmak için değişken ve metodların görünür olup olmadığı aralığı belirlemek
çok önemlidir. Özellikle derslerde Java veri yapıları arayüzü ve metodları işleneceği için bu konuyu bilmek
veri yapılarını öğrenme açısından çok önem kazanır.

![Resim](https://miro.medium.com/v2/resize:fit:720/format:webp/1*htCp0d5RelHdaekk1l6CUg.png)


# Java Sürümleri:

Java'nın piyasaya sunuluşu üç düzeye ayrılır:

- Java SE (Standart Edition)

-> java başlangıç düzeyi olarak adlandırabiliriz. Basit projeler ve java dilini öğrenmek için idealdir.
Ücretsizdir.

- Java EE (Enterprise Edtion)

-> ileri düzey projeler için kullanılır ve lisansa taabi tutulur.

- Java ME (Micro Edition)

-> mobil oyunlar için kullanılır.

şimdi anlattıklarımızın en baştan en sona java ile ilgili kaynak kodlarını yazıyor olacağım.  paket000'a Bknz.


# Author: Berat Kurt







