---
title: tối ưu hóa tốc độ tìm kiếm fzf trong vim, cli
author: thuanpham2311
date: 2021-09-03 08:44
categories: [Blogging]
tags: [vim, terminal]
---

Cách của tui như sao:
- Không search hidden files, folder (.git, ~/.config, .??)
- Bỏ mấy thư mục mà không cần tìm như là (gems,...), đặc biệt chế nào xài undodir thì nên exclude undodir folder luôn tại vì vừa giảm được file phải tìm và khỏi chọn nhầm luôn, mấy bạn có thể chạy fzf rồi review thử xem cái folder hay loại file nào không cần thì exclude nó luôn
- Tui chỉnh file config của shell thì vim nó nhận config đó khi mình chạy một terminal nó sẽ load qua file config của shell rồi từ đó vim sẽ nhận mấy cái setting của fzf, tui có thử xài telescope thì nó không phụ thuộc vào cái setting này không biết cần phải chỉnh gì không tui có xem sơ qua wiki nhưng không tìm thấy cách nào, chắc do tu đọc không kỉ :D , chế nào biết chỉnh telescope thì thú tui cái. Tạm thời thì xài fzf, fzf.vim thì bình thường.

```bash
# debian
export FZF_DEFAULT_COMMAND='fdfind --type f --follow --exclude .git --exclude undodir --exclude gems'
# arch | termux | fedora
export FZF_DEFAULT_COMMAND='fd --type f --follow --exclude .git --exclude undodir --exclude gems'
```


**Reference**

-   Dotfiles: <https://github.com/thuanpham2311/dotfiles>
-   Github của tui: [http://github.com/thuanpham2311](http://github.com/thuanpham2311)
-   Đọc thêm mấy cái xàm xí của tui: [https://thuanpham2311.github.io](https://thuanpham2311.github.io)

---

**DISCLAIMER**

Những câu chuyện, bài học và lời khuyên của tui là những trải nghiệm riêng của cá nhân, không phản ánh ý kiến từ những tổ chức hay công ty nào. Đa phần lời tui viết là chém gió, nên mấy chế nên suy ngẫm nó có phù hợp với hoàn cảnh của bản thân không nha.
