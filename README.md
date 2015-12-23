# DoAnVb
đồ án cuối kỳ
Imports DAO

Public Class BUS_GiaoVien

    Shared dt_GiaoVien As DataTable
    'ham lay danh sach cac giao vien
    Shared Function Bus_DanhSachGiaoVien()
        dt_GiaoVien = New DataTable
        dt_GiaoVien = DAO.DAO_GiaoVien.DAO_XuatGiaoVien()
        Return dt_GiaoVien
    End Function

    'ham lay danh sach cac giao vien theo tung bo mon
    Shared Function Bus_GiaoVien_BoMon(ByVal bomon As String)
        dt_GiaoVien = New DataTable
        dt_GiaoVien = DAO_GiaoVien.DAO_GiaoVien_BoMon(bomon)
        Return dt_GiaoVien
    End Function
End Class
