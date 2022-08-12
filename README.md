### First Responsive Homepage web design.

- [Creator](#Creator)
- [Important Code Notes](#Important-Code-Notes)
- [What I learned](#what-i-learned)
- [Continued development](#Topics-I'm-missing-and-want-to-improve-myself)
- [Useful resources](#Resources-that-helped-me-with-this-project)

## Creator

- Website - [Publish Site This Project](https://alperennucr.github.io/Responsive-HomePage-website/)
- Frontend Mentor - [@alperennucr](https://www.frontendmentor.io/profile/alperennucr)
- Github - [@alperennucr](https://github.com/alperennucr)
- LinkedIn - [Alperen Uçar](https://www.linkedin.com/in/alperen-u%C3%A7ar-a26434247/)


### Important Code Notes

```html

<h1>Some HTML code I'm proud of</h1>

```

```css

.proud-of-this-css {
  color: papayawhip;
}

```

### What I learned 

Turkish Explain
-----------------
NOT1: Margin ve Paddingleri - biçiminde kulllanma, bu sağlıksız bir yöntem olur. Bunun yerine mesela sağdan
 ve soldan padding gibi bir yöntem uygulayabilirsin. Bunun örneğini style.scss de 277-278. satırlarda
(satır sayısı değişmezse) bulabiliriz.

NOT2: Mobile Responsive yaparken font büyüklüklerini büyük tutmamaya dikkat et. Bilgisayarda tasarladığın 
çin sen anlamayabilirsin ama fontlar telefonda daha büyük durabilir.

NOT3: Bir div'i sol tarafa yollamak için yaklaşık 3-4 saatimi harcadım. Garipsediğim bir şekilde flex-direction' u
col olan bir div' i align item flex-start yaptığımda sola gitmek yerine ortada kalıyor,align items ile ne yaparsam yapayım işe
yaramıyordu. Daha sonra div' in 100% lük bir alan kapladığı için ortada kalıp hareket etmediğini düşündüğüm için div'in boyutunu
kendi boyutuna(max-width:76px; width:100%;) getirdim. Bunu yaptığımda ortada durma sorunu yok oldu ve kendisini solda
serbest bıraktı. Ama garip bir şekilde hala align items çalışmıyordu, şöyle düşünüyorum bunun sebebi, div'in boyutunu kendi boyutuna
getirdiğim için kendi içinde hareket edememesiydi. Bende sorunu farklı bir şekilde çözdüm, bu div ve onun altında bulunan div'i
kaplayan section kapsayıcı div'ine max-width:767(mobilde tüm genişlik); ardından width:93%; yaparak onu istediğim şekilde
sağa kaydırmış oldum ve bu div'in kopyalarıyla bir farkı kalmadı.---- Evet bu yazıyı yazarken kurcalayacağım yerleri kavradığımı
hissettim ve sorunu çözdüm yani artık ortada bilinmezlik yok. align-items'ı çalışmayan divlerin içinde iki adet element vardı
bende ya elementler tüm alanı kaplıyorsa dedim ve hayır kaplamıyordu. Sonradan farkettim ki elementlerin altına margin: 0 auto; koymuşum
ve bu da onları daima center'da yapıyor ve böylece align items'ı da işlevsiz kılıyor. Sorunun bu projede hangi kısımda yaşandığını
söyleyeyim. section-news div'inin içindeki section-top kısmını sola yatırmaya çalışırken bu hatayla karşılaştım.

NOT4: Hataları ayıklarken bir yerde takıldığında kendine sorular sormaya başla. Belli bir süre sonra o
sorular sana farkındalık kazandıracaktır.

NOT5: Bazen height verilmiş divler azıcık da olsa üst üste biner(height yükseltme yapabilirsin). Genelde bu
üst üste binmenin sebebi(yaşadığım kadarıyla) divlere verilen height değerlerinin onlara yetmemesi ve dışarı taşması,
 bu yüzden
de diğer divin üstüne taşıyor. Araya ekstra height verip daha kötü yapmak yerine div'in height sorununu çöz.Bu sorunu 
proje içerisinde tekrardan yaşadım ve sorunu biraz daha bariz bir şekilde görebildim, örneklendireyim.Bir x divi var, 
birde x divinin içerisinde duran y divi var. İkisinede height veriyoruz ama eğer biz içteki y divinin height' ını onun 
kapsayıcısı olan x div'inin height' ından daha fazla yaparsak, bu içteki div'in dışarıya taşmasına neden olur ve engellenmesi
 için dıştaki x div'inin height'ının içteki y divinin height' ından büyük olması gereklidir.

NOT6: Responsive sass dosyasını sağda ana style sass doyasını da sağda tutarak kontrol ettiğimde
daha az karışıklık oluyor.

NOT7: Bu projede toparlamaya çalıştım ama bidahaki projelerde uygulaycağım: Respon
sive design yaparken kodları kopyalayıp bir de responsive de aynılarını tutarsan 
od kalabalığı olur. Kendi kodunu kopyalama, bakarak değişecekleri
değiştir. 

ÖNEMLİ BİLGİ: Responsive yazarken media sırası büyükten küçüğe doğru gidiyor.

SORU: Responsive Design' da breakpointler neden birbirini ezer ?
CEVAP: Aslında birbirlerini ezmezler, eğer dikkatli bakarsanız breakpointler arasında ufak bir öncelik sırası
olduğunu görürsünüz. Ekran boyutuna kendini en çok hangi breakpoint'e kabul ettirmiş ise o breakpoint geçerli olur.

AŞIRI ÖNEMLİ NOT: CSS' de yukarıdaki kod en az önemli olan, aşağıdaki kod ise en önemli olan kod'dur. Yani aynı değişkene farklı değerler verdiğimizi düşünürsek en aşağıdaki kod geçerli olacaktır. Responsive design yaparken ekran genişliğimi 1200 baz aldım ve (min-width:1100) olarak en yüksek genişliğe sahip filtrem de bu idi. Ben de bu aralığa((min-width:1100)) bazı kodlar yazdım ve kodlar işlemiyordu. Sebebi bu media etiketinin birkaç satır aşağısında (min-width:500px) aralığında bir kod olmasıydı. Genişliği 1100px olan media etiketimin kodlarını alarak 500px aralıklı media etiketi kodlarımın altına yazdım ve sorunu çözdüm. 

### Topics I'm missing and want to improve myself

More practice and javascript.

### Resources that helped me with this project

- [Reset CSS](https://meyerweb.com/eric/tools/css/reset/) - Reset CSS code resources.

- [Chrome Dev Tools](https://developer.chrome.com/docs/devtools/css/overrides/)
Stiller bölmesinde CSS'nizi görebiliyorsanız, ancak CSS'nizin üzeri çizilmişse,
bu, CSS'nizi geçersiz kılan başka bir CSS olduğu anlamına gelir. CSS terminolojisinde
bu kavram Specificity(Özgüllük) olarak adlandırılır. Chrome Geliştirici Araçları, yeni CSS'nizin uygulanmamasına
neden olan eski CSS'yi bulmanıza yardımcı olabilir.
