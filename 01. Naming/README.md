## İsimlendirme I

    There are only two hard things in Computer Science: cache invalidation and naming things.

    Bilgisayar Bilimlerinde sadece iki tane zor şey vardır: ön belleği temizleme ve şeyleri isimlendirme.

    Phill Karlton


    İsimlendirme yapılırken ingilizce kelimeler kullanılarak isimlendirme yapılmasına dikkat edilmelidir.

- ### Kabul Edilen Kısaltmalar
        Verilen kısaltma anlaşılır olmalıdır. O anki ruh halimize göre aklımıza gelen kısaltma doğru bir kısaltma değildir.

    #### Örnek:
    
    ~~~C++
        // Hatalı kısaltma:
        private int nofInst;

        // Evrensel kısaltmalar:
        #define http
        #define Tcp
        #define Pi

        // Method isimleri:
        init();

        // For döngüleri:
        int i, j, k;

        // Anlamı hemen beliren özellikler:
        int in, out, r;
    ~~~

        Bilindik olmayan kısaltmalardan kaçının. Bu durumda uzun yazmak daha iyidir.

- ### Kısa - Uzun İsim
    - #### Kötü örnekler:
        ~~~C++
            int amnt;
            int tmpAmnt;
            
            Product pr;
            
            File file;
        ~~~
    
    - #### İyi örnekler:
        ~~~C++
            int temporaryAmount;
            
            Product productToBeDeleted;
            Product productToShipToSecondaryAddress;
            
            File fileToReadFromClientToConfigureServer;
        ~~~

- ### Soyut, Kapsayıcı İsim

    - #### Kötü örnekler:
        ~~~C++
            int km
            
            int hour
            
            int calculateKm(City c1, City c2)
        ~~~

    - #### İyi isimlendirme:
        ~~~C++
            int distance
            int distanceToGo
            
            int timeToCook
            int reamingDistance
            
            int calculateDistanceBetween(City from, City to)
        ~~~

---

## İsimlendirme II

    Ne yapıyorsanız ona isim verin, isimlendirdiğinizi yapın.

~~~Dart
    List<RegisteredEmail> findPrimaryUserListByUid(String uid);

    List<User> findPrimaryUserListByUid(String uid);
~~~

