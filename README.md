# Nesne-Tabanl-Programlama
class Uygulama():
    def __init__(self,Adı,SoyAdı,ZamMiktarı,Maaş,OyuncuÜcreti):
        self.Adı = Adı
        self.SoyAdı = SoyAdı
        self.ZamMiktarı = ZamMiktarı
        self.Maaş = Maaş
        self.OyuncuÜcreti = OyuncuÜcreti

    def BilgileriGoster(self):
        print(""""
        Adı: {}
        SoyAdı:{}
        Zam Miktarı: {}
        Maaş:{}
        Oyuncu Ücreti: {}
        """.format(self.Adı,self.SoyAdı,self.ZamMiktarı,self.Maaş,self.OyuncuÜcreti))

    def MaaşAttır(self,Maaş_Artar):
        print("Maaş Arttırılıyor")
        self.Maaş += Maaş_Artar

    def MaaşZam(self,Zam):
        print("Zam Yapılıyor")
        self.Maaş *= 2

    def OyuncuÜcretiHesaplama(self,Oyuncu_Ücret):
        self.OyuncuÜcreti *= Oyuncu_Ücret
        print("\tAlex'in Toplam Ücreti:",Oyuncu_Ücret)


yazılımcı = Uygulama("Rıdvan Can","GİZLİ",2000,3000,10000)
yazılımcı.BilgileriGoster()
yazılımcı.OyuncuÜcretiHesaplama(20000)

