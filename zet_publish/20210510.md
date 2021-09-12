---
title: Setup lướt web tịnh tâm trong internet nhiều 💩
author: thuanpham2311
date: 2021-05-10 18:05
categories: [Blogging]
image:
  src: /assets/img/aniemPrayMeme.jpg
  alt: aniemPrayMeme
tags: [productive]
---

hello, bà con

Tâm tịnh đời vạn biến,

Tịnh tâm chốn tơ nẹt.

## Một số 💩 khi tui lướt web

- Quảng cáo
- Tà đạo (hacker, spammer,...)
- Web béo phì (ui/ux khó hiểu, tấn công tâm lý,...)

## Nhu cầu và các phần cứng

Một số nhu cầu cơ bản của tui khi lướt web:
- Xem youtube, anime, kdrama,...
- Web dev (chủ yếu về front-end)
- Design linh tin các thể loại
- Chiến đấu với bug
- Đọc tài liệu các thể loại

Một số phần cứng tui thường sử dụng lướt internet
- Điện thoại (android)
- Laptop (linux)

## Trình duyệt

Về trình duyệt tui chọn Brave Browser

Nói sơ về brave thì nó trong dòng họ chromium, được cài đặt mặc định về chặn quảng cáo, tracking,...


Trên điện thoại tui vào trang brave://adblock rồi tui chọn hai cái ô [x] ABPVN List và [x] Easylist-Cookie List

Nói chung nó sẽ có những cái filters để block ads hiệu quả hơn tại mấy trang web việt nam, với chặn mấy cái popup hỏi về cookie.

Trên điện thoại thì tui xài youtube trên web, để nó block mấy cái ads lại luôn. Với enable cái background video playback để tắt màn hình nhưng vẫn phát tiếng phù hợp với thể loại nghe nhạc trên youtube.

Có một cách block ads hiệu quả hơn, block ads tất cả thiết bị trong mạng nhà mấy đồng chí luôn, nguyên lý là chơi chặn ngay cổng ra vào mạng nhà mấy chế, mấy chế có thể tìm hiểu về Pi-hole, hay mấy cái tương tự vậy.

Để phòng chống tà đạo thì tui chơi chiêu, tạo mật khẩu ngẫu nhiên cho từng tài khoản cộng với xác thực hai lớp.

## Các liều vắc xin (extensions)

1. uBlock Origin: sử dụng phần block ads của brave thôi thì cũng okay rồi, tôi thì thích xử lý chặn những cái giao diện thông tin của những web béo phì nên tui xài thêm ublock origin này

Trong phần options thì tôi bật thêm mấy cái filter:
- Anti-Facebook
- EasyList Cookie
- VIE: ABPVN List

Còn về xử lý mấy cái web béo phì như youtube, facebook thì tui custom filter

