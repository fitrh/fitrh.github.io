# Tugas Praktikum 2 : Penyeleksian Kondisi

Lengkapilah potongan program barikut

```java
class Role {

  public static void main(String[] args) {
    int menuIndex = 0;
    int subMenuIndex = 0;
    boolean isValidRole = false;

    if (args.length == 0) {
      System.out.println("What role you want to see ?");
      System.out.println("For example, try 'Admin'.");
    } else if (args.length == 1) {
      // Your magic is here
      if (...) {
        // Another magic
      } else {
        System.out.println("Invalid Role");
        System.out.println("Valid Role : Super Admin, Admin, User");
      }
    } else {
      System.out.println("Too many argument");
    }
  }
}
```

Sehingga menghasilkan output berikut

[![asciicast](https://asciinema.org/a/365892.svg)](https://asciinema.org/a/365892)

## Dengan Ketentuan

- Tidak ada varaiabel tambahan selain variabel yang telah disediakan

- Gunakan `args[0]` sebagai variabel pengecekan _Role_

- Index menu dan sub menu bersifat dinamis (sesuai _Role_) yang merupakan hasil dari variabel `indexMenu` dan `indexSubmenu`

- Tidak ada duplikasi dalam menampilkan menu masing-masing _Role_

```java
if (args[0] == "Admin") {
  System.out.printf("%d. Admin\n", menuIndex);
  System.out.printf("%2d.%d. CRUD Admin\n", menuIndex, subMenuIndex);
  System.out.printf("%2d.%d. CRUD User\n\n", menuIndex, subMenuIndex);
  System.out.printf("%d. User\n", menuIndex); // Duplikasi, bagian ini hanya boleh terdapat dibagian User
  System.out.printf("%2d.%d. View\n", menuIndex, subMenuIndex); // Duplikasi, bagian ini hanya boleh terdapat dibagian User
  System.out.printf("%2d.%d. Edit\n", menuIndex, subMenuIndex); // Duplikasi, bagian ini hanya boleh terdapat dibagian User
} else if (args[0] == "User") {
  System.out.printf("%d. User\n", menuIndex);
  System.out.printf("%2d.%d. View\n", menuIndex, subMenuIndex);
  System.out.printf("%2d.%d. Edit\n", menuIndex, subMenuIndex);
}
```

> - Diatas merupakan contoh duplikasi, dimana **role** **Admin** menampilkan menu **User** dalam pengecekan kondisinya
> - Setiap **Role** hanya menampilkan menu untuk **Role** tersebut dialam blok pengecekannya

- Ketentuan menu masing-masing _Role_
  - _Super Admin_ dapat melihat menu untuk _Admin_ dan _User_
  - _Admin_ dapat melihat menu untuk _User_ tapi tidak dapat melihat menu _Super Admin_
  - _User_ hanya dapat melihat menu _User_

Untuk lebih jelasnya, silahkan perhatikan bagian output
