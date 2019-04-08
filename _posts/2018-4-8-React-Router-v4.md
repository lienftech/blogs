---
layout: post
title: Tất tần tật về React Router V4
---
Trước tiên để hiểu được các cú pháp code trong bài này, các bạn hãy hiểu về những khái niệm sau đã nhé (Mình sẽ đề cập sau các bài sau)
- React [(Stateless) Functional Components ](https://reactjs.org/docs/components-and-props.html)
- ES2015 [Arrow Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions) và "implicit returns" của nó
- ES2015 [Destructuring](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)
- ES2015 [Template Literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)

OK! Nếu bạn thích nhảy vô demo luôn thì đây là link nhé
[demo](https://codepen.io/bradwestfall/project/editor/XWNWge/?preview_height=50&open_file=src/app.js)

Ok! let's go

# #API mới và mô hình mới so với React Router version cũ
Trong những version trước của React Router, định nghĩa Route rules được đặt vào 1 chỗ (thường thì là 1 file như app.jsx hay index.jsx hay file riêng,vân vân và mây mây), chỗ định nghĩa route đó thì thường là riêng biệt với các file components. Trong React Router V4 (mình sẽ viết tắt là v4 nhé) có thể nó sẽ được đặt ở nhiều chỗ hơn, phân mảnh và định nghĩa ở nhiều files hơn. 

Có lẽ cách tốt nhất để xem v4 khác với các version khác thế nào thì chúng ta hãy thử viết 2 trang đơn giản, mỗi trang chạy một version và thử so sánh chúng. Ví dự dưới đây mình sẽ dẫn ra hai routes là Home page và User's page nhé. Cùng coi nào!

Đây là v3 nhé:

![_config.yml]({{ site.baseurl }}/images/config.png)
