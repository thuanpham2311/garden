---
title: trong vim mấy phím mũi tên làm cái chi khi có hjkl?
author: thuanpham2311
date: 2021-08-11 15:42
categories: [Blogging]
tags: [vim]
---

- theo kinh vimmer thì mấy cái phím mũi tên vô dụng nên tui map lại thành cái resize window.
- kết hợp với cái xmodmap ở trên nó cũng được nha.

```bash
map <silent> <Right> <C-w><
map <silent> <Down> <C-W>-
map <silent> <Up> <C-W>+
map <silent> <Left> <C-w>>
```

bonus :smile:

```bash
noremap ss :split<Return><C-w>w
noremap sv :vsplit<Return><C-w>w
```

**Reference**

- Github của tui: [http://github.com/thuanpham2311](http://github.com/thuanpham2311)
- Đọc thêm mấy cái xàm xí của tui: [https://thuanpham2311.github.io](https://thuanpham2311.github.io)

---

**DISCLAIMER**

Những câu chuyện, bài học và lời khuyên của tui là những trải nghiệm riêng của cá nhân, không phản ánh ý kiến từ những tổ chức hay công ty nào. Đa phần lời tui viết là chém gió, nên mấy chế nên suy ngẫm nó có phù hợp với hoàn cảnh của bản thân không nha.
