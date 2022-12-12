
#oylamali oyun
import time
import random
oda = ["a", "b", "c", "d", "e", "f", "g", "h"]
sayiBelirle = int(input("kisi sayisini secin: "))
if sayiBelirle < 4:
    print("[☻]  Boyle oyun mu olur kardesim :)")
elif sayiBelirle < 5:
    oda.pop(4)
    oda.pop(4)
    oda.pop(4)
    oda.pop(4)
    print("[+]  4 kisilik olda olusturuldu")
elif sayiBelirle < 6:
    oda.pop(4)
    oda.pop(4)
    oda.pop(4)
    print("[+]  5 kisilik olda olusturuldu")
elif sayiBelirle < 7:
    oda.pop(4)
    oda.pop(4)
    print("[+]  6 kisilik olda olusturuldu")
elif sayiBelirle < 8:
    oda.pop(4)
    print("[+]  7 kisilik olda olusturuldu")
elif sayiBelirle < 9:
    print("[+]  8 kisilik olda olusturuldu")
elif sayiBelirle > 8:
    print("[-]  O kadar buyuk oda kuramazsin!")
    
if sayiBelirle == 4:
    a = input("1.oyuncu adini giriniz: ")
    oda[0] = a
    b = input("2.oyuncu adini giriniz: ")
    oda[1] = b
    c = input("3.oyuncu adini giriniz: ")
    oda[2] = c
    d = input("4.oyuncu adini giriniz: ")
    oda[3] = d
    print("Oyuncular hazir miyizz!! ", oda)
    sozluk = {oda[0]:0, oda[1]:0, oda[2]:0, oda[3]:0}
    time.sleep(1)
    print("[+]  Oyun basliyoorr...")
    time.sleep(1)
    print("Hosgeldiniz, sirayla oy veriniz...")
    t  = True
    t2 = True
    t3 = True
    t4 = True
    t5 = True
    t6 = True
    t7 = True
    t9 = True
    tg = True
    while tg:
        while t:
            print("sira sizde: ", oda[0].upper(), f"""seciminizi yapiniz;
                  1- {oda[1]}
                  2- {oda[2]}
                  3- {oda[3]}
                  
                  """)
            secim = input("1'mi, 2'mi, 3'mu ")
            if secim == "1":
                sozluk[oda[1]] += 1
                print(sozluk.items())
                t = not t
            elif secim == "2":
                sozluk[oda[2]] += 1
                print(sozluk.items())
                t = not t
            elif secim == "3":
                sozluk[oda[3]] += 1
                print(sozluk.items())
                t = not t
        time.sleep(1)
        while t2:
            print("sira sizde: ", oda[1].upper(), f"""seciminizi yapiniz;
                  1- {oda[0]}
                  2- {oda[2]}
                  3- {oda[3]}
                  
                  """)
            secim = input("1'mi, 2'mi, 3'mu ")
            if secim == "1":
                sozluk[oda[0]] += 1
                print(sozluk.items())
                t2 = not t2
            elif secim == "2":
                sozluk[oda[2]] += 1
                print(sozluk.items())
                t2 = not t2
            elif secim == "3":
                sozluk[oda[3]] += 1
                print(sozluk.items())
                t2 = not t2
        time.sleep(1)
        while t3:
            print("sira sizde: ", oda[2].upper(), f"""seciminizi yapiniz;
                  1- {oda[0]}
                  2- {oda[1]}
                  3- {oda[3]}
                  
                  """)
            secim = input("1'mi, 2'mi, 3'mu ")
            if secim == "1":
                sozluk[oda[0]] += 1
                print(sozluk.items())
                t3 = not t3
            elif secim == "2":
                sozluk[oda[1]] += 1
                print(sozluk.items())
                t3 = not t3
            elif secim == "3":
                sozluk[oda[3]] += 1
                print(sozluk.items())
                t3 = not t3
        time.sleep(1)
        while t4:
            print("sira sizde: ", oda[3].upper(), f"""seciminizi yapiniz;
                  1- {oda[0]}
                  2- {oda[2]}
                  3- {oda[3]}
                  
                  """)
            secim = input("1'mi, 2'mi, 3'mu ")
            if secim == "1":
                sozluk[oda[0]] += 1
                print(sozluk.items())
                t4 = not t4
            elif secim == "2":
                sozluk[oda[2]] += 1
                print(sozluk.items())
                t4 = not t4
            elif secim == "3":
                sozluk[oda[1]] += 1
                print(sozluk.items())
                t4 = not t4
        time.sleep(1)
        print("deneme yazisi")
        if sozluk[oda[0]] > sozluk[oda[1]] and sozluk[oda[0]] > sozluk[oda[2]] and sozluk[oda[0]] > sozluk[oda[3]]:
            print("en yuksek oy alan: ", oda[0], "elendiniz")
            sozluk[oda[0]] = "!-ELENDI-!"
            print(sozluk.items())
            t2 = True
