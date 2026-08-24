# WDchocopie Extensions

Kho extension tự host cho [Mihon](https://mihon.app).

**[English](README.md)**

---

## Đây là gì

Mihon là ứng dụng đọc truyện nhưng không kèm sẵn nguồn truyện nào. Nguồn đến từ các *extension*, còn extension đến từ một *kho extension* — là một đường dẫn bạn thêm vào ứng dụng. Repo này chính là một kho như vậy.

Thêm đường dẫn bên dưới là Mihon biết chỗ tải các extension trong danh sách, và tự báo cho bạn khi có bản mới.

## Cách cài

**1. Cài Mihon**

Tải tại [mihon.app](https://mihon.app) hoặc [trang phát hành trên GitHub](https://github.com/mihonapp/mihon/releases).

**2. Thêm kho này**

Trong ứng dụng, vào **More → Settings → Browse → Extension stores → Add**, rồi dán:

```
https://raw.githubusercontent.com/wdchocopie/mihon-extensions/main/repo.json
```

Kho sẽ hiện lên với tên *WDchocopie Extensions*.

> Đường dẫn phải trỏ thẳng tới `repo.json`. Dán đường dẫn thư mục mà thiếu tên file sẽ báo lỗi `HTTP error 404`.

**3. Cài extension**

Vào **Browse → Extensions**, tìm extension rồi bấm biểu tượng tải xuống.

**4. Bật ngôn ngữ**

Mihon ẩn những nguồn thuộc ngôn ngữ bạn chưa bật, mà tiếng Việt thì mặc định tắt. Nếu thấy danh sách trống, vào **Browse → Extensions → ⋮ → Filter** rồi bật **Tiếng Việt**.

## Extension hiện có

| Extension | Ngôn ngữ | Phiên bản | Website |
|---|---|---|---|
| TruyenQQ VN | Tiếng Việt | 1.6.1 | https://truyenqq.com.vn |

## Gặp lỗi thì làm gì

**Báo "HTTP error 404" khi thêm kho**
Đường dẫn thiếu `/repo.json` ở cuối.

**Danh sách extension trống**
Bộ lọc ngôn ngữ đang ẩn nó. Xem bước 4 ở trên.

**Làm bước 4 rồi vẫn trống**
Kéo danh sách xuống để làm mới, hoặc mở lại ứng dụng.

**Ảnh trong chương không hiện**
Website chặn ảnh khi bị gọi từ bên ngoài trang của họ. Extension đã tự gửi kèm thông tin cần thiết để vượt qua, nên nếu ảnh vẫn hỏng thì nhiều khả năng website đã đổi cấu trúc — bạn mở issue giúp mình nhé.

## Ghi chú

Extension ở đây được ký bằng khóa riêng của kho này. Mihon đối chiếu chữ ký đó với dấu vân tay công bố trong index, nên extension cài từ kho này được tin cậy tự động, không hiện cảnh báo "untrusted extension".

Cũng vì chữ ký phải khớp, extension cài từ kho này không thể cập nhật đè lên bản đã cài từ nguồn khác. Hãy gỡ bản cũ trước.

## Mã nguồn

Mã nguồn extension nằm ở [wdchocopie/extensions-source](https://github.com/wdchocopie/extensions-source), là bản fork của repo [Keiyoushi](https://github.com/keiyoushi/extensions-source).

## Ghi công

Xây dựng dựa trên [Mihon](https://github.com/mihonapp/mihon) và bộ khung extension do [Keiyoushi](https://github.com/keiyoushi/extensions-source) duy trì.
