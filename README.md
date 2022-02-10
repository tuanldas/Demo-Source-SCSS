* Abstracts là nơi định nghĩa variables, function, mixins
* Base bao gồm những tiêu chuẩn style như reset, rule và phần chung dùng xuyên suốt project
* Component ( or modules ) định nghĩa các style dành cho buttons, tabs, card, sliders và các thành phần tương tự, thông thường 1 project sẽ có nhiều componets như vậy 
* Layout chứa tất cả các styles liên quan đến layout trong project của bạn. Ví dụ như phần header, footer, navigation và grid system.
* Pages những styles cho từng trang cụ thể. Ví dụ như có một trang không cùng styles với các trang khác và bạn không muốn để ở phần styles chung.
* Vendors (có thể import từ node_modules) bao gồm tất cả những phần code mở rộng của bên thứ 3 của thư viện như, jQuery, Bootstrap...
* main.scss dùng import các file khác để tạo ra file css chung cho cả website.

```
@import 'abstracts/variables';
@import 'abstracts/functions';
@import 'abstracts/mixins';

// Import library from node_modules
@import 'node_modules/jquery';
@import 'node_modules/bootstrap';

@import 'base/reset';
@import 'base/fonts';
@import 'base/animation';
@import 'base/global';

@import 'layout/grid';
@import 'layout/header';
@import 'layout/footer';
@import 'layout/navigation';
@import 'layout/sidebar';
@import 'layout/forms';

@import 'components/buttons';
@import 'components/tabs';
@import 'components/slider';

@import 'pages/home';
@import 'pages/about';
@import 'pages/contact';

@import 'base/utilities';
```