elif sayiBelirle == 5:
    a = input("1.oyuncu adini giriniz: ")
    oda[0] = a
    b = input("2.oyuncu adini giriniz: ")
    oda[1] = b
    c = input("3.oyuncu adini giriniz: ")
    oda[2] = c
    d = input("4.oyuncu adini giriniz: ")
    oda[3] = d
    e = input("5.oyuncu adini giriniz: ")
    oda[4] = e
    print("Oyuncular hazir miyizz!! ", oda)
    sozluk = {oda[0]:0, oda[1]:0, oda[2]:0, oda[3]:0, oda[4]:0}
elif sayiBelirle == 6:
    a = input("1.oyuncu adini giriniz: ")
    oda[0] = a
    b = input("2.oyuncu adini giriniz: ")
    oda[1] = b
    c = input("3.oyuncu adini giriniz: ")
    oda[2] = c
    d = input("4.oyuncu adini giriniz: ")
    oda[3] = d
    e = input("5.oyuncu adini giriniz: ")
    oda[4] = e
    f = input("6.oyuncu adini giriniz: ")
    oda[5] = f
    print("Oyuncular hazir miyizz!! ",  oda)
    sozluk = {oda[0]:0, oda[1]:0, oda[2]:0, oda[3]:0, oda[4]:0, oda[5]:0}
elif sayiBelirle == 7:
    a = input("1.oyuncu adini giriniz: ")
    oda[0] = a
    b = input("2.oyuncu adini giriniz: ")
    oda[1] = b
    c = input("3.oyuncu adini giriniz: ")
    oda[2] = c
    d = input("4.oyuncu adini giriniz: ")
    oda[3] = d
    e = input("5.oyuncu adini giriniz: ")
    oda[4] = e
    f = input("6.oyuncu adini giriniz: ")
    oda[5] = f
    g = input("7.oyuncu adini giriniz: ")
    oda[6] = g
    print("Oyuncular hazir miyizz!! ", oda)
    sozluk = {oda[0]:0, oda[1]:0, oda[2]:0, oda[3]:0, oda[4]:0, oda[5]:0, oda[6]:0}
elif sayiBelirle == 8:
    a = input("1.oyuncu adini giriniz: ")
    oda[0] = a
    b = input("2.oyuncu adini giriniz: ")
    oda[1] = b
    c = input("3.oyuncu adini giriniz: ")
    oda[2] = c
    d = input("4.oyuncu adini giriniz: ")
    oda[3] = d
    e = input("5.oyuncu adini giriniz: ")
    oda[4] = e
    f = input("6.oyuncu adini giriniz: ")
    oda[5] = f
    g = input("7.oyuncu adini giriniz: ")
    oda[6] = g
    h = input("8.oyuncu adini giriniz: ")
    oda[7] = h
    print("Oyuncular hazir miyizz!! ", oda)
    sozluk = {oda[0]:0, oda[1]:0, oda[2]:0, oda[3]:0, oda[4]:0, oda[5]:0, oda[6]:0, oda[7]:0}




#%%





























































































