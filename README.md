## Git Nedir ?

Git, bir **versiyon kontrol sistemi (Version Control System)**dir. Yani, projelerdeki dosya ve kod değişikliklerini takip eden bir araçtır. Hem bireysel hem de ekip çalışmaları için tasarlanmıştır. Yazılım geliştirme dünyasında yaygın olarak kullanılır, çünkü projeler üzerinde yapılan değişiklikleri düzenli ve güvenli bir şekilde kaydetmeye yardımcı olur.


---

### Git Neden Çıktı?

Git, özellikle büyük projelerde birden fazla kişinin aynı dosyada çalıştığı durumlarda ortaya çıkan sorunları çözmek için geliştirilmiştir. Linus Torvalds tarafından, Linux çekirdeği üzerinde çalışan yüzlerce geliştiricinin daha verimli işbirliği yapabilmesi için oluşturulmuştur.

---

### Git Olmadan Önce Ne Yapıyorduk?

Git öncesi insanlar versiyon kontrolünü genelde elle yapıyordu. Örneğin:

1. **Farklı Dosya İsimleriyle Saklama**:

- `proje_v1.txt`, `proje_v2_final.txt`, `proje_son_bu_ciddi_final.txt`

- Bu yöntem kaotikti ve hangi dosyanın en güncel olduğunu anlamak zordu.

2. **Manuel Yedekleme**:
- Eski dosyaları başka bir yere kopyalayıp yeni değişikliklerle çalışılıyordu.
- Bu yöntem hem zaman alıcı hem de hataya açıktı.

3. **Ekip Çalışması Sorunları**:

- Aynı dosya üzerinde birden fazla kişi çalıştığında, dosya çakışmaları sık sık yaşanıyordu.

Git, bu sorunları çözerek otomatik takip, hataları geri alma ve birleştirme gibi özelliklerle yazılım geliştirme sürecini daha verimli hale getirdi.

--- 

### Git'in Temel Kavramları

1. **Repository (Depo)**:

    - Proje dosyalarının tutulduğu ve değişikliklerin takip edildiği yer.

2. **Working Directory (Çalışma Dizini)**:

    - Depodaki dosyaların bilgisayarındaki mevcut kopyası.

3. **Staging Area (Sahneleme Alanı)**:

    - Commit işleminden önce değişiklikleri hazırladığın alan.

4. **Commit**:

    - Değişikliklerin kaydedildiği bir nokta.
5. **Remote Repository (Uzak Depo)**:

    - GitHub, GitLab gibi platformlarda tutulan ve diğer kullanıcılarla paylaşılan depo.


--- 

### En Çok Kullanılan Git Komutları

1. **Depo Oluşturma ve Başlatma**
  
    - Yeni bir Git deposu oluşturmak için:
    `` git init ``

2. **Dosyaları Takip Etme ve Sahneleme** 
    - Tüm dosyaları sahneye eklemek için:
    `` git add . ``

    - Belirli bir dosyayı sahneye eklemek için:
    `` git add dosya_adi.txt  ``

3.  **Değişiklikleri Kaydetme (Commit)**
    - Commit yapmak için:
    `` git commit -m "Değişiklik açıklaması" ``

4. **Bir uzak depoyu (örneğin GitHub) bağlamak için**:

    - Bir uzak depoyu (örneğin GitHub) bağlamak için:
    `` git remote add origin <URL>  `` 

5. **Dosyaları Uzak Depoya Gönderme**
    - Değişiklikleri uzak depoya göndermek için:
    `` git push -u origin main ``

6. **Uzak Depodaki Değişiklikleri Alma**
    - Değişiklikleri uzak depodan almak için:
    `` git pull origin main  ``

7. **Depo Durumunu Kontrol Etme** 
    - Hangi dosyaların değiştiğini veya eklenmeyi beklediğini görmek için:
    `` git status ``
8. **Geçmiş Commitleri Görüntüleme**
    - Commit geçmişini görmek için:
    ``git log  ``

9. **Dal (Branch) Yönetimi**
    - Yeni bir dal oluşturmak için:
    `` git branch yeni_dal  ``
    - Oluşturulan dala geçiş yapmak için:
    `` git checkout yeni_dal ``
    - Dalları birleştirmek için:
    `` git merge yeni_dal ``

10. **Değişiklikleri Karşılaştırma**
    - Son değişiklikleri görmek için:
    `` git diff ``

### Git Kullanımı Örnek Akış

1. Yeni bir proje başlat:
    
    `` git init ``    
2. Dosya ekle ve sahnele:
  `` git add .  `` 
3. Commit yap:
 `` git commit -m "Projenin ilk sürümü"  ``
4. GitHub deposunu bağla:
  `` git remote add origin <depo URL>  ``
5. Dosyaları gönder:
 ``git push -u origin main  ``

 #### Özet

 - **Git Nedir?** Projelerde yapılan değişiklikleri takip eden bir araç.
- **Neden Var?** Dosya çakışmalarını önlemek, geri alma kolaylığı sağlamak ve ekip çalışmalarını düzenlemek için.
- **Git Olmadan Önce?** Manuel yedekleme ve karmaşık dosya isimlendirme kullanılıyordu.
- **Temel Komutlar?** `init`, `add`, `commit`, `push`, `pull`, `status`, `log`.
