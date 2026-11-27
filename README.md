# livingdocs-s02-test
test SHA mới 
ket qua : 
Đã kiểm thử trên test2 qua HTTPS với JWT S01, PostgreSQL và GitHub thật.
- SHA mới B 4eaae721… được API-069 đọc đúng, API-070 trả PASS/CURRENT.
- SHA cũ A 351ee463… bị cả hai API từ chối với 409 STALE_SHA.
- PostgreSQL đã lưu B với sourceRevision=1.
Do A chưa được S02 ghi nhận trên test2 trước lần commit vừa rồi, còn thiếu phép kiểm phiên bản nguồn tăng sau khi nhánh thay đổi.

Bạn tạo thêm một commit trên test2 nhé. Môi trường thử đang chạy và đã lưu B làm mốc. Lượt tiếp theo sẽ kiểm B bị từ chối, SHA mới được chấp nhận và sourceRevision tăng lên 2.


test tiep SHA moi
