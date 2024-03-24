1. Model Oluşturma: Model klasörü yaratak bu klasör altında Book adında bir model oluşturun. Bu model Id, Title (Başlık), Author (Yazar), ve Year (Yayın Yılı) özelliklerine sahip olmalı.

2. Bu modeli kullanarak aşağıdaki kitapları içeren bir kitap listesi oluştur bu liste uygulamanın başlangıcında oluşturulmalıdır.
    Title = "Sefiller", Author = "Victor Hugo", Year = 1862
    Title = "1984", Author = "George Orwell", Year = 1949
    Title = "Suç ve Ceza", Author = "Fyodor Dostoyevsky", Year = 1866 


3. Bu kitap listesini kullanarak aşağıdaki işlemleri yapabilen bir API oluşturun.
	a. Tüm kitapları listele
	İp ucu: GET request to /books tüm kitapları döndürmeli. (Results.Ok ile döndürülmeli)


	b. Id'si verilen kitabı getir
	İp ucu: GET request to /books/{id} id'si verilen kitabı döndürmeli. (Bulduğunda Results.Ok ile döndürmeli bulamadığında Results.NotFound döndürmeli)

	c. Yeni kitap ekle
	İp ucu: POST request to /books yeni kitabı eklemeli ve eklenen kitabı döndürmeli. (Results.Ok ile döndürmeli) Yeni kitap bilgilerini "Book book" şeklinde almayacak ve 	Title, Author, Year bilgilerini methodun imzasında ayrı ayrı belirterek post parametreleri olarak almalı. Bkz: Postman Post Body form-data https://ctrl.vi/i/s4WLafeU5
Id bilgisi dişaridan verilmeli mevcut books listesindeki en büyük id ye +1 yapılarak elde edilmeli (linq kullanılmalı)

	d. Id'si verilen kitabı sil
	İp Ucu: DELETE request to /books/{id} id'si verilen kitabı silmeli. (Results.Ok string "Ok" döndürmeli bulamadığında Results.NotFound döndürmeli)




	https://drive.google.com/file/d/1JpUIvjcyNEZl1l3aer1nYyljcUg-440b/view?usp=sharing
