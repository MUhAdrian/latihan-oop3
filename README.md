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
