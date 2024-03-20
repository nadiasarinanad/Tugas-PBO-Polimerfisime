# PBO-5-POLIMORFISME

Berikut adalah contoh tiga program Java yang menggunakan konsep polimorfisme, masing-masing mengimplementasikan overloading dan overriding dengan permasalahan yang berbeda:

**1.** **Overloading (Polimorfisme Statis)**: Menghitung luas bangun datar (persegi dan lingkaran) dengan menggunakan metode overloading.

```java
class HitungLuas {
    // Overloading untuk persegi
    double hitungLuas(int sisi) {
        return sisi * sisi;
    }

    // Overloading untuk lingkaran
    double hitungLuas(double jariJari) {
        return Math.PI * jariJari * jariJari;
    }
}

public class Main {
    public static void main(String[] args) {
        HitungLuas hitung = new HitungLuas();
        System.out.println("Luas persegi: " + hitung.hitungLuas(4));
        System.out.println("Luas lingkaran: " + hitung.hitungLuas(3.5));
    }
}
```

**2.** **Overriding (Polimorfisme Dinamis)**: Menggunakan kelas induk dan kelas turunan untuk menampilkan informasi tentang hewan.

```java
class Hewan {
    void suara() {
        System.out.println("Beberapa hewan membuat suara...");
    }
}

class Kucing extends Hewan {
    @Override
    void suara() {
        System.out.println("Meong!");
    }
}

class Anjing extends Hewan {
    @Override
    void suara() {
        System.out.println("Guk Guk!");
    }
}

public class Main {
    public static void main(String[] args) {
        Hewan hewan1 = new Kucing();
        Hewan hewan2 = new Anjing();

        hewan1.suara();
        hewan2.suara();
    }
}
```

**3.** **Overloading dan Overriding Bersamaan**: Menggunakan kelas abstrak dan turunannya untuk menghitung luas dan volume bangun ruang (kubus dan bola).

```java
abstract class BangunRuang {
    abstract double hitungLuas(); // Overriding
    abstract double hitungVolume(); // Overriding
}

class Kubus extends BangunRuang {
    double sisi;

    Kubus(double sisi) {
        this.sisi = sisi;
    }

    @Override
    double hitungLuas() {
        return 6 * sisi * sisi;
    }

    @Override
    double hitungVolume() {
        return sisi * sisi * sisi;
    }
}

class Bola extends BangunRuang {
    double jariJari;

    Bola(double jariJari) {
        this.jariJari = jariJari;
    }

    @Override
    double hitungLuas() {
        return 4 * Math.PI * jariJari * jariJari;
    }

    @Override
    double hitungVolume() {
        return (4.0 / 3.0) * Math.PI * jariJari * jariJari * jariJari;
    }
}

public class Main {
    public static void main(String[] args) {
        BangunRuang kubus = new Kubus(5);
        BangunRuang bola = new Bola(4);

        System.out.println("Luas Kubus: " + kubus.hitungLuas());
        System.out.println("Volume Kubus: " + kubus.hitungVolume());

        System.out.println("Luas Bola: " + bola.hitungLuas());
        System.out.println("Volume Bola: " + bola.hitungVolume());
    }
}
```
