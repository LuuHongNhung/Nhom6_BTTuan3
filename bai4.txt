# Nhom6_BTTuan4
package mypackage;

import java.util.Scanner;

public class BaiTapJava {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

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