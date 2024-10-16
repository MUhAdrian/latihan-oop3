# latihan-oop3
#   ENKAPSULASI
public class person {
    private int umur;
    private String nama;
    private String jeniskelamin;

    public void setNama(String nama){
        this.nama = nama;
    }

    public void setJeniskelamin(String jeniskelamin){
        this.jeniskelamin = jeniskelamin;
    }

    public void setUmur(int umur){
        this.umur = umur;
    }

    public String getNama(){
        return this.nama;
    }

    public String getJeniskelamin(){
        return this.jeniskelamin;
    }

    public int getUmur(){
        return this.umur;
    }

    public static void main(String[] args) {
        person anton = new person();
        person riko = new person();

        anton.setNama("anton lari maraton");
        anton.setJeniskelamin("laki-laki");
        anton.setUmur(99);

        riko.setNama("riko cox");
        riko.setJeniskelamin("perempuan");
        riko.setUmur(1);

        System.out.println("Nama: " + anton.getNama() + 
        ", Jenis Kelamin: " + anton.getJeniskelamin() + 
        ", Umur: " + anton.getUmur());
        System.out.println("Nama: " + riko.getNama() 
        + ", Jenis Kelamin: " + riko.getJeniskelamin() 
        + ", Umur: " + riko.getUmur());
    }
}

#ALASAN MENGGUNAKAN SETTER DAN GETTER
1.gunanya untuk enkapsulasi alias agar data atribut tidak dapat dipakai selain dari class itu sendiri
2.kontrol penuh pada data yang memungkinkan kita dapat dengan mudah menambah logika atau atribut tambahan
3.fleksibel (saya gatau kenapa fleksibel,tpi kata gugel gitu)
4.mencegah berubahnya atribut dari luar class

#KESIMPULANNYA
dengan setter dan getter membuat konsep dari OOP itu sendiri berjalan dengan baik,juga memberikan kontrol lebih terhadap bagaimana atribut diakses dan dimodifikasi. Ini sangat penting dalam menjaga integritas data, memungkinkan validasi, serta memastikan data dikelola dengan cara yang benar sesuai
