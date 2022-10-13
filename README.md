print("""
                        Dönüştürücü

     Bayt ı diğer birimlere çevirmek istiyorsanız "1" tuşuna basın  
     KiloBayt ı diğer birimlere çevirmek istiyorsanız "2" tuşuna basın
     MegaBayt ı diğer birimlere çevirmek istiyorsanız "3" tuşuna basın
     GigaBayt ı diğer birimlere çevirmek istiyorsanız "4" tuşuna basın  
                   
""")    #kullanıcı bilgilendiriliyor
 

islem = str(input("İşlem seçin:"))
if islem == "1":
    a = int(input("Çevirmek istediğiniz sayıyı girin:"))
#kullanıcı bayt ı çevirmeyi istemiş
    print("Kilobayt karşılığı:" , a/1024)
    print("Megaobayt karşılığı:" , a/1024*1024)
    print("Gigabayt karşılığı:" , a/1024^3)

elif islem == "2":
    a = int(input("Çevirmek istediğiniz sayıyı girin:"))
#kullanıcı kilobaytı çevirmeyi istemiş
    print("Bayt karşılığı:" , a*1024)
    print("Megabayt karşılığı:" , a/1024)
    print("Gigabayt karşılığı:" , a/1024^2)
   

elif islem == "3":
    a = int(input("Çevirmek istediğiniz sayıyı girin:"))
#kullanıcı megabaytı çevirmeyi istemiş
    print("Bayt karşılığı:" , a*1024^2)
    print("Kilobayt karşılığı:" , a*1024)
    print("Gigabayt karşılığı:" , a/1024)
  

elif islem == "4":
#kullanıcı gigabaytı çevirmeyi istemiş
    a = int(input("Çevirmek istediğiniz sayıyı girin:"))

    print("Bayt karşılığı:" , a*1024^3)
    print("Kilobayt karşılığı:" , a*1024^2)
    print("Megabayt karşılığı:" , a*1024)


else: 
     print("Geçerli işlem girin....")
