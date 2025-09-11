# Nhom6_BTTuan4
package mypackage;

import java.util.Scanner;

public class BaiTapJava {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Bài 2
        String ten = "Luu Hong Nhung";
        int tuoi = 21;
        double chieuCao = 1.60;
        boolean thichLapTrinh = true;
        
        System.out.println("\n THONG TIN CA NHAN ");
        System.out.println("Ten: " + ten);
        System.out.println("Tuoi: " + tuoi);
        System.out.println("Chieu cao: " + chieuCao + "m");
        System.out.println("Co thich lap trinh khong: " + (thichLapTrinh ? "Co" : "Khong"));

        // Bài 4
        System.out.println("\n=== Bài 4 ===");
        System.out.print("Nhập số tiền gửi: ");
        double soTienGui = sc.nextDouble();
        System.out.print("Nhập lãi suất hàng năm (%): ");
        double laiSuatNam = sc.nextDouble();
        System.out.print("Nhập số tháng gửi: ");
        int soThang = sc.nextInt();

        // Lãi suất theo tháng
        double laiSuatThang = laiSuatNam / 12 / 100;
        double tienLai = soTienGui * laiSuatThang * soThang;
        double tongTien = soTienGui + tienLai;

        System.out.println("Tiền lãi: " + tienLai);
        System.out.println("Tổng số tiền cuối kỳ: " + tongTien);

        sc.close();
    }
}