```
www.youtube.com##ytd-topbar-menu-button-renderer.style-default.ytd-masthead.style-scope:nth-of-type(2)
www.youtube.com##ytd-toggle-button-renderer.style-text.force-icon-button.ytd-menu-renderer.style-scope > .ytd-toggle-button-renderer.style-scope.yt-simple-endpoint > .style-text.ytd-toggle-button-renderer.style-scope
www.youtube.com##ytd-guide-section-renderer.ytd-guide-renderer.style-scope:nth-of-type(4)
www.youtube.com##ytd-guide-section-renderer.ytd-guide-renderer.style-scope:nth-of-type(3)
www.youtube.com##ytd-guide-section-renderer.ytd-guide-renderer.style-scope:nth-of-type(2)
www.youtube.com##ytd-button-renderer.size-default.style-default.ytd-menu-renderer.style-scope:nth-of-type(3)
www.youtube.com##ytd-button-renderer.size-default.style-default.force-icon-button.ytd-menu-renderer.style-scope:nth-of-type(1)
www.youtube.com##yt-formatted-string.ytd-playlist-sidebar-primary-info-renderer.style-scope:nth-of-type(2)
www.youtube.com##span.ytd-video-meta-block.style-scope:nth-of-type(1)
www.youtube.com##span.ytd-grid-video-renderer.style-scope:nth-of-type(1)
www.youtube.com###voice-search-button > .size-default.style-default.ytd-masthead.style-scope
www.youtube.com###subscribers
www.youtube.com###subscriber-count
www.youtube.com###subscribe-button > .ytd-video-secondary-info-renderer.style-scope
www.youtube.com###subscribe-button > .ytd-channel-renderer.style-scope
www.youtube.com###sponsor-button
www.youtube.com###separator
www.youtube.com###sentiment
www.youtube.com###related
www.youtube.com###owner-sub-count
www.youtube.com###logo
www.youtube.com###guide-links-secondary
www.youtube.com###guide-links-primary
www.youtube.com###dot
www.youtube.com###count > .ytd-video-primary-info-renderer.style-scope
www.youtube.com###copyright
www.youtube.com###buttons > .ytd-c4-tabbed-header-renderer.style-scope
www.google.com##div:nth-of-type(12)
www.google.com##.logo
www.google.com##.hpuQDe
www.facebook.com##li.hw7htvoc.h676nmdw.dawyy4b1.jrc8bbd0.o5zgeu5y.to382e16.buofh1pr:nth-of-type(4)
www.facebook.com##li.hw7htvoc.h676nmdw.dawyy4b1.jrc8bbd0.o5zgeu5y.to382e16.buofh1pr:nth-of-type(3)
www.facebook.com##div.sjgh65i0 > div > div > div > div > .k4urcfbm.l9j0dhe7.j83agx80
www.facebook.com##.sbcfpzgs.stjgntxs.ni8dbmo4.k4urcfbm.nwvqtn77.fbipl8qg.m5lcvass.io0zqebd.hybvsw6c.du4w35lb.l9j0dhe7.rq0escxv > div > div > .k4urcfbm.l9j0dhe7.j83agx80 > .sbcfpzgs.stjgntxs.ni8dbmo4.k4urcfbm.nwvqtn77.fbipl8qg.m5lcvass.io0zqebd.hybvsw6c.du4w35lb.l9j0dhe7.rq0escxv > .d2edcug0.pfnyh3mw.cbu4d94t.j83agx80.du4w35lb.l9j0dhe7.rq0escxv > .tgvbjcpo.buofh1pr.cbu4d94t.j83agx80.du4w35lb.l9j0dhe7.rq0escxv > div.d2edcug0.pfnyh3mw.cbu4d94t.j83agx80.du4w35lb.l9j0dhe7.rq0escxv
www.facebook.com##.kcmanqeg.g2wm7t24.n99bqvw7.rek2kq2y.aghb5jc5.h676nmdw.bi6gxh9e.oi9244e8.aov4n071.g5gj957u.buofh1pr.o387gat7.hpfvmrgz.qmfd67dx.du4w35lb.l9j0dhe7.rq0escxv
www.facebook.com##.hlyrhctz.be9z9djy.stjgntxs.ni8dbmo4.fer614ym.dp1hu0rb.rirtxc74.pad24vr5.qbu88020.o387gat7.du4w35lb.lpgh02oy.rq0escxv
www.facebook.com##.ejjq64ki.v8c10jal.e3xpq0al.d2edcug0
www.facebook.com##.ejjq64ki.abvwweq7.oh7imozk.d2edcug0 > div.sjgh65i0 > .k4urcfbm.l9j0dhe7.j83agx80
www.facebook.com##.bx45vsiw.be9z9djy.rek2kq2y.stjgntxs.ni8dbmo4.fer614ym.dp1hu0rb.rirtxc74.pad24vr5.qbu88020.o387gat7.du4w35lb.lpgh02oy.rq0escxv
www.facebook.com##.bp9cbjyn.rq0escxv.j83agx80.buofh1pr.byvelhso.dhix69tm.poy2od1o.j9ispegn.kr520xx4.ehxjyohh

```

Tui thích tự custom, nếu đồng chí muốn giảm béo cho mấy cái web béo phì thì mấy chế có thể sử dụng cái này cho tiện, trên web nó có nói một số triết học về web béo phì cũng okay nha.

[https://minimal.aupya.org/](https://minimal.aupya.org/)

2. SponsorBlock for YouTube: nói chung nó sẽ bỏ qua khoảng nội dung quảng cáo của cá nhân kênh trên video, mấy cái tài trợ, giới thiệu sản phẩm các thứ
3. YouTube NonStop: tui hay nghe nhạc trên youtube, thường tui bấm vô cái playlist music của tui rồi nó tự chạy, nhưng chạy được một khoảng thì nó sẽ hiện cái khung youtube hỏi bạn muốn tiếp tục hay không gì đó, nó ngừng phát nhạc nên hơi cay, nên tui xài cái extension này
4. Octotree: nó thêm một cái cây thư mục trên trang github, khi vào repo, nó giống cái cây thư mục trên cái chỗ gõ code của bạn ý.
5. Vimium: là một vimer chân chính không thể bỏ qua cái extension này, nói 	chung không cần chuột khi lướt web. Hiện tại cái project này vài tháng rồi chưa có commit nên tui dự định chuyển sang cái khác, mà tui hiện tại thì lười.
6. Google Translate: khi các bạn select một chữ, hay một cụm gì đó thì nó sẽ hiện pop up hiện lên dịch từ đó nghĩa là gì, tiện trong việc đọc tài liệu trên web.
7. OneTab: nói chung gộp một đống tab lại thành một cục, tui sử dụng trong khi đọc nhiều blogs, hay muốn lưu lại đọc sau.

## Tóm cái quần lại

Mấy công cụ trên thì giúp ích chúng ta một phần trong công cuộc tịnh tâm khi lướt web, còn về mặt tư tưởng, suy nghĩ cá nhân, cách nhìn nhận thì tui thấy cũng quan trọng không kém, mấy chế có thể tìm hiểu thêm về chủ đề này nha.

**Ref:**
- Hội nghiện code trên github: [https://github.com/dsc-stu](https://github.com/dsc-stu)
- Github của tui: [http://github.com/thuanpham2311](http://github.com/thuanpham2311)
- Đọc thêm mấy cái xàm xí của tui: [https://thuanpham2311.github.io](https://thuanpham2311.github.io)

---

**DISCLAIMER**

Những câu chuyện, bài học và lời khuyên của tui là những trải nghiệm riêng của cá nhân, không phản ánh ý kiến từ những tổ chức hay công ty nào. Đa phần lời tui viết là chém gió, nên mấy chế nên suy ngẫm nó có phù hợp với hoàn cảnh của bản thân không nha.
