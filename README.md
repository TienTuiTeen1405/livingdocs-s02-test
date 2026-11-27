# livingdocs-s02-test
test SHA mới 
ket qua : 
Đã kiểm thử trên test2 qua HTTPS với JWT S01, PostgreSQL và GitHub thật.
- SHA mới B 4eaae721… được API-069 đọc đúng, API-070 trả PASS/CURRENT.
- SHA cũ A 351ee463… bị cả hai API từ chối với 409 STALE_SHA.
- PostgreSQL đã lưu B với sourceRevision=1.
Do A chưa được S02 ghi nhận trên test2 trước lần commit vừa rồi, còn thiếu phép kiểm phiên bản nguồn tăng sau khi nhánh thay đổi.

Bạn tạo thêm một commit trên test2 nhé. Môi trường thử đang chạy và đã lưu B làm mốc. Lượt tiếp theo sẽ kiểm B bị từ chối, SHA mới được chấp nhận và sourceRevision tăng lên 2.


test tiep SHA moi : 
Đã kiểm thử đạt luồng SHA thay đổi thật trên test2.
- SHA cũ 4eaae721… bị cả API-069 và API-070 từ chối với 409 STALE_SHA.
- SHA mới b26ba429… được đọc đúng và xác minh PASS/CURRENT.
- PostgreSQL chuyển từ SHA cũ sang SHA mới, sourceRevision tăng từ 1 lên 2.
- Ba lượt xác minh cùng SHA mới giữ nguyên phiên bản 2.
Lượt kiểm thử dùng HTTPS, JWT do S01 cấp, GitHub App và PostgreSQL thật. Ca thay đổi đầu nguồn này đã đủ bằng chứng.
