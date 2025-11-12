classDiagram
class Sach {
- id: string
- title: string
- author: string
- year: int
- quantity: int
- status: boolean
}

&nbsp;   class DocGia {
        - id: string
        - name: string
        + borrowBook(bookId): boolean
        + returnBook(bookId): boolean
    }

    class NhanVienThuVien {
        - id: string
        - name: string
    }

    DocGia --> Sach : muon / tra
    NhanVienThuVien --> Sach : quan ly

