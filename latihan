# latihan membuat toko
# menu : cek produk, cek ketersediaan, beli produk, cetak struk, keluar

def show_menu():
    print("""
=============================       
SELAMAT DATANG DI TOKO     
=============================
1. Cek Produk
2. Cek Ketersediaan
3. Beli produk
4. Cetak Struk
5. Exit
""")
    
def lihat_produk():
    print("\nList Produk : ")
    print("1. mawar : Rp.10000/tangkai")
    print("2. anggrek : Rp.15000/tangkai")
    print("3. melati : Rp.10000/tangkai \n")

def cek_ketersediaan(mawar, anggrek, melati):
    print("\nList Ketersediaan : ")
    print(f"1. mawar : {mawar}")
    print(f"2. anggrek : {anggrek}")
    print(f"3. melati : {melati}")

def beli_produk(saldo, mawar, anggrek, melati):
    lihat_produk()
    pilihan = input('pilih yang akan dibeli : ')
    if pilihan == '1':
        saldo
        jenis = 'mawar'
        harga = 10000
        jumlah = int(input('Berapa tangkai mawar : '))
        total = jumlah * harga
        pembelian = saldo - total
        if mawar < jumlah:
            print('maaf stok tidak ada')
        else:
            if total > saldo:
                print('maaf, saldo tidak cukup')
            else:
                print(f'Pembelian bunga {jenis} berhasil seharga {total}')
                print(f'Saldo saat ini : {pembelian}')
                try:
                    with open('struk.txt','a') as struk:
                        struk.write('===============\n')
                        struk.write('STRUK PEMBELIAN\n')
                        struk.write('===============\n')
                        struk.write(f'Nama Bunga   : {jenis} \n')
                        struk.write(f'Banyak bunga : {jumlah} \n')
                        struk.write(f'Harga Satuan : {harga} \n')
                        struk.write(f'total        : {total} \n')
                        struk.write(f'Saldo anda   : {saldo} \n')
                        struk.write(f'Kembalian    : {pembelian} \n')
                except Exception as e:
                    print(e)

    elif pilihan == '2':
        saldo
        jenis = 'anggrek'
        harga = 15000
        jumlah = int(input('Berapa tangkai anggrek : '))
        total = jumlah * harga
        pembelian = saldo - total
        if anggrek < jumlah:
            print('maaf stok tidak ada')
        else:
            if total > saldo:
                print('maaf, saldo tidak cukup')
            else:
                print(f'Pembelian bunga {jenis} berhasil seharga {total}')
                print(f'Saldo saat ini : {pembelian}')
                try:
                    with open('struk.txt','a') as struk:
                        struk.write('===============\n')
                        struk.write('STRUK PEMBELIAN\n')
                        struk.write('===============\n')
                        struk.write(f'Nama Bunga   : {jenis} \n')
                        struk.write(f'Banyak bunga : {jumlah} \n')
                        struk.write(f'Harga Satuan : {harga} \n')
                        struk.write(f'total        : {total} \n')
                        struk.write(f'Saldo anda   : {saldo} \n')
                        struk.write(f'Kembalian    : {pembelian} \n')
                except Exception as e:
                    print(e)

    elif pilihan == '3':
        saldo
        jenis = 'melati'
        harga = 10000
        jumlah = int(input('Berapa tangkai melati : '))
        total = jumlah * harga
        pembelian = saldo - total
        if melati < jumlah:
            print('maaf stok tidak ada')
        else:
            if total > saldo:
                print('maaf, saldo tidak cukup')
            else:
                print(f'Pembelian bunga {jenis} berhasil seharga {total}')
                print(f'Saldo saat ini : {pembelian}')
                try:
                    with open('struk.txt','a') as struk:
                        struk.write('===============\n')
                        struk.write('STRUK PEMBELIAN\n')
                        struk.write('===============\n')
                        struk.write(f'Nama Bunga   : {jenis} \n')
                        struk.write(f'Banyak bunga : {jumlah} \n')
                        struk.write(f'Harga Satuan : {harga} \n')
                        struk.write(f'total        : {total} \n')
                        struk.write(f'Saldo anda   : {saldo} \n')
                        struk.write(f'Kembalian    : {pembelian} \n')
                except Exception as e:
                    print(e)
    else:
        print('error')

def cetak_struk():
    try:
        with open('struk.txt','r') as saw:
            lihat = saw.read()
            print(lihat)
    except Exception as e:
        print(e)

def main():
    saldo = 500000
    mawar = 50
    anggrek = 50
    melati = 50

    while True:

        show_menu()
        pilihan = input('pilih menu : ')
        if pilihan == '1':
            lihat_produk()
        elif pilihan == '2':
            cek_ketersediaan(mawar, anggrek, melati)
        elif pilihan == '3':
            beli_produk(saldo, mawar, anggrek, melati)
        elif pilihan == '4':
            cetak_struk()
        elif pilihan == '5':
            exit()
            break
        else:
            print('inputan error')

if __name__ == '__main__':
    main()
