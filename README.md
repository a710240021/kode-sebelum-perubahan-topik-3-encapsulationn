class Mobil:
    def __init__(self, merk, model, tahun_produksi, warna, nomor_polisi, kecepatan_maksimum, bahan_bakar, jumlah_penumpang):
        self.merk = merk
        self.model = model
        self.tahun_produksi = tahun_produksi
        self.warna = warna
        self.nomor_polisi = nomor_polisi
        self.kecepatan_maksimum = kecepatan_maksimum
        self.bahan_bakar = bahan_bakar
        self.jumlah_penumpang = jumlah_penumpang
        self.posisi_gigi = 0
        self.status_mesin = False
        self.kecepatan_sekarang = 0

    def start_engine(self):
        self.status_mesin = True
        print("Mesin dinyalakan.")

    def stop_engine(self):
        self.status_mesin = False
        self.kecepatan_sekarang = 0
        self.posisi_gigi = 0
        print("Mesin dimatikan.")

    def info_mobil(self):
        print(f"Nomor Polisi: {self.nomor_polisi}")
        print(f"Posisi Gigi : {self.posisi_gigi}")
