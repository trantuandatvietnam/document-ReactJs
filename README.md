<span style="color:red; font-size: 20px">**Học ReactJs**</span>

<span style="color:yellow">**Giới thiệu ReactJs**</span>

-   reactJs là thư viện được viết từ javascript được viết bởi đội ngũ kĩ sư facebook được sử dụng để xây dựng giao diện người dùng
-   Cộng đồng lớn
-   Được đánh giá là thân thiện với SEO trong những Lib/Fw Js
    (SEO - Search Engine Optimization)
-   Khả năng mở rộng tốt, tái sử dụng cao
-   Hiệu suất cao, phát triển nhanh chóng
-   Khả năng tương thích ngược
-   Tương lai sáng
-   Lộ trình học ReactJs
    -   Giới thiệu
        -   ReactJs là gì?
        -   SPA là gì?
    -   Ôn lại ES6
        -   Arow function
        -   Js module
        -   Enhanced object literals
        -   Spread operator
        -   Destructering
    -   Làm quen với React Element
        -   Thêm React vào dự án
        -   Document.createElement
        -   React.createElement
        -   Hiểu về thư viện React Dom
        -   Render UI với React Dom
    -   Tính năng cơ bản và dự án
        -   Tạo dự án với create-react-app
        -   Cấu trúc thư mục của create-react-app
        -   JSX là gì
        -   Function Conponent
        -   Class Component
        -   Sử dụng lại Component
        -   Khái niệm Props
        -   Childen Prop
        -   Pass Props
        -   Thư viện "prop-types"
        -   Khái niệm state
        -   Phân biệt Props & State
        -   Xử lí dom event
        -   Stateless & Stateful Component
        -   Thêm "To way binding"
        -   Viết Css inline
        -   Viết Css externals
        -   Sử dụng Scss
        -   Render nội dung với điều kiện
    -   Style trong ReactJs
        -   Giới thiệu css modules
        -   sử dụng đồng thời nhiều classes
        -   Sử dụng nhiều className động (dinamically)
        -   Sử dụng thư viện "classesnames"
        -   Sử dụng styled trong components
    -   Thư viện react router dom
        -   Điều hướng trang với react router dom
    -   Tìm lỗi và sửa lỗi (debug)
        -   Sử dụng react developer tools
        -   Khái niệm sourcemaps
        -   Sử dụng Error Bondaries Component
    -   Xây dựng cấu trúc dự án
        -   Cấu trúc thư mục dự án
        -   Cấu trúc components
        -   Cấu trúc assets
        -   Cấu trúc ulti
        -   Thêm file cấu hình
    -   Cấu hình theo môi trường
        -   Environment là gì? Tại sao phải sử dụng nó?
        -   Thêm tệp cấu hình môi trường vào dự án
    -   Hooks
        -   Khái niệm
        -   Sử dụng useState() hook
        -   Sử dụng Effect() hook
        -   Sử dụng useCallback() hook
        -   Tự tạo hook của bạn Custom Hook
    -   Các kĩ thuật tối ưu
        -   Sử dụng props key sao cho đúng
        -   Tối ưu component với react.memo()
        -   Hiểu cách React cập nhật lại Dom
        -   Các kĩ thuật tránh re-render không cần thiết
        -   Kĩ thuật Lazy Load Components
        -   Sử dụng thư viện Loadable
        -   Component bậc cao (HOC)
    -   Context Api
        -   Vấn đề khi truyền Props nhiều cấp
        -   Sử dụng Context API
    
    - Một số thư viện ReactJs animation
    	- https://www.framer.com/docs/introduction/ 

<span style="color:yellow">**SPA**</span>

-   SPA (Single page application): ứng dụng trang đơn
-   ReactJs là một trong những thư viện giúp ta tạo ra SPA
-   MPA(Multi-Page application): ứng dụng nhiều trang
-   Sự khác biệt:
    -   SPA:
        -   Được cho là cách tiếp cận hiện đại hơn
        -   Không yêu cầu tải lại trang trong quá trình sử dụng
    -   MPA:
        -   Là cách tiếp cận cổ điển hơn
        -   Tả lại trang trong quá trình sử dụng (click vào đường link, chuyển sang)
-   So sánh:
    -   Tốc độ:
        -   SPA nhanh hơn khi sử dụng
            -   Phần lớn tài nguyên được tải trong lần đầu
            -   Trang chỉ tải thêm dữ liệu mới khi cần
        -   MPA chậm hơn khi sử dụng
            -   Luôn tải lại toàn toàn bộ trang khi truy cập và chuyển hướng
-   Bóc tách
    -   SPA có phần front-end riêng biệt
    -   MPA có phần front-end và backend phụ thuộc nhiều hơn, được đặt trong cùng dự án
-   Seo
    -   SPA không thân thiện với Seo như MPA
    -   SPA trải nghiệm trên thiết bị di động tốt hơn
-   UX
    -   SPA cho trải nghiệm tốt hơn, nhất là khi chuyển trang
-   Quá trình phát triển
    -   SPA dễ dàng tái sử dụng code (component)
    -   SPA bóc tách front-end & backend
        -   Có thể chia team phát triển song song
        -   Phát triển thêm mobile app dễ dàng
-   Phụ thuộc Javascript
    -   SPA phụ thuộc hoàn toàn vào Javascript
    -   MPA có thể không cần Javascript
-   Chọn SPA hay MPA?
    -   Không có gì hoàn hảo trong mọi trường hợp
-   Tên gọi khác:
    -   SPA: CSR (Client side rendering)
    -   SSR: Server Side rendering

<span style="color:yellow">**Arrow function**</span>

```javascript
// Ví dụ 1
const logger = (message) => {
    console.log(message);
};
logger('I love you so much!');

// Ví dụ 2
const sum = (a, b) => a + b; //nếu không có dấu {} => nó sẽ hiểu là return giá trị đằng sau nó
const result = sum(2, 2);
console.log(result);

// Ví dụ 3: muốn return luôn ra một object mà không cần dùng tới "return"
const myObj = (firstName, lastName) => ({
    //kí tự đầu tiên sau dấu "=>" nếu khác "{}" được hiểu là return
    firstName: firstName,
    lastName: lastName,
});
const result = myObj('Dat', 'Tran');
console.log(result);

// Ví dụ 4: Khi số lượng tham số truyền vào là 1 thì có thể viết ngắn gọn như sau:
const log = (mess) => console.log(mess);
log('hihi ngắn thế!');

// Ví dụ 5: Xét hai ví dụ sau:
const myObj = {
    name: 'dat',
    getName: function () {
        return this; //context
    },
};

console.log(myObj.getName()); //in ra chính this (đó là myObj)

('use strict');
this.name = 'Mai';
const myObj = {
    name: 'dat',
    getName: () => {
        return this; //context của nó lúc này là đối tượng Window
    },
};

console.log(myObj.getName().name); //in ra Mai

// Ví dụ 6:
const Animal = (name) => {
    this.name = name;
};

const dog = new Animal('Tom');
// sẽ gặp lỗi: Animal is not a constructor

// Ví dụ 5: Arow Funcion no argument
('use strict');
const logger = () => console.log('no argument!');
logger();
```

<span style="color:yellow">**Document.createElement để làm gì?**</span>

```javascript
const h1 = document.querySelector('h1');
console.log(typeof h1); //object
```

Ví dụ:

```html
<body>
    <div id="root"></div>
    <script src="./main.js"></script>
</body>
```

```javascript
const root = document.getElementById('root');
const h1 = document.createElement('h1');
h1.innerHTML = 'Hello reactJs';
h1.className = 'heading heading__title';
h1.style.color = 'red';
// Hoặc sử dụng cách sau: (Sử dụng quy tắc CamelCase)
Object.assign(h1.style, {
    color: 'blue',
    fontSize: 50 + 'px',
});
root.appendChild(h1);
```

<span style="color:yellow">**Cách thêm React vào Website**</span>

**npm**: node package maneger(Quản lý gói cho node)

-   Khái niệm:
    -   Cdn: content delivery network
-   Tìm hiểu thêm tại: [Unpkg](https://unpkg.com/)
-   Sau khi thêm react vào app thì sẽ có một biến global đó là React
-   API trong một thư viện là một method để làm việc với thư viện

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>CSS Flexbox equal</title>
        <link rel="preconnect" href="https://fonts.gstatic.com" />
        <link
            href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap"
            rel="stylesheet"
        />
        <link rel="stylesheet" href="main.css" />
        <!-- Thêm react vào website(link trên trang chủ) -->
        <script
            src="https://unpkg.com/react@17/umd/react.development.js"
            crossorigin
        ></script>
    </head>

    <body>
        <div id="root"></div>
        <script src="./main.js"></script>
    </body>
</html>
```

<span style="color:yellow">**React.createElement()**</span>

-   Nội dung bài học:

    1. React.createElement(type, props, children, ...childrenN) -> ReactElement (là thành phần nhỏ nhất khi làm việc với react)

    -   thực ra khi thể hiện element thì react coi children như một props

    2. So sánh với document.createElement() -> DOM element (Thành phần nhỏ nhất của DOM là node)
    3. Thay đổi id, className, style, ...
    4. Thêm text, HTML
    5. Tạo:

    ```html
    <h1 title="Hello" class="heading">Hello guy!</h1>
    ```

    6. Tạo:

    ```html
    <ul>
        <li>Javascript</li>
        <li>ReactJs</li>
    </ul>
    ```

    7. Tạo:

    ```html
    <div class="post-item">
        <h2 title="Học ReactJs tại F8">Học ReactJs</h2>
        <p>Học ReactJs từ cơ bản tới nâng cao</p>
    </div>
    ```

-   Thực hiện

Bài làm: 5.

```javascript
// Cách làm với create element
const h1 = document.createElement('h1');
h1.title = 'Hello';
h1.className = 'heading';
h1.textContent = 'Hello guy!';
const root = document.querySelector('#root');
root.appendChild(h1);
// Cách làm với reactJs
const h1Reatc = React.createElement(
    'h1',
    {
        title: 'Hello',
        className: 'heading',
    },
    'Hello guys'
);
```

Bài làm 6:

```javascript
// Cách làm với create element
const ulDom = document.createElement('ul');
ulDom.id = 'ul-id';
ulDom.style = 'color: red';
const liDom1 = document.createElement('li');
liDom1.textContent = 'Javascript';
const liDom2 = document.createElement('li');
liDom2.textContent = 'ReactJs';
ulDom.appendChild(liDom1);
ulDom.appendChild(liDom2);
const root = document.querySelector('#root');
root.appendChild(ulDom);
// Cách làm với reactJs
const ulReact = React.createElement(
    'ul',
    {
        id: 'ul-id',
        style: 'color; red',
    },
    React.createElement('li', null, 'Javascript'),
    React.createElement('li', null, 'Javascript')
);
```

Bài làm 7:

```javascript
// Cách làm với create element
const divDom = document.createElement('div');
divDom.className = 'post-item';
const h2Dom = document.createElement('h2');
h2Dom.title = 'Học lập trình ReactJs tại F8';
h2Dom.textContent = 'Học ReactJs';
const pDom = document.createElement('p');
pDom.textContent = 'Học lập trình ReactJs từ căn bản tới nâng cao';
divDom.appendChild(h2Dom);
divDom.appendChild(pDom);
const root = document.querySelector('#root');
root.appendChild(divDom);
// Cách làm với reactJs

const divReact = React.createElement(
    'div',
    {
        className: 'post-item',
    },
    React.createElement(
        'h2',
        {
            title: 'Học lập trình ReactJs tại F8',
        },
        'Học ReactJs'
    ),
    React.createElement('p', null, 'Học ReactJs từ cơ bản tới nâng cao')
);
```

<span style="color:yellow">**React-DOM**</span>

-   Lưu ý: thằng cu react-DOM này chỉ sử dụng được khi có react
    => cần import file reactDom sau khi nhúng được react nha
-   Sau khi cài đặt thành công thì sẽ có một biến là ReactDOM (console.log ra mà xem!)

```html
<!-- react -->
<script
    src="https://unpkg.com/react@17/umd/react.development.js"
    crossorigin
></script>
<!-- react-DOM -->
<script
    src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"
    crossorigin
></script>
```

1. Tại sao phải sử dụng reactDOM?

-   Để render React element ra trình duyệt
-   React dom là một thư viện là cầu nối giữa react và dom

2. Tại sao lại tách react-DOM ra?

-   Vì có nhiều thư viện khác như react-Native, ...
    => tách ra làm cầu nối giữa react và thư viện đó cho tinh gọn

3. Render UI

```javascript
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Document</title>
        <script
            src="https://unpkg.com/react@17/umd/react.development.js"
            crossorigin
        ></script>
        <script
            src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"
            crossorigin
        ></script>
    </head>
    <body>
        <div id="root"></div>
        <script>
            const divReact = React.createElement(
                'div',
                {
                    className: 'post-item',
                },
                React.createElement(
                    'h2',
                    {
                        title: 'Học lập trình ReactJs tại F8',
                    },
                    'Học ReactJs'
                ),
                React.createElement(
                    'p',
                    null,
                    'Học ReactJs từ cơ bản tới nâng cao'
                )
            );
            const root = document.querySelector('#root');
            ReactDOM.render(divReact, root);
        </script>
    </body>
</html>
```

<span style="color:yellow">**JSX là gì?**</span>

-   JSX: Javacript XML
    -   (XML là cú pháp thể hiện ở thẻ mở hoặc thẻ đóng, html là cú pháp mở rộng của XML) hay nói khác html cũng là XML thôi
    -   XML ra đời để hỗ trọ viết html trong javascript
-   JSX không thể truyền thẳng cho ReactDOM được vì ReactDOM cần nhận vào một react
-   JSX không phải là html, cần có javascript
-   Cần có Javacript, Babel để dùng JSX
-   Babel (sủ dụng để chuyển đổi các cú pháp của javacript es6 trở lên trở thành es5 nhằm hỗ trợ hầu hết trình duyệt có thể chạy được dự án của bạn )
-   Link demo: [Babel](http://bit.ly/2VOIMN7)
-   Nhúng babel:

```html
<script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
```

-   Tác dụng của babel:
    -   Ví dụ:

```javascript
const ul = (
	<ul>
    	<li>Trần Tuấn Đạt</li>
  	</ul>
)
<!-- babel -->
"use strict";

const ul = /*#__PURE__*/React.createElement("ul", null, /*#__PURE__*/React.createElement("li", null, "Tr\u1EA7n Tu\u1EA5n \u0110\u1EA1t"));
```

-   Sau khi add babel vào file, chúng ta vẫn chưa thể viết cú pháp jsx vì code vẫn sẽ thực thi javascript
    => Để ngăn chặn điều này chúng ta sẽ thêm một tag type="text/babel" vào javascript như sau

```html
<script type="text/babel">
```

-   Trong JSX để thực thi một javascript chúng ta sẽ chèn thêm cặp ngoặc {} vào, và javasript sẽ được viết bên trong {}
-   Ví dụ full:

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Document</title>
        <script
            src="https://unpkg.com/react@17/umd/react.development.js"
            crossorigin
        ></script>
        <script
            src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"
            crossorigin
        ></script>
        <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    </head>
    <body>
        <div id="root"></div>
        <script type="text/babel">
            const root = document.getElementById('root');
            const courses = [
                { name: 'HTML/CSS' },
                { name: 'Javascript' },
                { name: 'ReactJs' },
                { name: 'NodeJS' },
            ];
            const ulReact = (
                <ul>
                    {courses.map((course, index) => (
                        <li key={index}>{course.name}</li>
                    ))}
                </ul>
            );
            ReactDOM.render(ulReact, root);
        </script>
    </body>
</html>
```

<span style="color:yellow">**JSX render Array**</span>

-   Nhắc lại kiến thức:
    -   Thằng cu childrens nếu có >= 2 phần tử thì nó sẽ là một mảng chứa nhiều children
    -   Khi sử dụng map ta không phải join như khi code thuần javascript do:
        -   thằng javascript thuần cần innerHTML một chuỗi
        -   thằng react cần một mảng children để render:
-   Ví dụ:

```javascript
{
    courses.map((course, index) => <li key={index}>{course.name}</li>);
}
// Đoạn code trên tương ứng với code:
{
    courses.map((course, index) =>
        React.createElement('li', null, course.name)
    );
}
```

-   Chúng ta không thể tạo ra hoặc render cùng lúc 2 element !
    -   ví dụ:

```html
<!-- Failed -->
const ulReact = (
<li>HIHI</li>
<li>haha</li>
)
<!-- Chúng ta cần một thẻ wrap nó lại:
OK -->
<script type="text/babel">
    const root = document.getElementById('root');
    const ulReact = (
        <ul>
            <li>HIHI</li>
            <li>haha</li>
        </ul>
    );
    ReactDOM.render(ulReact, root);
</script>
<!-- Tuy nhiên, trong trường hợp thẻ wrap không phải là một ul thì ta sẽ cần chọn một thẻ div hay thẻ nào đó để gói nó lại
=> Nó sẽ xuất hiện thẻ wrap mà chúng ta không mong muốn
=> Thằng react nó có một conponent để giải quyết vấn đề này đó là: React.Fragment-->
<!-- Fix -->
<script type="text/babel">
    const root = document.getElementById('root');
    const ulReact = (
        <React.Fragment>
            <span>HIHI</span>
            <span>HIHI</span>
        </React.Fragment>
    );
    ReactDOM.render(ulReact, root);
</script>
<!-- Viết theo kiểu React.createElement -->
<script type="text/babel">
    const root = document.getElementById('root');
    const ulReact = React.createElement(
        React.Fragment,
        null,
        React.createElement('h1', null, 'haha'),
        React.createElement('h1', null, 'hihi')
    );
    ReactDOM.render(ulReact, root);
</script>
```

<span style="color:yellow">**React element types**</span>

-   Ta có React.createElement(type, props, childrens);
-   React elemenet types có thể nhận: string, function/class
-   Khi một hàm được sử dụng làm component thì tên của nó phải được bắt đầu bằng chữ cái in hoa(quy tắc PascalCase)
-   Ta xem ví dụ sau:

```javascript
<div id="root"></div>
<script type="text/babel">
    function PostItem(props) {
        const { name } = props;
        return (
            <div>
                <h3>Name</h3>
                <img
                    style={{ width: '200px', height: '350px' }}
                    src="https://i.pinimg.com/564x/3b/7e/53/3b7e538bcdd59ac121761d62aba160b8.jpg"
                    alt=""
                />
                <p>{name}</p>
            </div>
        );
    }
    function App() {
        return (
            <div id="wrapper">
                <PostItem name="Lisa" />
                <PostItem name="Jenni" />
                <PostItem name="rose" />
            </div>
        );
    }
    ReactDOM.render(<App />, root);
</script>
```

<span style="color:yellow">**Props là gì? Dùng khi nào?**</span>

-   Nó là một object, nó chứa những thuộc tính để chúng ta có thể miêu tẩ cho react element

### Props

-   React elements
    -   Sử dụng props giống như với attrubute của các thẻ element
    -   2 props class, for được chuyển thành className, htmlFor
    -   Phải tuân theo quy ước có sẵn
-   React components
    -   Sử dụng props giống như đối số cho component
    -   Tự do đặt tên cho props
        -   Đặt theo quy tắc camelCase
        -   Có thể bao gồm dấu gạch ngang (không nên dùng)
-   Chú ý:

    -   Prop key là một prop đặc biệt (không được đặt tên prop là key trừ khi nó đang dùng trong mảng)
    -   Props cơ bản là đối số của component
        => Prop có thể là bất kì kiểu dữ liệu gì
    -   Sủ dụng destructering

-   Ví dụ:

```javascript
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Document</title>
        <script
            src="https://unpkg.com/react@17/umd/react.development.js"
            crossorigin
        ></script>
        <script
            src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"
            crossorigin
        ></script>
        <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    </head>
    <body>
        <div id="root"></div>
        <script type="text/babel">
            // PostItem là mọt react component
            function PostItem(props) {
                // Nếu không dùng cú pháp dưới đây thì có thể truy cập như trong mọt object bằng cách props.img chẳng hạn
                const { name, img, callBack } = props;
                callBack(Math.random());
                return (
                    // bên dưới là react element
                    <div>
                        <h3>Name</h3>
                        <img
                            style={{ width: '200px', height: '350px' }}
                            src={img}
                            alt=""
                        />
                        <p>{name}</p>
                    </div>
                );
            }
            // App là một react component
            function App() {
                // return về một cái gọi là react element
                return (
                    <div id="wrapper">
                        khi click vào label email thì tự nhiên input được
                        focus(2 dòng code dưới sẽ thực hiện điều đó)
                        <label htmlFor="input">email</label>
                        <input type="text" id="input" />
                        <PostItem
                            name="Lisa"
                            img="https://i.pinimg.com/236x/2a/a7/4d/2aa74d47265dd4d150ebf404a96c773f.jpg"
                            callBack={(number) => {
                                console.log(number);
                            }}
                        />
                        <PostItem
                            name="Jenni"
                            img="https://i.pinimg.com/236x/eb/6f/37/eb6f37a25377363020efdd54916cf752.jpg"
                            callBack={(number) => {
                                console.log(number);
                            }}
                        />
                        <PostItem
                            name="rose"
                            img="https://i.pinimg.com/236x/7a/85/80/7a8580bcae9b1a0cffe09d00810469a0.jpg"
                            callBack={(number) => {
                                console.log(number);
                            }}
                        />
                    </div>
                );
            }
            ReactDOM.render(<App />, root);
        </script>
    </body>
</html>
```

Bài tập:

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Document</title>
        <script
            src="https://unpkg.com/react@17/umd/react.development.js"
            crossorigin
        ></script>
        <script
            src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"
            crossorigin
        ></script>
        <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    </head>
    <body>
        <div id="root"></div>
        <script type="text/babel">
            const courses = [
                {
                    id: 2,
                    category_id: 2,
                    title: 'HTML, CSS từ Zero đến Hero',
                    slug: 'html-css',
                    description:
                        'Trong khóa này chúng ta sẽ cùng nhau xây dựng giao diện 2 trang web là The Band & Shopee.',
                    thumbnail: 'courses/2.png',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: 'R6plN3FvzFY',
                    preview_path: null,
                    language: 'html',
                    syntax_highligh: 'language-html',
                    level: 'Trình độ cơ bản',
                    priority: 10,
                    students_count: 58776,
                    created_at: '2020-04-10T14:23:13.000000Z',
                    updated_at: '2021-10-08T17:01:35.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/2.png',
                },
                {
                    id: 1,
                    category_id: 1,
                    title: 'Javascript Cơ Bản',
                    slug: 'javascript-co-ban',
                    description:
                        'Học Javascript cơ bản phù hợp cho người chưa từng học lập trình. Với hơn 100 bài học và có bài tập thực hành sau mỗi bài học.',
                    thumbnail: 'courses/1.png',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: '0SJE9dYdpps',
                    preview_path: null,
                    language: 'javascript',
                    syntax_highligh: 'language-javascript',
                    level: 'Trình độ cơ bản',
                    priority: 30,
                    students_count: 38202,
                    created_at: '2020-06-10T14:23:13.000000Z',
                    updated_at: '2021-10-08T17:05:35.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/1.png',
                },
                {
                    id: 7,
                    category_id: 4,
                    title: 'Kiến Thức Nhập Môn',
                    slug: 'lessons-for-newbie',
                    description:
                        'Để có cái nhìn tổng quan về ngành IT - Lập trình web các bạn nên xem các videos tại khóa này trước nhé.',
                    thumbnail: 'courses/7.png',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: 'M62l1xA5Eu8',
                    preview_path: null,
                    language: null,
                    syntax_highligh: null,
                    level: 'Trình độ cơ bản',
                    priority: 0,
                    students_count: 33303,
                    created_at: '2020-02-10T14:23:13.000000Z',
                    updated_at: '2021-10-08T17:00:45.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/7.png',
                },
                {
                    id: 3,
                    category_id: 2,
                    title: 'Responsive Với Grid System',
                    slug: 'responsive-web-design',
                    description:
                        'Trong khóa này chúng ta sẽ học về cách xây dựng giao diện web responsive với Grid System, tương tự Bootstrap 4.',
                    thumbnail: 'courses/3.png',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: 'uz5LIP85J5Y',
                    preview_path: null,
                    language: 'html',
                    syntax_highligh: 'language-html',
                    level: 'Trình độ cơ bản',
                    priority: 20,
                    students_count: 13423,
                    created_at: '2020-05-10T14:23:13.000000Z',
                    updated_at: '2021-10-08T16:30:11.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/3.png',
                },
                {
                    id: 6,
                    category_id: 3,
                    title: 'Node & ExpressJS',
                    slug: 'nodejs',
                    description:
                        'Học Back-end với Node & ExpressJS framework, hiểu các khái niệm khi làm Back-end và xây dựng RESTful API cho trang web.',
                    thumbnail: 'courses/6.png',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: 'z2f7RHgvddc',
                    preview_path: null,
                    language: 'javascript',
                    syntax_highligh: 'language-javascript',
                    level: 'Trình độ cơ bản',
                    priority: 32,
                    students_count: 11253,
                    created_at: '2020-08-01T14:23:13.000000Z',
                    updated_at: '2021-10-08T16:32:25.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/6.png',
                },
                {
                    id: 5,
                    category_id: 2,
                    title: 'HTML, CSS Tips & Tricks',
                    slug: 'html-css-tutorials',
                    description:
                        'Tutorials về HTML, CSS, UI, UX sẽ được tổng hợp tại khóa học này, các video có nội dung ngắn gọn, súc tích giúp học viên có thể ứng dụng ngay vào thực tế',
                    thumbnail: 'courses/5.png',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: 'nB6cJh_bb1U',
                    preview_path: null,
                    language: 'html',
                    syntax_highligh: 'language-html',
                    level: 'Trình độ cơ bản',
                    priority: 40,
                    students_count: 8500,
                    created_at: '2020-03-10T14:23:13.000000Z',
                    updated_at: '2021-10-08T16:59:21.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/5.png',
                },
                {
                    id: 12,
                    category_id: 1,
                    title: 'Javascript Nâng Cao',
                    slug: 'javascript-nang-cao',
                    description:
                        'Hiểu sâu hơn về cách Javascript hoạt động, tìm hiểu về IIFE, closure, reference types, this keyword, bind, call, apply, prototype, ...',
                    thumbnail: 'courses/12.png',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: 'MGhw6XliFgo',
                    preview_path: null,
                    language: 'javascript',
                    syntax_highligh: 'language-javascript',
                    level: 'Trình độ nâng cao',
                    priority: 31,
                    students_count: 6894,
                    created_at: '2021-04-03T14:23:13.000000Z',
                    updated_at: '2021-10-08T17:01:52.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/12.png',
                },
                {
                    id: 13,
                    category_id: 0,
                    title: 'ReactJS',
                    slug: 'reactjs',
                    description:
                        'Khóa học ReactJS từ cơ bản tới nâng cao, kết quả của khóa học này là bạn có thể làm hầu hết các dự án thường gặp với ReactJS. Cuối khóa học này bạn sẽ sở hữu một dự án giống Tiktok.com, bạn có thể tự tin đi xin việc khi nắm chắc các kiến thức được chia sẻ trong khóa học này.',
                    thumbnail: 'courses/13/13.png',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: 'x0fSBAgBrOQ',
                    preview_path: null,
                    language: 'javascript',
                    syntax_highligh: 'language-jsx',
                    level: 'Trình độ trung bình',
                    priority: 0,
                    students_count: 4867,
                    created_at: null,
                    updated_at: '2021-10-08T17:02:32.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/13/13.png',
                },
                {
                    id: 4,
                    category_id: 1,
                    title: "Don't Touch Your Face",
                    slug: 'tool-canh-bao-so-len-mat',
                    description:
                        'Xây dựng ứng dụng đưa ra cảnh báo khi người dùng sờ tay lên mặt. Chúng ta sẽ sử dụng thư viện ReactJS & Tensoflow để hoàn thiện ứng dụng này.',
                    thumbnail: 'courses/4/4.jpeg',
                    content: null,
                    preview_origin: 'youtube',
                    preview_youtube_id: 'r6GWbQL-qwA',
                    preview_path: null,
                    language: 'javascript',
                    syntax_highligh: 'language-javascript',
                    level: 'Trình độ cơ bản',
                    priority: 50,
                    students_count: 3264,
                    created_at: '2020-01-10T14:23:13.000000Z',
                    updated_at: '2021-10-08T15:54:25.000000Z',
                    thumbnail_cdn:
                        'https://cdn.fullstack.edu.vn/f8-learning/courses/4/4.jpeg',
                },
            ];
            function CouseItem({
                title,
                students_count,
                description,
                language,
            }) {
                return (
                    <li>
                        <h3>{title}</h3>
                        <p>{description}</p>
                        <p>{students_count}</p>
                        <p>{language}</p>
                    </li>
                );
            }
            function App() {
                return courses.map((course, index) => (
                    <CouseItem
                        key={index}
                        title={course.title}
                        students_count={course.students_count}
                        language={course.language}
                        description={course.description}
                    />
                ));
            }
            ReactDOM.render(<App />, root);
        </script>
    </body>
</html>
```

<span style="color:yellow">**DOM events**</span>

-   Lưu ý về props + Khi props quá nhiều thì ta truyền thẳng vào props một object
    Ví dụ:
-   Phần 1:
    -   Xử lí DOM event
    -   Component do chúng ta định nghĩa phải in hoa kí tự đầu
    -   Chọn component trong một object
    -   Boolean, null, underfined sẽ không được render
    -   Kết hợp toán tử logic để render theo điều kiện

```html
<script type="text/babel">
    const courses = [
        {
            name: 'javascript',
            id: 1,
            price: 100,
        },
        {
            name: 'reactJs',
            id: 2,
            age: 1111,
        },
        {
            name: 'Html/css',
            id: 3,
            age: 1011,
        },
    ];
    function Item(props) {
        const { data } = props;
        const { name, id, age } = data;
        return <h3>{(name, id, age)}</h3>;
    }
    function App() {
        return courses.map((course) => <Item key={course.id} data={course} />);
    }
    ReactDOM.render(<App />, root);
</script>
```

Ví dụ về DOM event

```javascript
function App() {
    return (
        <button
            onClick={() => {
                console.log(Math.random());
            }}
        >
            click
        </button>
    );
}
```

-   Ví dụ một object chứa các function component

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Document</title>
        <script
            src="https://unpkg.com/react@17/umd/react.development.js"
            crossorigin
        ></script>
        <script
            src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"
            crossorigin
        ></script>
        <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    </head>
    <body>
        <div id="root"></div>
        <script type="text/babel">
            const Form = {
                // Viết thăng function trong một object theo cách viết của es6 khi key và value trùng tên
                Input() {
                    return <input type="text" />;
                },
                CheckBox() {
                    return <input type="Checkbox" />;
                },
            };
            console.log(Form);
            function App() {
                return <Form.Input />;
            }
            ReactDOM.render(<App />, root);
        </script>
    </body>
</html>
```

-   Tuy nhiên, khi một object chứa các function component thì chúng ta không cần viết hoa chữ cái đầu như sau:

```html
<script type="text/babel">
    const form = {
        // Viết thăng function trong một object theo cách viết của es6 khi key và value trùng tên
        input() {
            return <input type="text" />;
        },
        checkbox() {
            return <input type="Checkbox" />;
        },
    };
    function App() {
        return <form.input />;
    }
    ReactDOM.render(<App />, root);
</script>
```

=> Cách này không khuyến khích sử dụng do nó không tuân theo quy chuẩn của ông React, vì thế sẽ dễ gây nhầm lẫn khi làm việc với team

-   Render theo type được định nghĩa sẵn

```html
<!-- Failed do có dấu ngoặc vuông -->
<script type="text/babel">
    const Form = {
        // Viết thăng function trong một object theo cách viết của es6 khi key và value trùng tên
        Input() {
            return <input type="text" />;
        },
        CheckBox() {
            return <input type="Checkbox" />;
        },
    };
    function App() {
        const type = 'input'
        return <Form[type] />;
    }
    ReactDOM.render(<App />, root);
</script>
<!-- Fix -->
<script type="text/babel">
    const Form = {
        // Viết thăng function trong một object theo cách viết của es6 khi key và value trùng tên
        Input() {
            return <input type="text" />;
        },
        CheckBox() {
            return <input type="Checkbox" />;
        },
    };
    function App() {
        const type = 'Input';
        const MyComponent = Form[type];
        return <MyComponent />;
    }
    ReactDOM.render(<App />, root);
</script>
```

-   Tạo rả một component linh hoạt:

```html
<div id="root"></div>
<script type="text/babel">
    function Button({ title, href, onClick }) {
        // do return ra một thẻ có tên không giống với bất kì tên tag nào của thẻ html thế nên cần khai báo một biên có tên bắt đầu bằng một chữ cái in hoa, điều này giúp react hiểu là chúng ta đang return ra một component
        let Component = 'button';
        const props = {};
        if (title) {
            Component = 'h3';
            props.title = title;
        }
        if (href) {
            Component = 'a';
            props.href = href;
        }
        if (onClick) {
            props.onClick = onClick;
        }
        return <Component {...props}>{title}</Component>;
    }
    function App() {
        return (
            // Khi props của Button thay đổi thì ta có một component linh hoạt tương ứng
            <Button
                id="wraper"
                title="Click me"
                // href="https://fullstack.edu.vn/learning/reactjs?id=2739"
                // onClick={() => console.log(Math.random() * 100)}
            ></Button>
        );
    }
    ReactDOM.render(<App />, root);
</script>
```

-   Dùng toán tử logic render theo điều kiện

```html
<!-- Toán tử or -->
<script type="text/babel">
    function App({ contentFirst, contentFinal }) {
        return <div>{contentFirst || contentFinal}</div>;
    }
    ReactDOM.render(<App contentFinal="welcome to comback" />, root);
</script>

<!-- Toán tử && -->
<script type="text/babel">
    function App({ content }) {
        let firstAccess = true;
        return <div>{firstAccess && content}</div>;
    }
    ReactDOM.render(<App content="welcome to F8" />, root);
</script>
```

<span style="color:yellow">**Chilren Props, Render Props**</span>

Phần 2: - Bất kì function nào cũng có thể trở thành function component (nhưng tên của nó phải viết hoa chữ cái đầu, trừ khi function đó nằm trong một object) - Props trong JSX

```html
<script type="text/babel">
    <YourCompoent props1={expression} props2="String literal" />
    // - Props default to true
    // - spread/rest props
    // - Children props
    <YourCompoent>String literal</YourCompoent>
    <YourCompoent>{expression}</YourCompoent>
    // - Render props
    ReactDOM.render(<App />, root);
</script>
```

-   Expressioin là một biểu thức, thế nhưng ta không thể viêt câu lệnh if else hay switch case vào nó được, có thể truyền cho nó một object, array, string, ...

```html
<script type="text/babel">
    function Button({ isPrimery }) {
        console.log(isPrimery); // true;
        return <button>hehe</button>;
    }
    function App() {
        // truyền một props như này thì có giá trị là true
        return <Button isPrimery />;
    }
    ReactDOM.render(<App />, document.getElementById('root'));
</script>

<!--Chỉ truyền vào một boolean nếu nó là false hoặc phụ thuộc vào biến khác  -->
<script type="text/babel">
    function Button({ isPrimery }) {
        console.log(isPrimery);
        return <button>hehe</button>;
    }
    function App() {
        const isClick = true;
        // truyền một props như này thì có giá trị là true
        return <Button isPrimery={isClick} />;
    }
    ReactDOM.render(<App />, document.getElementById('root'));
</script>
```

-   Spread/rest props

```html
<!-- Trong trường hợp không có spread -->
<script type="text/babel">
    function Form({ label, type, placeholder, required }) {
        return (
            <React.Fragment>
                <form action="">
                    <label htmlFor="">{label}</label>
                    <input
                        type={type}
                        placeholder={placeholder}
                        label={label}
                        required
                    />
                </form>
            </React.Fragment>
        );
    }
    function App() {
        return (
            <Form
                label="email"
                placeholder="enter email address"
                type="text"
                required
            />
        );
    }
    ReactDOM.render(<App />, document.getElementById('root'));
</script>

<!-- Có spead và toán tử rest -->
<script type="text/babel">
    function Form({ label, ...inputProps }) {
        return (
            <React.Fragment>
                <form action="">
                    <label htmlFor="">{label}</label>
                    <input {...inputProps} />
                </form>
            </React.Fragment>
        );
    }
    function App() {
        return (
            <Form
                label="email"
                placeholder="enter email address"
                type="text"
                required
            />
        );
    }
    ReactDOM.render(<App />, document.getElementById('root'));
</script>

<!-- Object -->
<script type="text/babel">
    function Form({ myProps }) {
        const { label, ...inputProps } = myProps;
        return (
            <React.Fragment>
                <form action="">
                    <label htmlFor="">{label}</label>
                    <input {...inputProps} />
                </form>
            </React.Fragment>
        );
    }
    function App() {
        return (
            <Form
                myProps={{
                    label: 'email',
                    placeholder: 'enter email address',
                    type: 'text',
                    required: true,
                }}
            />
        );
    }
    ReactDOM.render(<App />, document.getElementById('root'));
</script>
```

-   Children Props

```html
<!-- Kiểu String literal -->
<script type="text/babel">
    function Button({ children }) {
        return <button>{children}</button>;
    }
    function App() {
        return <Button>Click me!</Button>;
    }
    ReactDOM.render(<App />, document.getElementById('root'));
</script>

<!-- Kiểu expression -->
< type="text/babel">
    function Button({ children }) {
        return <button>{children}</button>;
    }
    function App() {
        return <Button>{'I love you so much'}</Button>;
    }
    ReactDOM.render(<App />, document.getElementById('root'));
</script>
```

-   Render Props

```js
< type="text/babel">
    function List({ data, children }) {
        return (
            <ul>{data.map((item, index) => children(item, index))}</ul>
            // Trong trường hợp có nhiều tham số truyền vào thì:
            // <ul>{data.map((...props) => children(...props))}</ul>
            // Thằng cu map nhận vào một function, mà thằng children cũng là một function
            // vì thế ta có thể làm như sau:
            // <ul>{data.map(children)}</ul>
        );
    }
    function App() {
        const courses = ['ReactJs', 'Javascript', 'html/css'];
        return (
            <List data={courses}>
                {(item, index) => <li key={index}>{item}</li>}
            </List>
        );
    }
    ReactDOM.render(<App />, document.getElementById('root'));
</script>
```

<span style="color:yellow">**NodeJs là gì? Tại sao phải sử dụng nodeJs**</span>

-   Nodejs là mọt javascript runtime
-   Khi cài thì nó tạo ra một môi trường độc lập giúp thực hiện code javascript
-   NodeJs giúp tạo ra một web server
-   Khi cài nodeJs thì nó sẽ tự cài thêm npm
-   webpack là một thư viện giúp ta có thể chia ra nhỏ file
-   Tải nodeJs - Nhớ tắt trình biên dịch trước khi download để đỡ phải re-open APP

<span style="color:yellow">**Tạo dự án với React-Webpack**</span>

-   Giúp chúng ta module hóa ứng dựng frontend
-   mini hóa file giúp file nhẹ hơn
-   ...
    Xem ví dụ trong blog...

<span style="color:yellow">**Create React App**</span>

-   ./: Ngang cấp

<span style="color:yellow">**npm, npx, yarn**</span>

-   Npm

    -   Phạm vi cài đặt:(project scope || global scope)

        -   project scope (Cài thư viện vào một dự án cụ thể)

            -   Cài đặt

                -   npm install react react-dom => dependencies
                -   npm i react react-dom (shorthand) => dependencies

                -   npm i -D react react-dom => devDependencies
                -   npm install react react-dom => devDependencies

            -   Xóa thư viện khỏi một dự án
                -   npm uninstall react react-dom (nó tự kiểm tra, không cần chỉ định là xóa ở đâu, ví dụ như dependencies)

        -   global scope (Cài vào máy tính)
            -   Sử dụng khi dự án của ta không phụ thuộc vào thư viện đó
            -   Cú pháp: (lưu ý: với máy linux, unbuntu, macos thì cần thêm sudo vào đầu tiên của câu lệnh)
                -   Cài đặt:
                    -   npm i --global create-react-app
                    -   npm i --g create-react-app (shorthand)
                -   Gỡ:
                    -   npm uninstall -g create-react-app

-   Npx: Node => npm, npx

    -   Tại sao lại dùng? Không cần cài đặt thư viện lên máy của mình (nếu cài lên global mà không cập nhật phiên bản thì nó luôn luôn dùng phiên bản cũ đó nếu nó được cập nhật)

-   Yarn & npm - Nếu xóa một package trong dự án của mình thì cài lại bằng cách: npm i - npm khi cài nhiều thư viện cùng một lúc thì nó sẽ cài tuần tự - cơ chế cache của npm không tốt bằng yarn - Nhược điểm của yarn là tốn dung lượng vì nó cache nhiều dữ liệu - yarn khi cài nhiều thư viện một lúc thì nó có thể cài song song
    => ít dung lượng dùng npm, thừa dung lượng thì dùng yarn
-   Yarn install
    -   npm i -g yarn
-   Lưu ý: luôn bật development server (npm start || yarn start)

<span style="color:yellow">**CRA, Folder Structure**</span>

-   Từ trình duyệt của chúng ta có thể truy cập những file nằm trong thư mục public (đóng vai trò là thư mục gốc(root))
    => Nó truy cập vào file public => index.html
-   file gitinore loại bỏ một số file khi cho code lên git
-   khi push code lên git thì sẽ không có file node module , vì thế chúng ta sẽ không thể start được ứng dụng => fix: yarn, hoặc nếu dùng npm thì có thể gõ lệnh: npm i để kéo lại node module

<span style="color:yellow">**Hook là gì?**</span>

-   Hook nghĩa là "gắn"
-   Bản chất hook trong javascript là một cái hàm được cung cấp sẵn trong thư viện reactJs
-   Các hook cần biết:
    -   useState
    -   useEffect
    -   useLayoutEffeact
    -   useRef
    -   useCallback
    -   useMemo
    -   useReducer
    -   useContext
    -   useImperativeHandle
    -   useDebugValue
-   import hook từ react
-   Hook chỉ sử dụng trong function component
-   Component sẽ trở nên đơn giản và dễ hiểu hơn
    -   Không bị chia logic như lifecycle trong class component
    -   Không sử dụng this
-   Sử dụng hook khi nào?
    -   Dự án mới: hooks
    -   Dự án cũ:
        -   component mới => function component + hooks
        -   component cũ => Giữ nguyên, có thời gian thì tối ưu lại sau
    -   Logic nghiệp vụ cần sử dụng các tính năng của Opp => class component
    -   Có thể kết hợp sử dụng class component và function component
-   Người mới nên tiếp cận với function component

<span style="color:yellow">**useState**</span>

-   state (trạng thái) => Trạng thái của dữ liệu
-   Dữ liệu thay đổi gì, trạng thái thay đổi đó
-   Khi nào dùng useState?
    -   Khi muốn dữ liệu thay đổi thì giao diện tự động cập nhật lại (render lại theo dữ liệu)
-   Cú pháp:

```jsx
import { useState } from 'react';
function Component() {
    const [state, useState] = useState(initState);
}
```

-   Trong đó giá trị được truyền vào useState là init chỉ được dùng duy nhất trong lần đầu tiên render ra ngoài màn hình

-   Lưu ý:

    -   Component được render sau khi setState
    -   initial State chỉ được dùng khi render lần đầu
    -   setState với callback
    -   initialState với callback
    -   setState là thay thế state bằng giá trị mới

-   Ví dụ 1: app counter

```jsx
import { useState } from 'react';
function App() {
    const [counter, setNumber] = useState(1);
    const handleIncrease = () => {
        setNumber(counter + 1);
    };
    return (
        <div className="App">
            <button onClick={handleIncrease}>Increase</button>
            <p>{counter}</p>
        </div>
    );
}

export default App;
```

-   Giả sử ta làm như sau thì mỗi lần bấm chỉ tắng lên một giá trị chứ không phải là ba giá trị

```jsx
import { useState } from 'react';
function App() {
    const [counter, setNumber] = useState(1);
    const handleIncrease = () => {
        // Note
        setNumber(counter + 1);
        setNumber(counter + 1);
        setNumber(counter + 1);
    };
    return (
        <div className="App">
            <button onClick={handleIncrease}>Increase</button>
            <p>{counter}</p>
        </div>
    );
}

export default App;
```

-   Vậy làm như thế nào để tắng giá trị counter một phát 3 đơn vị?
    => Sử dụng callback

```jsx
import { useState } from 'react';
function App() {
    const [counter, setNumber] = useState(1);
    const handleIncrease = () => {
        setNumber((prevState) => prevState + 1);
        setNumber((prevState) => prevState + 1);
        setNumber((prevState) => prevState + 1);
    };
    return (
        <div className="App">
            <button onClick={handleIncrease}>Increase</button>
            <p>{counter}</p>
        </div>
    );
}

export default App;
```

-   initialState với callback

*   Ta thấy rằng: thằng initialState chỉ có tác dụng trong lần đầu tiên render, nếu ta truyền vào nó một kết quả cuối cùng nhưng kết quả này là do một quá trình tạo ra, vì thế không nên tách code của nó bên ngoài state mà nên cho vào nó mọt callback (sau khi state bị thay đổi thì app bị re-render)
*   Ví dụ như sau:

```jsx
// Bad
import { useState } from 'react'
function App() {
    const myCost = [12, 343, 235, 11, 134];
    const total = myCost.reduce((acc, cost) => {
        return acc + cost;
    })
    const [number, setNumber] = useState(total);
    const handleBtnClick = () => {
        setNumber((prevState) => prevState + 1);
    }
    return (
        <div className="App">
            <button onClick={handleBtnClick}>Show total</button>
            <p>{number}</p>
        </div>
    );
}

export default App;

// Good
import { useState } from 'react'
function App() {
    const myCost = [12, 343, 235, 11, 134];
    const [number, setNumber] = useState(myCost.reduce((acc, cost) => {
        return acc + cost;
    }));
    const handleBtnClick = () => {
        setNumber((prevState) => prevState + 1);
    }
    return (
        <div className="App">
            <button onClick={handleBtnClick}>Show total</button>
            <p>{number}</p>
        </div>
    );
}

export default App;
```

-   setState là thay thế state bằng giá trị mới chứ không phải là muli vào state (chèn)

*   Ví dụ:

```jsx
import { useState } from 'react'
function App() {
    const [info, setInfo] = useState({
        name: "tran tuan dat",
        age: 19
    })
    const handleBtnClick = () => {
        setInfo({
            adress: 'ha nam',
        })
    }
    return (
        <div className="App">
            <button onClick={handleBtnClick}>Show total</button>
            <p>{JSON.stringify(info)}</p>
        </div>
    );
}

export default App;
// Muốn thêm key vào trong một array hoặc object thì chúng ta cần clone nó ra một object hoặc arrat mới do vấn đề tham chiếu
// Fix:
import { useState } from 'react'
function App() {
    const [info, setInfo] = useState({
        name: "tran tuan dat",
        age: 19
    })
    const handleBtnClick = () => {

        setInfo({
            ...info,
            adress: 'ha nam',
        })
    }
    return (
        <div className="App">
            <button onClick={handleBtnClick}>Show total</button>
            <p>{JSON.stringify(info)}</p>
        </div>
    );
}

export default App;
// Hoặc sử dụng callback khi có sử dụng thêm logic
import { useState } from 'react'
function App() {
    const [info, setInfo] = useState({
        name: "tran tuan dat",
        age: 19
    })
    const handleBtnClick = () => {

        setInfo((prev) => {
            // logic...
            return {
                ...prev,
                adress: 'ha nam'
            }
        })
    }
    return (
        <div className="App">
            <button onClick={handleBtnClick}>Show total</button>
            <p>{JSON.stringify(info)}</p>
        </div>
    );
}

export default App;

```

<span style="color:yellow">**To-way binding**</span>

-   One-way binding: Ràng buộc một chiều (ReactJs)
    -   Khi tương tác với giao diện thì có thể dữ liệu bên trong app bị thay đổi
    -   Ví dụ:

```jsx
import { useState } from 'react';
function App() {
    const [name, setName] = useState('');
    const handleOnChange = (e) => {
        setName(e.target.value);
    };
    return (
        <div className="App">
            <input onChange={handleOnChange} type="text" />
            {/* giao diện bên ngoài không bị thay đổi khi thay dữ liệu trong component*/}
            <button
                onClick={() => {
                    setName('lú luôn');
                }}
            >
                Change
            </button>
        </div>
    );
}
export default App;
```

-   Two way binding: Ràng buộc hai chiều (VueJs)
    -   Sửa dữ liệu ở trong component mà giao diện cũng thay đổi theo
    -   Khi tương tác với giao diện thì có thể dữ liệu bên trong app bị thay đổi
    -   Ví dụ:

```jsx
import { useState } from 'react';
function App() {
    const [name, setName] = useState('');
    const handleOnChange = (e) => {
        setName(e.target.value);
    };
    return (
        <div className="App">
            <input onChange={handleOnChange} type="text" value={name} />
            {/* giao diện bên ngoài bị thay đổi khi thay dữ liệu trong component*/}
            <button
                onClick={() => {
                    setName('lú luôn');
                }}
            >
                Change
            </button>
        </div>
    );
}
export default App;
```

-   Ví dụ app get gift

```jsx
import { useState } from 'react';
function App() {
    const gifts = [
        'Iphone XS Max',
        'Xiaomi Mi 11 Pro',
        'SamSung Flip',
        'mesedes',
    ];
    const [gift, setGift] = useState('');
    const randomGift = () => {
        const indexGiftRandom = Math.trunc(Math.random() * gifts.length);
        return gifts[indexGiftRandom];
    };
    const handleClickBtn = () => {
        const newGift = randomGift();
        setGift(newGift);
    };
    return (
        <div className="App">
            <h3>{gift || 'Chưa có phần thưởng'}</h3>
            <button onClick={handleClickBtn}>Lấy thưởng</button>
        </div>
    );
}

export default App;
```

-   Ví dụ get value from

```jsx
import { useState } from 'react';
function App() {
    const [name, setName] = useState('');
    const [email, setEmail] = useState('');
    const handleOnChange = (e) => {
        setName(e.target.value);
    };
    const handleOnSubmit = () => {
        console.log({
            name,
            email,
        });
    };
    return (
        <div className="App">
            <input onChange={handleOnChange} type="text" />
            <br />
            <input onChange={handleOnChange} type="text" />
            {/* giao diện bên ngoài không bị thay đổi khi thay dữ liệu trong component*/}
            <button onClick={handleOnSubmit}>Change</button>
        </div>
    );
}
export default App;
```

-   Two binding với radio box

```jsx
import { useState } from 'react';
const courses = [
    {
        id: 1,
        name: 'Html/ css',
    },
    {
        id: 2,
        name: 'Javascript',
    },
    {
        id: 3,
        name: 'ReactJs',
    },
];
function App() {
    const [checked, setChecked] = useState(1);
    const handleOnChange = (idCourse) => {
        setChecked(idCourse);
    };
    const handOnSubmit = () => {
        console.log({ id: checked });
    };
    return (
        <div className="App">
            {courses.map((course) => (
                <div key={course.id}>
                    <input
                        type="radio"
                        onChange={() => handleOnChange(course.id)}
                        checked={checked === course.id}
                    />
                    {course.name}
                </div>
            ))}
            <button onClick={handOnSubmit}>Submit</button>
        </div>
    );
}
export default App;
```

-   Xử lí với checkbox

```jsx
import { useState } from 'react';
const courses = [
    {
        id: 1,
        name: 'Html/ css',
    },
    {
        id: 2,
        name: 'Javascript',
    },
    {
        id: 3,
        name: 'ReactJs',
    },
];
function App() {
    const [checked, setChecked] = useState([]);
    const handleCheck = (idCourse) => {
        const isChecked = checked.includes(idCourse);
        setChecked((prev) => {
            if (isChecked) {
                return checked.filter((id) => id !== idCourse);
            } else {
                return [...prev, idCourse];
            }
        });
    };
    const handOnSubmit = () => {
        console.log(checked);
    };
    return (
        <div className="App">
            {courses.map((course) => (
                <div key={course.id}>
                    <input
                        type="checkbox"
                        onChange={() => handleCheck(course.id)}
                        checked={checked.includes(course.id)}
                    />
                    {course.name}
                </div>
            ))}
            <button onClick={handOnSubmit}>Submit</button>
        </div>
    );
}
export default App;
```

-   Trong trường hợp hàm include được sử dụng nhiều lần thì ta có thể tách riêng nó ra như sau để có thể tái sử dụng:

```jsx
import { useState } from 'react';
const courses = [
    {
        id: 1,
        name: 'Html/ Css',
    },
    {
        id: 2,
        name: 'Javascript',
    },
    {
        id: 3,
        name: 'ReactJs',
    },
    {
        id: 4,
        name: 'NodeJs',
    },
    {
        id: 5,
        name: 'React Native',
    },
];
function App() {
    const [listChecked, setListChecked] = useState([1]);
    const handleChange = (idCourse) => {
        setListChecked((prev) => {
            if (checkInclude(idCourse)) {
                return listChecked.filter((id) => id !== idCourse);
            } else {
                return [...listChecked, idCourse];
            }
        });
    };
    const handleSubmmit = () => {
        console.log(listChecked);
    };
    const checkInclude = (id) => {
        return listChecked.includes(id);
    };
    return (
        <div>
            {courses.map((course) => (
                <div key={course.id}>
                    <input
                        onChange={() => handleChange(course.id)}
                        type="checkbox"
                        checked={checkInclude(course.id)}
                    />
                    {course.name}
                </div>
            ))}
            <button onClick={handleSubmmit}>Done</button>
        </div>
    );
}
export default App;
```

-   Giải thích lí do phải truyền callback vào một sự kiện khi có tham số:
    -   Ví dụ

```jsx
<input
  type="radio"
  onChange={() => handleOnChange(course.id)}
  checked={checked === course.id}
/>
// ta có mỗi khi input thay đổi thì hàm bên trong nó sẽ được gọi (callback), khi hàm bên trong được gọi thì nó sẽ gọi tiếp một hàm là handleOnChange
  onChange={handleOnChange(course.id)}
  // Nếu làm như bên trên thì handleOnChange luôn được thực hiện khi code chạy qua phần này mà không cần phải lắng nghe sự kiện onChange
  onChange={handleOnChange(course.id)}
  => Lỗi do phải re-render mấy lần vì hàm gọi liên tục
  onChange={handleOnChange}
  => Hàm được gọi khi sự kiện onChange được thực thi
```

=> Nói tóm lại, khi ta sửa dữ liệu bên trên giao diện mà dữ liệu trong component(state) thay đổi </br>
theo thì đây được gọi là one way binding, Còn nếu ta thay đổi dữ liệu trên giao diện => Dữ liệu </br>
trong component thay đổi và khi sửa dữ liệu trong component => Giao diện thay đổi thì đây gọi là </br>
two way binding

-   Xây dựng app todolist

```jsx
import React, { useState } from 'react';

function App(props) {
    const [toDos, setToDos] = useState(() => {
        const storageList = JSON.parse(localStorage.getItem('TODOS'));
        // Toán tử nullest, khi vế trước là null hoặc underfied thì sẽ lấy vế sau
        return storageList ?? [];
    });
    const [value, setValue] = useState('');
    const handleClickSubmit = (e) => {
        if (!value) return;
        const newToDo = {
            id: toDos.length + 1000,
            name: value,
        };
        setToDos((prev) => {
            const newToDoList = [...prev, newToDo];
            localStorage.setItem('TODOS', JSON.stringify(newToDoList));
            return newToDoList;
        });
        setValue('');
    };
    return (
        <div>
            <input
                value={value}
                onChange={(e) => setValue(e.target.value)}
                type="text"
            />
            <button onClick={handleClickSubmit}>Add</button>
            <ul>
                {toDos.map((item) => (
                    <li key={item.id}> {item.name} </li>
                ))}
            </ul>
        </div>
    );
}

export default App;
```

-   Code hoàn thiện hơn ứng dụng todolist (Giới thiệu dùng useRef hook)

```jsx
import React, { useRef, useState } from 'react';

function App(props) {
    const [toDos, setToDos] = useState(() => {
        const storageList = JSON.parse(localStorage.getItem('TODOS'));
        // Toán tử nullest, khi vế trước là null hoặc underfied thì sẽ lấy vế sau
        return storageList ?? [];
    });
    const [value, setValue] = useState('');
    const inputElm = useRef(null);
    const handleClickSubmit = (e) => {
        if (!value) return;
        const newToDo = {
            id: randomId(),
            name: value,
        };
        setToDos((prev) => {
            const newToDoList = [...prev, newToDo];
            setLocalToDos(newToDoList);
            return newToDoList;
        });
        setValue('');
        inputElm.current.focus();
    };
    const handleClickToRemove = (id) => {
        const index = toDos.findIndex((item) => item.id === id);
        setToDos((prev) => {
            const newToDoList = [...prev];
            newToDoList.splice(index, 1);
            setLocalToDos(newToDoList);
            return newToDoList;
        });
    };
    const setLocalToDos = (data) => {
        localStorage.setItem('TODOS', JSON.stringify(data));
    };
    const randomId = () => {
        return Math.floor(Math.random() * 9999);
    };
    return (
        <div>
            <input
                value={value}
                onChange={(e) => setValue(e.target.value)}
                type="text"
                ref={inputElm}
            />
            <button onClick={handleClickSubmit}>Add</button>
            <ul>
                {toDos.map((item) => (
                    <li
                        style={{ cursor: 'pointer' }}
                        key={item.id}
                        onClick={() => handleClickToRemove(item.id)}
                    >
                        {item.name}
                    </li>
                ))}
            </ul>
        </div>
    );
}

export default App;
```

<span style="color:yellow">**Mounted (lắp vào) & Unmounted (tháo ra)**</span>

-   Ví dụ:

```jsx
// App.js
import React, { useState } from "react";
import Hello from "./Hello";

App.propTypes = {};

function App(props) {
  const [status, setStatus] = useState(false);
  return (
    <div>
      <button onClick={() => setStatus(!status)}>
        {status ? "Hide" : "Show"}
      </button>
      {status && <Hello />}
    </div>
  );
}

export default App;
// Hello.js
import React from "react";

Hello.propTypes = {};

function Hello(props) {
  return <h3>Hello anh em</h3>;
}

export default Hello;
```

<span style="color:yellow">**useEffect hook (react hook)**</span>

-   Sử dụng useEffect khi muốn thực hiện các side effects(là một thuật ngữ sử dụng chung trong lĩnh vực phầm mềm, không phải là thuật ngữ của react, side effects nghĩa là đang nói tới một chương trình phần mềm, khi có một tác động xảy ra, nó dẫn tới việc dữ liệu của chương trình bị thay đổi )

-   Cú pháp: useEffect(callback, [deps]); trong đó tham số truyền vào callback là bắt buộc(trong callback sẽ thực hiện các side effect như: update dom, call Api, listen dom event)

-   Các trường hợp thường gặp:

1. useEffect(callback);

-   Gọi callback mỗi khi component được re-render
-   Gọi callback khi element được thêm vào DOM (được render)

    -   Bản chất thằng useEffect nó vẫn được chạy trước nhưng nó sẽ cầm callback và đợi khi component được render ra thì nó mới gọi callback này
    -   Trong trường hợp một side effects phức tạp mà ta đặt nó trước component thì nó sẽ tốn thời gian chạy thằng side effects đó trước, sau đó mới render => ảnh hưởng tới UI

    => Cho nó vào useEffect thì khi component được render xong nó mới chạy cái side effects đó.

2. useEffect(callback, []);

-   Chỉ gọi callback một lần sau khi component mounted

3. useEffect(callback, [deps]);

-   callback sẽ được gọi lại mỗi khi deps thay đổi

*   Note
    -   callback luôn được gọi sau khi component được mounted
    -   clean up function luôn được gọi mỗi khi component unmounted
        Ví dụ:
        Change title
    -   Cleanup function luôn luôn được gọi trước khi callback (trong useEffect) được gọi (trừ lần mounted)
        => Khi despendence thay đổi thì nó sẽ cleanup cái cũ đi và thực hiện callback

```jsx
// App.js
import React, { useState } from "react";
import Hello from "./Hello";
function App(props) {
  const [status, setStatus] = useState(false);
  return (
    <div>
      <button onClick={() => setStatus(!status)}>
        {status ? "Hide" : "Show"}
      </button>
      {status && <Hello />}
    </div>
  );
}

export default App;

// Hello.js
import React, { useState } from "react";
import { useEffect } from "react";

function Hello(props) {
  const [value, setValue] = useState("");
  useEffect(() => {
    document.title = value;
  });
  return (
    <div>
      <input
        value={value}
        type="text"
        onChange={(e) => setValue(e.target.value)}
      />
      <h3>Hello anh em</h3>
    </div>
  );
}

export default Hello;

```

-   Call API
    -   dùng api từ trang json place holder
-   Ví dụ sử dụng useEffect với dependencies

```jsx
// App.js
import React, { useState } from "react";
import { useEffect } from "react";
import Hello from "./Hello";
const tabs = ["comments", "users", "albums"];
function App(props) {
  const [status, setStatus] = useState(false);
  const [datas, setDatas] = useState([]);
  const [data, setData] = useState("comments");
  useEffect(() => {
    fetch(`https://jsonplaceholder.typicode.com/${data}`)
      .then((res) => res.json())
      .then((commentsList) => {
        setDatas(commentsList);
      });
  }, [data]);
  const handleTabClick = (tab) => {
    setData(tab);
  };
  return (
    <div>
      <button onClick={() => setStatus(!status)}>
        {status ? "Hide" : "Show"}
      </button>
      {status && <Hello />}
      {tabs.map((tab) => (
        <button
          style={data === tab ? { color: "red" } : {}}
          onClick={() => handleTabClick(tab)}
          key={tab}
        >
          {tab}
        </button>
      ))}
      <ul>
        {datas.map((data) => (
          <li key={data.id}>{data.name || data.title}</li>
        ))}
      </ul>
    </div>
  );
}

export default App;

// Hello.js
import React, { useState } from "react";
import { useEffect } from "react";

function Hello(props) {
  const [value, setValue] = useState("");
  useEffect(() => {
    document.title = value;
  });
  return (
    <div>
      <input
        value={value}
        type="text"
        onChange={(e) => setValue(e.target.value)}
      />
      <h3>Hello anh em</h3>
    </div>
  );
}

export default Hello;
```

Ví dụ: chức năng go to top

```jsx
// App.js
import React, { useState } from "react";
import Hello from "./Hello";
function App(props) {
  const [status, setStatus] = useState(false);
  return (
    <div>
      <button onClick={() => setStatus(!status)}>
        {status ? "Hide" : "Show"}
      </button>
      {status && <Hello />}
    </div>
  );
}

export default App;
// Hello.js
import React, { useState } from "react";
import { useEffect } from "react";

function Hello(props) {
  const [value, setValue] = useState("");
  const [datas, setDatas] = useState([]);
  const [data, setData] = useState("comments");
  const [showGoToTop, setShowGoToTop] = useState(false);
  const tabs = ["comments", "users", "albums"];
  useEffect(() => {
    fetch(`https://jsonplaceholder.typicode.com/${data}`)
      .then((res) => res.json())
      .then((commentsList) => {
        setDatas(commentsList);
      });
  }, [data]);
  useEffect(() => {
    const handleScroll = () => {
      setShowGoToTop(window.scrollY >= 200);
    };
    window.addEventListener("scroll", handleScroll);
    // clean up function
    return () => {
      window.removeEventListener("scroll", handleScroll, false);
    };
  }, []);
  const handleTabClick = (tab) => {
    setData(tab);
  };
  const handleGoToTop = () => {
    window.scrollTo(0, 0);
  };
  useEffect(() => {
    document.title = value;
  });
  return (
    <div>
      <input
        value={value}
        type="text"
        onChange={(e) => setValue(e.target.value)}
      />
      <h3>Hello anh em</h3>
      {tabs.map((tab) => (
        <button
          style={data === tab ? { color: "red" } : null}
          onClick={() => handleTabClick(tab)}
          key={tab}
        >
          {tab}
        </button>
      ))}
      <ul>
        {datas.map((data) => (
          <li key={data.id}>{data.name || data.title}</li>
        ))}
      </ul>
      {showGoToTop && (
        <button
          onClick={handleGoToTop}
          style={{ position: "fixed", bottom: 0, right: 24 }}
        >
          go to top
        </button>
      )}
    </div>
  );
}

export default Hello;
```

-   Ví dụ tạo một App resize (khi thay đổi kích thước chiều ngang của trình duyệt thì sẽ hiển thị chiều ngang hiện tại lên)

```jsx
// App.js
import React, { useState } from "react";
import Hello from "./Hello";
function App(props) {
  const [status, setStatus] = useState(false);
  return (
    <div>
      <button onClick={() => setStatus(!status)}>
        {status ? "Hide" : "Show"}
      </button>
      {status && <Hello />}
    </div>
  );
}

export default App;

// Hello.js
import React, { useState } from "react";
import { useEffect } from "react";

function Hello(props) {
  const [size, setSize] = useState(window.innerWidth);
  useEffect(() => {
    const handleResize = () => {
      setSize(window.innerWidth);
    };
    window.addEventListener("resize", handleResize);
    return () => {
      window.removeEventListener("resize", handleResize);
    };
  }, []);
  return (
    <div>
      <h3>Size: {size}</h3>
    </div>
  );
}

export default Hello;
```

-   useEffect with timer functions

    -   Nếu ta code theo kiểu dưới đây thì trong hàm setInterval giá trị của time luôn luôn là 179(UI) do bản chất thằng useEffect với mảng rỗng chỉ chạy một lần => Lúc này trong phạm vi của hàm useEffect chúng ta sẽ có một biến time có giá trị là 180 là biến time trong setInterval tham chiếu tới biến time trên useEffect (closure)

```jsx
import React, { useState } from 'react';
import { useEffect } from 'react';

function Hello(props) {
    const [time, setTime] = useState(180);
    useEffect(() => {
        const timeOut = setInterval(() => {
            setTime(time - 1);
        }, 1000);
        return () => {
            clearInterval(timeOut);
        };
    }, []);
    return <h3>{time}</h3>;
}

export default Hello;
// Fix
useEffect(() => {
    const timeOut = setInterval(() => {
        setTime((prev) => prev - 1);
    }, 1000);
    return () => {
        clearInterval(timeOut);
    };
}, []);
// Hoặc
// Lúc này thằng setTimeout chạy lần đầu tiên và lắng nghe sự thay đổi của despendence đó là time, nếu time thay đổi thì component được re-render
function Hello(props) {
    const [time, setTime] = useState(180);
    useEffect(() => {
        const timeOut = setTimeout(() => {
            setTime(time - 1);
        }, 1000);
        return () => {
            clearInterval(timeOut);
        };
    }, [time]);
    return <h3>{time}</h3>;
}
```

-   useEffect with preview avatar

```jsx
// FileImage.js
import React, { useState } from "react";
import { useEffect } from "react";

function FileImage(props) {
  const [avatar, setAvatar] = useState();
  useEffect(() => {
    // cleanup
    return () => {
      // xóa object url khỏi bộ nhớ
      // nếu chỉ dùng URL.revokeObjectURL(avatar.preview);
      // thì sẽ gặp lỗi do khi mới bắt đầu chọn file (lúc này sẽ lọt vào handlePreviewAvata do change file)
      // khi này thì avatar sẽ thay đổi và hàm cleanup được gọi nhưng avatar là undefined (do nó gọi clearn up trước)
      // => cần check như dưới đây
      avatar && URL.revokeObjectURL(avatar.preview);
    };
  }, [avatar]);
  const handlePreviewAvata = (e) => {
    const file = e.target.files[0];
    file.preview = URL.createObjectURL(file);
    setAvatar(file);
    // fix trường hợp chọn 2 lần 2 file giống nhau ( Lúc này cần set value của ô input thành null để nó vẫn lắng nghe
    //được sự kiện onChange(Để cập nhật lại UI) từ input)
    e.target.value = null;
  };
  return (
    <div>
      <input
        type="file"
        // Nếu muốn chọn nhiều ảnh thì thêm
        // multiple
        onChange={handlePreviewAvata}
      />
      {avatar && <img src={avatar.preview} alt="" />}
    </div>
  );
}

export default FileImage;
// App.js
import React, { useState } from "react";
import FileImage from "./FileImage";
function App(props) {
  const [status, setStatus] = useState(false);
  return (
    <div>
      <button onClick={() => setStatus(!status)}>
        {status ? "Hide" : "Show"}
      </button>
      {status && <FileImage />}
    </div>
  );
}

export default App;

```

-   Qua đoạn code dưới đây ta sẽ hiểu, count trong clean up sẽ có giá trị chậm 1 nhịp so với count trong callback

=> Lý do: Sau khi nhận thấy có dự thay đổi count khi click vào "Click me" (Tắng 1 giá trị), Lúc này giao diện </br>
sẽ được render ra trước, sau đó mới đến useEffect, tuy nhiên clean up được gọi trước khi cập nhật cái giá trị </br>
trong callback nên giá trị sẽ chậm hơn một nhịp

```js
import { useEffect, useState } from 'react';
import './App.css';

function App() {
    const [count, setCount] = useState(0);

    useEffect(() => {
        console.log('Count in callback ', count);
        return () => {
            // clean up
            console.log('Count in Clean up ', count);
        };
    }, [count]);

    return (
        <div onClick={() => setCount(count + 1)} className="App">
            Click me
        </div>
    );
}

export default App;
```

-   useEffect with fake chat app

```jsx
// App.js
import React, { useState } from "react";
import FileImage from "./FileImage";
function App(props) {
  const [status, setStatus] = useState(false);
  return (
    <div>
      <button onClick={() => setStatus(!status)}>
        {status ? "Hide" : "Show"}
      </button>
      {status && <FileImage />}
    </div>
  );
}

export default App;
// FileImage.js
import React, { useEffect, useState } from "react";
const myLesson = [
  {
    id: 1,
    name: "Javascript",
  },
  {
    id: 2,
    name: "ReactJs",
  },
  {
    id: 3,
    name: "NodeJs",
  },
];
function FileImage(props) {
  const [lessonId, setLessonId] = useState(1);
  useEffect(() => {
    const handleComment = ({ detail }) => {
      console.log(detail);
    };
    window.addEventListener(`lesson-${lessonId}`, handleComment);
    return () => {
      window.removeEventListener(`lesson-${lessonId}`, handleComment);
    };
  }, [lessonId]);
  return (
    <ul>
      {myLesson.map((lesson) => (
        <li
          onClick={() => setLessonId(lesson.id)}
          style={{
            cursor: "pointer",
            color: lessonId === lesson.id ? "red" : "#333",
          }}
          key={lesson.id}
        >
          {lesson.name}
        </li>
      ))}
    </ul>
  );
}

export default FileImage;
// index.js
import React from "react";
import ReactDOM from "react-dom";
import "./index.css";
import App from "./App";
import reportWebVitals from "./reportWebVitals";
// Đứng ở phạm vi global để phát ra một sự kiện bắn đến file FileImage hoặc tất cả file con
function emitComment(id) {
  setInterval(function () {
    window.dispatchEvent(
      new CustomEvent(`lesson-${id}`, {
        detail: `Nội dung của lesson ${id}`,
      })
    );
  }, 2000);
}
emitComment(1);
emitComment(2);
emitComment(3);
ReactDOM.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>,
  document.getElementById("root")
);

// If you want to start measuring performance in your app, pass a function
// to log results (for example: reportWebVitals(console.log))
// or send to an analytics endpoint. Learn more: https://bit.ly/CRA-vitals
reportWebVitals();
```

<span style="color: red">useLayoutEffect hook</span>

-   So sánh giữa useEffect với useLayoutEffect
    -   useEffect
        -   Cập nhật lại state
        -   Cập nhật lại DOM (mutated)
        -   Render lại UI
        -   Gọi cleanup nếu despendence thay đổi
        -   Gọi useEffect callback
    -   useLayoutEffect
        -   Cập nhật lại state
        -   Cập nhật lại DOM (mutated) (Lúc này chưa render ra UI nhé, nó chỉ thay đổi ở bên trong thôi)
        -   Gọi cleanup nếu despendence thay đổi (sync)
        -   Gọi useLayoutEffect callback (sync)
        -   Render lại UI (Bước này thì mới nhìn thầy từ UI nè (bước 2))

*   Note:
    -   Hai hook lại được tạo ra để thực hiện sideEffect(Nên sử dụng useEffect)
    -   Khi sử dụng useEffect mà làm ảnh hưởng tới giao diện người dùng thì lúc này sẽ sử dụng useLayoutEffect(Nếu nó giải quyết được vấn đề)

-   Ta xem xét ví dụ sau:

    -   Ví dụ: khi click vào một nút thì tăng giá trị của số đó lên, nếu số lớn hơn 3 ( số chạy từ 0) thì set lại giá trị về 0
        -   Vấn đề: Khi giá trị của số đó lên tới 3, lúc này click một lần nữa thì ở giao diện sẽ thấy nó nháy số 4 rồi mới trờ về 0 ( rất nhanh )
            => Khắc phục bằng useLayoutEffect hook

```jsx
// App.js
import React, { useState } from "react";
import Counter from "./Counter";
function App(props) {
  const [status, setStatus] = useState(false);
  return (
    <div>
      <button onClick={() => setStatus(!status)}>
        {status ? "Hide" : "Show"}
      </button>
      {status && <Counter />}
    </div>
  );
}

export default App;
// Counter.js
import React, { useEffect, useState } from "react";

Counter.propTypes = {};

function Counter(props) {
  const [number, setNumber] = useState(0);
  useEffect(() => {
    if (number > 3) setNumber(0);
  }, [number]);
  const handleOnClickIns = () => {
    setNumber(number + 1);
  };
  return (
    <div>
      <h3>{number}</h3>
      <button onClick={handleOnClickIns}>Ins</button>
    </div>
  );
}

export default Counter;
```

-   Giải thích code trên:

    -   Khi giá trị của number là 3 (trên giao diện hiển thị 3), lúc này khi bấm vào nút ins thì number sẽ được tăng một giá trị (4), lúc này nó sẽ đi qua useEffect do thấy number là despendence thay đổi (nhưng chưa chạy callback của useEffect)
        => render ra giao diện (số 4) render ra UI xong thì nó mới chạy callback của useEffect (trong callback thầy number đang là giá trị 4 thì nó sẽ thực hiện set State lại về 0)

    => Gây ra hiện tượng nháy số 4 rồi trở về 0
    => Fix bằng usLayoutEffect

```jsx
// Counter.js
import React, { useLayoutEffect, useState } from 'react';

Counter.propTypes = {};

function Counter(props) {
    const [number, setNumber] = useState(0);
    useLayoutEffect(() => {
        if (number > 3) setNumber(0);
    }, [number]);
    const handleOnClickIns = () => {
        setNumber(number + 1);
    };
    return (
        <div>
            <h3>{number}</h3>
            <button onClick={handleOnClickIns}>Ins</button>
        </div>
    );
}

export default Counter;
```

-   Giải thích code trên chạy nếu thay thế vào(Ở phần đầu luôn, khác biệt là nó render UI ở cuối cùng)

<span style="color: red;">**useRef hook**</span>

-   ref được kí hiệu là một reference (tham chiếu)
-   Tác dụng: Lưu các giá trị qua một tham chiếu bên ngoài function component
-   Ví dụ 1: Tạo ra một app, app này khi ta bấm vào start thì số 60 sẽ được đếm từ 60 lùi lại theo từng giây

```jsx
import React, { useState } from 'react';

function App(props) {
    const [count, setCount] = useState(60);
    let timeID;
    const handleOnclickStart = () => {
        // hàm setInterval trả về một id
        timeID = setInterval(() => {
            setCount((prev) => prev - 1);
        }, 1000);
        console.log(timeID);
    };
    const handleOnclickEnd = () => {
        clearInterval(timeID);
        console.log(timeID);
    };
    return (
        <div>
            <h3>{count}</h3>
            <button onClick={handleOnclickStart}>start</button>
            <button onClick={handleOnclickEnd}>end</button>
        </div>
    );
}

export default App;
```

-   Thế nhưng mọi chuyện không như ta nghĩ:
    -   Vấn đề: Khi bấm start thì nó có chạy từ số 60 lùi về sau, thế nhưng khi ta bấm end thì nó sẽ không kết thúc
        -   Tuy nhiên khi số 60 hiện ra, ta nhanh tay bấm end (khi nó vẫn là 60 mà chưa bị giảm giá trị) thì nó sẽ clear được interval
        -   Phải đợi số 60 bị lùi về 1 đơn vị thì khi bấm end nó mới KHÔNG dừng lại
    -   Nguyên nhân: khi component được render lần đầu tiên thì biến timeId được tạo ra, lúc này những biến timeId thứ hai trở đi sẽ được tham chiếu tới timeId đầu, tuy nhiên sau khi giá trị nó giảm đi thì component được thay đổi state và render lại và tạo ra một timeId mới (undefinded) => nó không thể clear time interval
        (Liên quan tới phạm vi, vì khi component được render lại thì nó sẽ tạo ra một phạm vi mới. Mỗi hàm được tạo nó sẽ không liên quan gì đến phạm vi trước đó) => Chúng ta có thể fix bằng cách đưa biến timeId ra ngoài phạm vi của App thì sẽ được kết quả như mong đợi, tuy nhiên thì không nên làm như thế :v
-   Ta sẽ sử dụng useRef để fixx vấn đề trên
    -   useRef sẽ luôn trả ra một object có property là current (value là giá trị định nghĩa trong initial value)
    -   Giá trị truyền cho ref lần đầu là initial value (nó có tác dụng trong lần đầu tiên khi component được mounted vì những lần sau nó bị thay đổi, giá trị này có thể là bất kì giá trị nào của Js)
-   Thực hiện fix

```jsx
import React, { useRef, useState } from 'react';

function App(props) {
    const [count, setCount] = useState(60);
    const timeID = useRef();
    const handleOnclickStart = () => {
        timeID.current = setInterval(() => {
            setCount((prev) => prev - 1);
        }, 1000);
        console.log(timeID.current);
    };
    const handleOnclickEnd = () => {
        clearInterval(timeID.current);
        console.log(timeID.current);
    };
    return (
        <div>
            <h3>{count}</h3>
            <button onClick={handleOnclickStart}>start</button>
            <button onClick={handleOnclickEnd}>end</button>
        </div>
    );
}

export default App;
```

-   Ví dụ lấy ra giá trị hiện tại và trước đó của state

```jsx
import React, { useEffect, useRef, useState } from 'react';

function App(props) {
    const [count, setCount] = useState(60);
    const timeID = useRef();
    const prevCount = useRef();
    useEffect(() => {
        prevCount.current = count;
    }, [count]);
    const handleOnclickStart = () => {
        timeID.current = setInterval(() => {
            setCount((prev) => prev - 1);
        }, 1000);
    };
    const handleOnclickEnd = () => {
        clearInterval(timeID.current);
    };
    console.log('count: ', count, 'prevCount: ', prevCount.current);
    return (
        <div>
            <h3>{count}</h3>
            <button onClick={handleOnclickStart}>start</button>
            <button onClick={handleOnclickEnd}>end</button>
        </div>
    );
}

export default App;
```

-   Ví dụ lưu một DOM element

```jsx
import React, { useEffect, useRef, useState } from 'react';

function App(props) {
    const h1Ref = useRef();
    useEffect(() => {
        console.log(h1Ref.current);
        // Lấy ra tọa độ của element
        const rect = h1Ref.current.getBoundingClientRect();
        console.log(rect);
    });
    return (
        <div>
            <h3 ref={h1Ref}>hello every one</h3>
        </div>
    );
}

export default App;
```

<span style="color: red">**Phương thức của thư viện React.memo() Higher Order component (HOC)**</span>

-   Giúp tối ưu hiệu năng, giúp xử lí một component tránh re-render ở những tình huống không cần thiết
-   Chúng ta cùng xem tình huống sau:

```jsx
// App.js
import React, { useState } from "react";
import Content from "./Content";

function App(props) {
  const [count, setCount] = useState(0);
  const handleOnIns = () => {
    setCount(count + 1);
  };
  return (
    <div>
      <Content />
      <h3>{count}</h3>
      <button onClick={handleOnIns}>ins</button>
    </div>
  );
}

export default App;
// Content.js
import React from "react";
function Content(props) {
  console.log("re-render");
  return <div>Hello anh em F8</div>;
}

export default Content;
```

-   Chúng ta thấy rằng, qua ví dụ trên, mặc dù logic của file App không liên quan gì đến file Content, thế nhưng khi App thay đổi state thì nó lại re-render lại nguyên một component đó là Content. Trong trường hợp component Content này xử lí rất phúc tạp thì nó làm giảm hiệu năng của App

=> Vì thế xử dụng memo để xử lí

```jsx
// Fix
import React, { memo } from 'react';
function Content(props) {
    console.log('re-render');
    return <div>Hello anh em F8</div>;
}
// Đây nè
export default memo(Content);
// Nó sẽ check tất cả props của Component Content xem mỗi lần render props có bị thay đổi hay không, chỉ cần ít nhất mọt props bị thay đổi thi nó sẽ cho phép component re-render, nếu không thay đổi thì thôi ;>
// memo sẽ sử dụng toán tử 3 dấu bằng để so sánh (Nhận biết props có thay đổi hay không)
```

-   Giả sử như này thì sẽ bị re-render

```jsx
// App.js
import React, { useState } from "react";
import Content from "./Content";

function App(props) {
  const [count, setCount] = useState(0);
  const handleOnIns = () => {
    setCount(count + 1);
  };
  return (
    <div>
      <Content count={count} />
      <h3>{count}</h3>
      <button onClick={handleOnIns}>ins</button>
    </div>
  );
}

export default App;

// Content.js
import React, { memo } from "react";
function Content({ count }) {
  console.log("re-render");
  return <div>Hello anh em F8 {count}</div>;
}

export default memo(Content);

```

-   Note: Sử dụng memo HOC khi nào?
    -   Khi có component sử dụng nhiều props, có thể gây ảnh hưởng đến performance, độ phức tạp UI lớn

<span style="color: red">**useCallback() hook**</span>

-   Dùng để tránh tạo ra những hàm mới một cách không cần thiết, do đôi khi sơ ý tạo ra các function mới một cách không cần thiết có thể làm cho component con bị re-render một cách không cần thiết mặc dù đã áp dụng memo
-   Quy tắc đặt tên: Hàm nào trực tiếp xử lí logic thì chúng ta sẽ đặt tên cho nó là handle..., với những props chờ hành động đó xảy ra thì thay handle thành on... (giống quy ước của DOM)

-   Chúng ta theo dõi ví dụ dưới đây:

```jsx
// App.js
import React, { useState } from "react";
import Content from "./Content";

function App(props) {
  const [count, setCount] = useState(0);
  const handleOnIns = () => {
    setCount(count + 1);
  };
  return (
    <div>
      <Content onIns={handleOnIns} />
      <h3>{count}</h3>
    </div>
  );
}

export default App;
// Content.js
import React, { memo } from "react";
function Content({ onIns }) {
  console.log("re-render");
  return (
    <>
      <div>Hello anh em F8</div>
      <button onClick={onIns}>ins</button>
    </>
  );
}

export default memo(Content);
```

-   Qua ví dụ trên chúng ta thấy rằng: mặc dù thằng Content không dùng bất kì dữ liệu gì (có sử dụng memo) thế nhưng khi click vào btn thì nó vẫn bị re-render do mỗi lần App re-render thì nó sẽ tạo ra một function handleOnIns khác => props thay đổi => component con bị re-render (kiến thức reference types: mỗi lần gán một dấu bằng là nó tạo ra một tham chiếu mới )
-   Chúng ta sẽ khắc phục bằng việc sử dụng useCallback
    -   Cú pháp: useCallback(fn, [despendence]): Cách sử dụng y như useEffect

```jsx
//Fix file App.js thành:
import React, { useCallback, useState } from 'react';
import Content from './Content';

function App(props) {
    const [count, setCount] = useState(0);
    // lúc này useCallback sẽ tạo ra hàm bên trong
    // và nhận vào một tham chiếu lưu ra bên ngoài phạm
    // vi App sau đó nó return tham chiếu đó cho biến
    // handleOnIns  rồi lưu vào props onIns
    const handleOnIns = useCallback(() => {
        setCount((prev) => prev + 1);
    }, []);
    // Nếu có despendence thay đổi thì nó sẽ tạo ra hàm
    // mới và return về một tham chiếu mới
    return (
        <div>
            <Content onIns={handleOnIns} />
            <h3>{count}</h3>
        </div>
    );
}

export default App;
```

-   Trong thực tế, một component nhận rất nhiều props trong đó có nhiều props là kiểu dữ liệu nguyên thủy và cũng nhiều props là kiểu dữ liệu reference (tham chiếu)

=> Hãy xác định nếu sử dụng memo thì những props function chúng ta phải sử dụng useCallback hết

-   Nếu không sử dụng memo thì không được dùng useCallback làm gì :>, bởi vì nếu không có memo thì lúc nào thằng cha re-render thì thằng con cũng re-render
-   function component + memo giống như pure component trong class component

<span style="color: red">**useMemo hook**</span>

-   useMemo (hook) và memo (higher older component) đều có nghĩa là ghi nhớ, nhưng mỗi thằng sẽ dùng để xử lí một công việc khác nhau
-   useMemo giúp tránh thực hiện lại một logic nào đó không cần thiết

-   Ta có một app sau để tính tổng giá product

```jsx
import React, { useState } from 'react';
function App() {
    const [name, setName] = useState('');
    const [price, setPrice] = useState('');
    const [products, setProducts] = useState([]);
    const handleOnClickToAdd = () => {
        const newProducts = [
            ...products,
            {
                name,
                price: +price, //convert to number from string
            },
        ];
        setProducts(newProducts);
        setName('');
        setPrice('');
    };
    const total = products.reduce((sum, product) => {
        console.log('tinh toan lai...');
        return sum + product.price;
    }, 0);
    return (
        <div>
            <div>
                <input
                    value={name}
                    onChange={(e) => setName(e.target.value)}
                    type="name"
                    placeholder="enter name product"
                />
            </div>
            <div>
                <input
                    onChange={(e) => setPrice(e.target.value)}
                    value={price}
                    type="price"
                    placeholder="enter price product"
                />
            </div>
            <button onClick={handleOnClickToAdd}>Add</button>
            <br />
            <span>Total: {total}</span>
            <ul>
                {products.map((product, index) => (
                    <li key={index}>
                        {product.name} - {product.price}
                    </li>
                ))}
            </ul>
        </div>
    );
}

export default App;
```

-   Tuy nhiên, khi hàm total sẽ bị re-render lại khi state thay đổi => bị re-render một cách không cần thiết
-   Fix: re-render khi cần thiết, tránh re-render nhiều lần

```jsx
import React, { useMemo, useState } from 'react';
function App() {
    const [name, setName] = useState('');
    const [price, setPrice] = useState('');
    const [products, setProducts] = useState([]);
    const handleOnClickToAdd = () => {
        const newProducts = [
            ...products,
            {
                name,
                price: +price, //convert to number from string
            },
        ];
        setProducts(newProducts);
        setName('');
        setPrice('');
    };
    const total = useMemo(() => {
        products.reduce((sum, product) => {
            console.log('tinh toan lai...');
            return sum + product.price;
        }, 0);
    }, [products]);
    return (
        <div>
            <div>
                <input
                    value={name}
                    onChange={(e) => setName(e.target.value)}
                    type="name"
                    placeholder="enter name product"
                />
            </div>
            <div>
                <input
                    onChange={(e) => setPrice(e.target.value)}
                    value={price}
                    type="price"
                    placeholder="enter price product"
                />
            </div>
            <button onClick={handleOnClickToAdd}>Add</button>
            <br />
            <span>Total: {total}</span>
            <ul>
                {products.map((product, index) => (
                    <li key={index}>
                        {product.name} - {product.price}
                    </li>
                ))}
            </ul>
        </div>
    );
}

export default App;
```

<span style="color: red">**useReducer hook**</span>

-   import useReducer từ thư viện react
-   Bài toán nào sử dụng useReducer giải quyết được thì cũng có thể dùng useState để giải quyết và ngược lại
-   Khi nào thì sử dụng thằng nào?

    -   Trong hầu hết các trường hợp chúng ta có thể sử dụng useState để tạo ra trạng thái cho component của mình(có thiên hướng sử dụng trong component có state đơn giản(chỉ là kiểu dữ liệu nguyên thủy hoặc là kiểu phức tạp như array, object, function nhưng chỉ đơn giản là có một cấp mà không phải lồng nhiều cấp) hoặc số lượng state trong component ít)
    -   useReducer nên được sử dụng khi state của chúng ta trở nên phức tạp hơn(ví dụ kiểu dữ liệu không phải đơn giản nữa mà là các kiểu như array, object, ... hay là có nhiều tầng: trong object có vài object con) => Sủ dụng useReducer giúp code dễ hiểu hơn, ngắn gọn và trông đơn giản hơn, ...có những thứ có thể tách hẳn ra một file riêng

-   const [count, dispatch] = useReducer(reducer, initState);

    -   useReducer có thể nhận 3 tham số
        -   Thứ nhất là reducer
        -   Hai là initState
        -   Thứ 3 tự tìm hiểu
    -   Nguyên lí hoạt động: Khi useReducer được chạy thì nó sẽ nhận reducer (nó tạm để đấy đã, chưa gọi vội trong lần đầu), nó nhận giá trị khởi tạo và return một array, phần tử thứ nhất là count- chính là giá trị khởi tạo (initState), giá trị thứ hai là hàm - dispatch dùng để kích hoạt một action

-   Ví dụ:

```jsx
import React, { useReducer } from 'react';
// useState
// 1. init State: 0
// 2. actions: Up(state + 1) / Down (state - 1)

// useReducer
// 1. init State: 0
// 2. actions: Up(state + 1) / Down (state - 1)
// 3. Reducer
// 4. Dispatch

// initState
const initState = 0;
// actions
const UP_ACTION = 'up';
const DOWN_ACTION = 'down';
// reducer
const reducer = (state, action) => {
    console.log('reducer running...');
    switch (action) {
        case UP_ACTION: {
            // cái state được return này sẽ luôn phải cùng kiểu dữ liệu với initState
            return state + 1;
        }
        case DOWN_ACTION: {
            // cái state này sẽ luôn phải cùng kiểu dữ liệu với initState
            return state - 1;
        }
        default: {
            throw new Error('invalid action');
        }
    }
};
function App(props) {
    const [count, dispatch] = useReducer(reducer, initState);
    return (
        <div>
            <h3>{count}</h3>
            {/* Mỗi lần ấn thì reducer mới được gọi */}
            <button onClick={() => dispatch(DOWN_ACTION)}>Down</button>
            <button onClick={() => dispatch(UP_ACTION)}>Up</button>
        </div>
    );
}

export default App;
```

-   To Do App with useReducer hook

```jsx
import React, { useReducer, useRef } from 'react';
// initState
const initState = {
    job: '',
    jobs: ['quet nha', 'rua bat', 'nau com'],
};
// actions
const SET_JOB = 'set_job';
const ADD_JOB = 'add_job';
const REMOVE_JOB = 'remove_job';
const setJob = (payload) => {
    return {
        type: SET_JOB,
        payload,
    };
};
const addJob = (payload) => {
    return {
        type: ADD_JOB,
        payload,
    };
};
const removeJob = (payload) => {
    return {
        type: REMOVE_JOB,
        payload,
    };
};
// reducer
const reducer = (state, action) => {
    let newState;
    switch (action.type) {
        case SET_JOB:
            newState = {
                ...state,
                job: action.payload,
            };
            break;
        case ADD_JOB:
            newState = {
                ...state,
                // job: '',  có thể làm bước này thay cho bước dispatch setJob trong handleSubmit nhưng không nên làm thế, nên bóc tách dữ liệu
                jobs: [...state.jobs, action.payload],
            };
            break;
        case REMOVE_JOB:
            const newJobs = [...state.jobs];
            newJobs.splice(action.payload, 1);
            newState = {
                ...state,
                jobs: newJobs,
            };
            break;
        default:
            throw new Error('invalid action');
    }
    return newState;
};
function App() {
    const inputEml = useRef();
    const [state, dispatch] = useReducer(reducer, initState);
    const { job, jobs } = state;
    const handleSubmit = () => {
        dispatch(addJob(job));
        dispatch(setJob(''));
        inputEml.current.focus();
    };
    return (
        <div style={{ marginLeft: 100 }}>
            <h3>To Do</h3>
            <input
                ref={inputEml}
                value={job}
                onChange={(e) => dispatch(setJob(e.target.value))}
                type="text"
                placeholder="enter to do..."
            />
            <button onClick={handleSubmit}>Add</button>
            <ul>
                {jobs.map((job, index) => (
                    <li style={{ lineHeight: 2 }} key={index}>
                        {job}
                        <span
                            onClick={() => {
                                dispatch(removeJob(index));
                            }}
                            style={{ cursor: 'pointer' }}
                        >
                            &times;
                        </span>
                    </li>
                ))}
            </ul>
        </div>
    );
}
export default App;
```

<span style="color:yellow">useReducer recap(tóm tắt lại)</span>

-   Bóc tách logic trong ví dụ trên
-   Viết hàm log theo kiểu middleware (một cái hàm nó ôm một cái hàm)

-   src
    -   ToDo
        -   actions.js
        -   constants.js
        -   logger.js
        -   reducer.js
        -   index.js
    -   App.js

```jsx
// App.js
import ToDoApp from './ToDo'   //không cần phải import './ToDo'
// vì webpack nó đã cấu hình sẵn rồi, nếu trong thư mục có file index.js thì nó sẽ tự nạp
function App() {
    return <ToDoApp />;
}
export default App;

// actions.js
import { ADD_JOB, REMOVE_JOB, SET_JOB } from './constants'
export const setJob = (payload) => {
    return {
        type: SET_JOB,
        payload,
    };
};
export const addJob = (payload) => {
    return {
        type: ADD_JOB,
        payload,
    };
};
export const removeJob = (payload) => {
    return {
        type: REMOVE_JOB,
        payload,
    };
};

// constants.js
export const SET_JOB = "set_job";
export const ADD_JOB = "add_job";
export const REMOVE_JOB = "remove_job";

// reducer.js
import { ADD_JOB, REMOVE_JOB, SET_JOB } from './constants'
export const initState = {
    job: "",
    jobs: ["quet nha", "rua bat", "nau com"],
};

const reducer = (state, action) => {
    switch (action.type) {
        case SET_JOB:
            return {
                ...state,
                job: action.payload,
            };
        case ADD_JOB:
            return {
                ...state,
                // job: '',  có thể làm bước này thay cho bước dispatch setJob trong handleSubmit nhưng không nên làm thế, nên bóc tách dữ liệu
                jobs: [...state.jobs, action.payload],
            };
        case REMOVE_JOB:
            const newJobs = [...state.jobs];
            newJobs.splice(action.payload, 1);
            return {
                ...state,
                jobs: newJobs,
            };
        default:
            throw new Error("invalid action");
    }
};
export default reducer

// index.js
import React, { useReducer, useRef } from "react";
import reducer, { initState } from "./reducer"
import { addJob, setJob, removeJob } from "./actions"
import logger from "./logger"
function ToDoApp() {
    const inputEml = useRef();
    const [state, dispatch] = useReducer(logger(reducer), initState);
    const { job, jobs } = state;
    const handleSubmit = () => {
        dispatch(addJob(job));
        dispatch(setJob(""));
        inputEml.current.focus();
    };
    return (
        <div style={{ marginLeft: 100 }}>
            <h3>To Do</h3>
            <input
                ref={inputEml}
                value={job}
                onChange={(e) => dispatch(setJob(e.target.value))}
                type="text"
                placeholder="enter to do..."
            />
            <button onClick={handleSubmit}>Add</button>
            <ul>
                {jobs.map((job, index) => (
                    <li style={{ lineHeight: 2 }} key={index}>
                        {job}
                        <span
                            onClick={() => {
                                dispatch(removeJob(index));
                            }}
                            style={{ cursor: "pointer" }}
                        >
                            &times;
                        </span>
                    </li>
                ))}
            </ul>
        </div>
    );
}
export default ToDoApp;

// logger.js
function logger(reducer) {
    // Hai thằng prevState và action là do thằng cu useReducer trả về, return thay cho return thẳng reducer
    return (prevState, action) => {
        console.group(action.type)
        console.log("PrevState: ", prevState)
        console.log("Action: ", action)
        const newState = reducer(prevState, action)
        console.log("NextState: ", newState)
        console.groupEnd();
        return newState
    }
}
export default logger;
```

<span style="color: yellow">**useContext hook**</span>

-   Trong thư viện react, họ đã cung cấp sẵn cho ta một phương thức để có thể tạo ra context
-   Đây là khái niệm giúp đơn giản hóa việc truyền dữ liệu từ component cha xuống các component con mà không phải sử dụng props

-   Xem ví dụ sau:
-   Giả sử ta có component theo cấp sau:
    ComA => ComB => ComC
    -   Muốn lấy dữ liệu của ComA từ ComC thì ta phải truyền qua trung gian ComB (theo cách bình thường)
    -   Dùng context có thể truyền dữ liệu từ A tới bất kì component con nào mà không cần qua trung gian
-   Thử làm App theme cho phép khi click thì đổi màu giữa dark/ light
    -   Làm với props
    -   src
        -   components
            -   Content
            -   Paragraph
        -   App.js

```jsx
// App.js
import React from 'react'
import Content from './components/Content'
import { useState } from 'react';
import './App.css'
function App() {
    const [color, setColor] = useState('dark')
    const handleOnClick = () => {
        setColor(color === 'light' ? 'dark' : 'light')
    }
    return (
        <div>
            <button onClick={handleOnClick}>Toggle</button>
            <Content color={color} />
        </div>
    )
}
export default App

// Content.js
import React from 'react';
import Paragraph from '../Paragraph';

function Content({ color }) {
    return (
        <div>
            <Paragraph color={color} />
        </div>
    );
}

export default Content;

// Paragraph.js
function Paragraph({ color }) {
    console.log(color);
    return (
        <div className={color}>
            <p>lorem ipsum lorem ipsum dolor sit amet, consectetur adip</p>
        </div>
    );
}

export default Paragraph;

// App.css
.dark {
  background: #000;
  color: #fff;
}
```

-   Khi làm theo cách trên, nếu 1 vài component ở giữa mất đi thì móc nối props giữa các component cũng mất theo => Cần chỉnh lại code để tạo ra lại móc nối đó
-   Làm với context:
-   3 Bước làm việc với Context
    -   Create Context
    -   Provider (Cung cấp)
    -   Consumer (Sử dụng)
-   Context nghĩa là ngữ cảnh, nó sẽ tạo ra một phạm vi để giúp chúng ta truyền dữ liệu trong phạm vi đó

-   Ví dụ: ComA => ComB => ComC
-   Giả sử ta tạo context ở component A(nó ôm cả component A) thì nó sẽ giúp truyền dữ liệu của A xuống bất cứ component nào là con của A
-   Để truyền đi dữ liệu thì thằng context này sẽ sử dụng Provider để nhận dữ liệu và để nhận dữ liệu của Component cha từ Component con thì sẽ sử dụng Consumer

-   Thực hiện

    -   Trong bài toán này chúng ta tạo ra sử dụng context để làm theme thì đặt tên cho đúng nghĩa:

    ```jsx
    const ThemeContext = createContext();
    ```

    -   ThemeContext sẽ trả ra một object bao gồm Provider và Consumer để cung cấp và nhận dữ liệu

    ```jsx
    <ThemeContext.Provider value={theme}>
        <div>
            <button onClick={handleOnClick}>Toggle</button>
            <Content />
        </div>
    </ThemeContext.Provider>
    ```

    -   Component này có props là value để nhận vào một giá trị sử dụng cho tất cả những gì bên trong component(children)
    -   Lưu ý: Trong một ứng dụng React có thể gọi vô số context khác nhau

    ```jsx
    export const ThemeContext = createContext();
    // để có thể sử dụng ở component khác
    ```

    -   Tại component con cần import ThemeContext và để lấy dữ liệu từ ThemeContext, cần import thêm useContext (trong useContext đã thiết kế Consumer để giúp mình nhận dữ liệu)

    ```jsx
    const theme = useContext(ThemeContext);
    ```

    -   Trong ThemeContext có value là gì thì useContext(ThemeContext) trả ra value đó (tại component con)

-   Full ví dụ trên

```jsx
// App.js
import React from 'react'
import Content from './components/Content'
import { useState, createContext } from 'react';
import './App.css'
export const ThemeContext = createContext();
function App() {
    const [theme, setTheme] = useState('dark')
    const handleOnClick = () => {
        setTheme(theme === 'light' ? 'dark' : 'light')
    }
    return (
        <ThemeContext.Provider value={theme}>
            <div>
                <button onClick={handleOnClick}>Toggle</button>
                <Content />
            </div>
        </ThemeContext.Provider>
    )
}
export default App

// Content.js
// Lúc này không cần truyền qua prop để nhận dữ liệu nữa :>
import React from 'react';
import Paragraph from '../Paragraph';

function Content() {
    return (
        <div>
            <Paragraph />
        </div>
    );
}
export default Content;

// Paragraph.js
import { useContext } from 'react'
import { ThemeContext } from '../../App'
function Paragraph() {
    const theme = useContext(ThemeContext)
    return (
        <div className={theme}>
            <p>lorem ipsum lorem ipsum dolor sit amet, consectetur adip</p>
        </div>
    );
}
export default Paragraph;
```

-   Tái cấu trúc lại cho gọn gàng hơn
-   Cấu trúc file
-   src
    -   components
        -   Content
        -   Paragraph
    -   App.js
    -   ThemeContext.js
    -   index.js

```jsx
// App.js
import React from 'react'
import Content from './components/Content'
import './App.css'
import { ThemeContext } from './ThemeContext'
import { useContext } from 'react'
function App() {
    const context = useContext(ThemeContext)
    return (
        /* div này là children của ThemeContext */
        <div>
            <button onClick={context.handleOnClick}>Toggle</button>
            <Content />
        </div>
    )
}
export default App

// index.js (file cao nhất)
import React from "react";
import ReactDOM from "react-dom";
import "./index.css";
import App from "./App";
import { ThemeProvider } from "./ThemeContext"
import reportWebVitals from "./reportWebVitals";
ReactDOM.render(
  <React.StrictMode>
    {/* cho ở cấp cao nhất là ở đây */}
    <ThemeProvider>
      <App />
    </ThemeProvider>
  </React.StrictMode>,
  document.getElementById("root")
);
reportWebVitals();

// Content.js
import React from 'react';
import Paragraph from '../Paragraph';
function Content() {
    return (
        <div>
            <Paragraph />
        </div>
    );
}
export default Content;

// Paragraph.js
import { useContext } from 'react'
import { ThemeContext } from '../../ThemeContext'
function Paragraph() {
    // lúc này context là một object do value của ThemContext truyền vào
    const context = useContext(ThemeContext)
    return (
        <div className={context.theme}>
            <p>lorem ipsum lorem ipsum dolor sit amet, consectetur adip</p>
        </div>
    );
}

export default Paragraph;

// ThemeContext
// Tạo context, Provider và dữ liệu của context
import { useState, createContext } from 'react';
const ThemeContext = createContext();
// function Component ThemeProvider
function ThemeProvider({ children }) {
    const [theme, setTheme] = useState('dark')
    const handleOnClick = () => {
        setTheme(theme === 'light' ? 'dark' : 'light')
    }
    const values = {
        theme,
        handleOnClick
    }
    return (
        <ThemeContext.Provider value={values}>
            {children}
        </ThemeContext.Provider>
    )
}
export { ThemeContext, ThemeProvider }
```

<span style="color: yellow">**GlobalState with Context + useReducer**</span>

-   Giải thích ý nghĩa của global State:
    -   Đưa state ra phạm vi cao nhất( Cấp cao nhất ), từ đó mọi component trong App có thể truy cập và sử dụng state đó
-   Code & Cấu trúc dự án

    -   Cấu trúc dự án
        -   src
            -   store
                -   action.js
                -   constants.js
                -   Context.js
                -   hooks.js
                -   index.js
                -   logger.js
                -   Provider.js
                -   reduce.js
            -   App.js
            -   index.js
            -   App.css

-   store(Kho, lưu trữ, state toàn cục sẽ được lưu trữ ở đây, file liên quan tới cấu trúc của useReducer như reducer, action, ...)
-   Context.js: file tạo context
-   Provider.js: cung cấp các store xuống component qua context
-   reducer.js: tạo reducer
-   index.js: export các file xung quanh nó ra ngoài => Khi các file nào muốn import thì không cần phải .../.../ nữa mà chỉ cần import từ file store
-   custom hook

    -   hooks.js

-   Redux vs React-context

    -   Không thể thay thế Redux bằng React-context
    -   Redux giúp dev dễ dàng triển khai debug hơn(thư viện react-debug) - React-context(chưa có)
    -   Redux có kiến trúc để nó sẵn sàng apply Middleware
    -   Redux có Addons and extensibility
    -   Redux là Cross-platForm (đa nền tảng, dùng cho mọi dự án code bằng Js) and cross-framework usage - React-context chỉ dùng cho React
    -   Depending on your app's setup, much better performance than working with just Context (phụ thuộc vào cách cài đặt dự án của bạn, hiệu năng tốt hơn)
    -   Yếu điểm của useContext là render lại nhiều component
        => Sử dụng cho ứng dụng vừa nhỏ, dùng trong trường hợp setState lại không nhiều (Ví dụ trong trường hợp làm dark/light theme vì người dùng ít thay đổi chức năng này)
    -   Redux dùng trong trường hợp setState lại nhiều lần và dùng trong ứng dụng lớn hơn.

-   Code:

```jsx
// actions.js
import {
    SET_TODO_INPUT,
    ADD_TODO,
    REMOVE_TODO,
    SET_TEXT_BTN,
    EDIT_TODO,
    SET_CURRENT_INDEX
} from "./constants";

export const setTodoInput = (payload) => {
    return {
        type: SET_TODO_INPUT,
        payload
    }
}
export const setTextBtn = (payload) => {
    return {
        type: SET_TEXT_BTN,
        payload
    }
}
export const setCurrentIndex = (payload) => {
    return {
        type: SET_CURRENT_INDEX,
        payload
    }
}
export const addToDo = (payload) => {
    return {
        type: ADD_TODO,
        payload
    }
}
export const removeToDo = (payload) => {
    return {
        type: REMOVE_TODO,
        payload
    }
}
export const editToDo = (payload) => {
    return {
        type: EDIT_TODO,
        payload
    }
}

// constants.js
export const SET_TODO_INPUT = "set_todo_input";
export const ADD_TODO = "add_todo";
export const REMOVE_TODO = "remove_todo";
export const SET_TEXT_BTN = "set_text_btn";
export const EDIT_TODO = "edit_todo";
export const SET_CURRENT_INDEX = "set_current_index";

// Context.js
import { createContext } from "react"
const Context = createContext()
export default Context

// hooks.js
import { useContext } from "react";
import Context from "./Context";
export const useStore = () => {
    const [state, dispatch] = useContext(Context);
    return [state, dispatch];
    // Hoặc có thể return useContext(Context) luôn, nhưng không nên làm kiểu thế, trình bày như này cho clean, dễ hiểu
}

// src/store/ index.js
export { default as StoreProvider } from './Provider'
export { default as StoreContext } from './Context'
export * from './hooks'
export * as actions from './actions'
// actions là một object chưa tất cả những gì được lấy ra (Lấy tất cả thằng bên trong quy thành object)

// logger.js
function logger(reducer) {
    return (prevState, action) => {
        console.group(action.type)
        console.log("prevState", prevState);
        const nextState = reducer(prevState, action);
        console.log("nextState", nextState);
        console.groupEnd()
        return nextState
    }
}
export default logger

// Provider.js
import Context from './Context'
import { useReducer } from 'react'
import reducer, { initState } from './reducer'
import logger from './logger'
function Provider({ children }) {
    const [state, dispatch] = useReducer(logger(reducer), initState)
    return (
        <Context.Provider value={[state, dispatch]}>
            {children}
        </Context.Provider>
    )
}
export default Provider

// reducer.js
import {
    SET_TODO_INPUT,
    ADD_TODO,
    REMOVE_TODO,
    SET_TEXT_BTN,
    SET_CURRENT_INDEX,
    EDIT_TODO
} from "./constants"

const initState = {
    toDos: [],
    toDoInput: '',
    textBtn: 'Add',
    currentIndex: -1
}
function reducer(state, action) {
    switch (action.type) {
        case SET_TODO_INPUT:
            return {
                ...state,
                toDoInput: action.payload
            }
        case SET_TEXT_BTN:
            return {
                ...state,
                textBtn: action.payload
            }
        case SET_CURRENT_INDEX:
            return {
                ...state,
                currentIndex: action.payload
            }
        case ADD_TODO:
            const newToDos = [...state.toDos]
            if (action.payload.trim()) newToDos.push(action.payload)
            return {
                ...state,
                toDos: newToDos
            }
        case REMOVE_TODO:
            const newToDosList = [...state.toDos]
            newToDosList.splice(action.payload, 1)
            return {
                ...state,
                toDos: newToDosList
            }
        case EDIT_TODO:
            const newToDosEdit = [...state.toDos]
            newToDosEdit[action.payload] = state.toDoInput
            console.log(newToDosEdit)
            return {
                ...state,
                toDos: newToDosEdit
            }
        default:
            throw new Error("Error, not invalid action type")
    }
}
export default reducer
export { initState }

// App.js
import { useRef } from "react";
import { useStore, actions } from "./store";
import "./App.css";
function App() {
  const inputElm = useRef();
  const [state, dispatch] = useStore();
  const { toDos, toDoInput, textBtn, currentIndex } = state;
  const handleAdd = () => {
    if (textBtn === "Add") {
      dispatch(actions.addToDo(toDoInput));
      inputElm.current.focus();
      dispatch(actions.setTodoInput(""));
    }
    if (textBtn === "Done") {
      dispatch(actions.editToDo(currentIndex));
      dispatch(actions.setTodoInput(""));
      dispatch(actions.setTextBtn("Add"));
    }
  };
  const handleRemoveTodo = (index) => {
    if (window.confirm("Are you sure to remove this todo?"))
      dispatch(actions.removeToDo(index));
  };
  const handleEditToDo = (index) => {
    const toDoIsEdited = toDos[index];
    dispatch(actions.setTodoInput(toDoIsEdited));
    dispatch(actions.setTextBtn("Done"));
    dispatch(actions.setCurrentIndex(index));
  };
  return (
    <div className="center">
      <h1>Ní Hảo, Hủa Ai Nỉ F8</h1>
      <input
        ref={inputElm}
        type="text"
        value={toDoInput}
        placeholder="enter todo"
        onChange={(e) => {
          dispatch(actions.setTodoInput(e.target.value));
        }}
      />
      <button style={{ cursor: "pointer" }} onClick={handleAdd}>
        {textBtn}
      </button>
      <ul style={{ listStyle: "none" }}>
        {toDos.map((toDo, index) => (
          <li key={index}>
            {toDo}
            <span
              onClick={() => handleRemoveTodo(index)}
              style={{ cursor: "pointer", margin: "0 12px", lineHeight: "3" }}
            >
              &times;
            </span>
            <button
              onClick={() => handleEditToDo(index)}
              style={{ cursor: "pointer" }}
            >
              Edit
            </button>
          </li>
        ))}
      </ul>
    </div>
  );
}
export default App;

// src/index.js
import ReactDOM from "react-dom";

import App from "./App";
import { StoreProvider } from "./store";

const rootElement = document.getElementById("root");
ReactDOM.render(
  <StoreProvider>
    <App />
  </StoreProvider>,
  rootElement
);

```

<span style="color: yellow">**useImperative Handle hook**</span>

-   hook này giúp ta có thể tùy chỉnh được ref của một function component
-   Tạo mộp app có chức năng play và pause video
-   Tải video trên tik tok về:
-   Cách tải:
    -   Vào tik tok bấm F12 => Tab netWork => Media
    -   Mỗi khi next sang video mới thì nó sẽ show lên một resquest
    -   open new tab => Lưu
-   Cấu trúc thư mục:

    -   src
        -   video
            -   video1.mp4
        -   App.js
        -   Video.js

-   Thử làm theo tư duy logic :>

```jsx
// App.js
import React, { useRef } from 'react'
import { useImperativeHandle } from 'react'
import Video from './Video'
function App() {
    const videoRef = useRef()
    return (
        <div>
            <Video ref={videoRef} />
            <button>Play</button>
            <button>Pause</button>
        </div>
    )
}
export default App

// Video.js
import video1 from './video/video1.mp4'
function Video(props) {
    const { ref } = props
    return (
        <video ref={ref} width={300} src={video1} />
    )
}
export default Video
```

-   Tuy nhiên, làm như trên không được do thằng react nó không quy định thế
-   Nếu chúng ta sủ dụng ref truyền thẳng cho react element mà nó đại diện cho một thẻ trong DOM thì chắc chắn sẽ lấy được DOM element của nó

```jsx
<video ref={ref} width={300} src={video1} />
```

-   Trong trường hợp truyền props là ref cho function component => sẽ không được vì mặc định thằng function component sẽ không có ref

```jsx
function App() {
    const videoRef = useRef();
    useEffect(() => {
        console.log(videoRef.current); //undefined
    });
    return (
        <div>
            <Video ref={videoRef} />
            <button>Play</button>
            <button>Pause</button>
        </div>
    );
}
// - Ref được thằng react sử dụng cho mục đích riêng => Không thể forward xuống dưới => Ở dưới không nhận được

function Video(props) {
    const { ref } = props;
    console.log(ref); //undefined
    return <video ref={ref} width={300} src={video1} />;
}
```

-   React cung cấp cho mình một higher order component để giúp chúng ta forward được ref từ function component App đến function componenent Video
-   Từ function Componenet Video import forwardRef (truyền tiếp) và ôm export Video

```jsx
import video1 from './video/video1.mp4';
import { forwardRef } from 'react';
function Video(props, ref) {
    console.log(ref);
    return <video ref={ref} width={300} src={video1} />;
}
export default forwardRef(Video);

// Thực chất dòng trên là expot ra thằng forwardRef, nó sẽ xử lí để export ra function component Video và nhận đói số thứ 2 là ref
// <Video ref={videoRef} /> truyền cho forwardRef
```

-   Full Code:

```jsx
// App.js
import React, { useRef, useEffect } from 'react'
import { useImperativeHandle } from 'react'
import Video from './Video'
function App() {
    const videoRef = useRef()
    const handlePlay = () => {
        videoRef.current.play()
    }
    const handlePause = () => {
        videoRef.current.pause()
    }
    return (
        <div>
            <Video ref={videoRef} />
            <button onClick={handlePlay}>Play</button>
            <button onClick={handlePause}>Pause</button>
        </div>
    )
}
export default App

// Video.js
import { forwardRef } from 'react'
import video1 from './video/video1.mp4'
function Video(props, ref) {
    return (
        <video
        // ref này bị public ra thằng App full ;>
            ref={ref}
            width={300}
            src={video1}
        />
    )
}
export default forwardRef(Video)
```

-   Tuy nhiên Chúng ta đang public hẳn một ref ra ngoài (ref trong Video.js) trong khi nhu cầu của chúng ta chỉ là play và pause thôi => Rất nguy hiểm (Liên quan tới Opp, tính đóng gói => Gây rủi ro)
-   Từ App không phải là Video mà nó lại có toàn quyền với ref của video như chính bản thân nó

```jsx
import React, { useRef } from 'react';
import Video from './Video';
function App() {
    const videoRef = useRef();
    const handlePlay = () => {
        // THÊM DÒNG NÀY LÀ HẸO
        videoRef.current.remove();
        videoRef.current.play();
    };
    const handlePause = () => {
        videoRef.current.pause();
    };
    return (
        <div>
            <Video ref={videoRef} />
            <button onClick={handlePlay}>Play</button>
            <button onClick={handlePause}>Pause</button>
        </div>
    );
}
export default App;
```

-   Cần làm sao để nó trả ra đúng 2 method cần dùng là play và pause thôi
-   Code

```jsx
// App.js
import React, { useRef } from 'react'
import Video from './Video'
function App() {
    const videoRef = useRef()
    const handlePlay = () => {
        console.log(videoRef.current)   //object truyền vào callBack bên file Video.js
        videoRef.current.play()
    }
    const handlePause = () => {
        videoRef.current.pause()
    }
    return (
        <div>
            <Video ref={videoRef} />
            <button onClick={handlePlay}>Play</button>
            <button onClick={handlePause}>Pause</button>
        </div>
    )
}
export default App

// Video.js
import { forwardRef, useImperativeHandle, useRef } from 'react'
import video1 from './video/video1.mp4'
function Video(props, ref) {
    const videoRef = useRef()
    // đối số 1 là ref, thứ 2 là callback
    // return một object mà thằng videoRef bên kia (file App) sẽ nhận được
    useImperativeHandle(ref, () => ({
        play() {
            videoRef.current.play()
        },
        pause() {
            videoRef.current.pause()
        }
    }))
    return (
        <video
            ref={videoRef}
            width={300}
            src={video1}
        />
    )
}
export default forwardRef(Video)
```

<span style="color: yellow">**Sử dụng Css trong ReactJS**</span>

-   Css inline

```jsx
import React from 'react';
function App() {
    return <h3 style={{ color: 'red' }}>Css inline</h3>;
}
export default App;
```

-   Cách 2:

    -   Đây là dự án được tạo bởi create-react-app => Có webpack (trong webpack cấu hình sẵn cho chúng ta rồi, nó nó thấy có import một file css thì nó sẽ hiểu đây là một file style và nó sẽ nạp vào trang web của các bạn khi chạy trên trình duyệt)
    -   Khi chạy ở chế độ development: npm start/ yarn start => Css **internal**
    -   Khi import các file css khác nhau thì nó sẽ tạo ra một thẻ style khác nhau chứa nội dung của các file css kia
    -   Khi Website được triển khai cho người dùng cuối(môi trường production => Cần build nó ra: npm run build | yarn build) => Css ở dạng **external**, thử gõ câu lệnh trên => Chạy xong nó sẽ tạo ra một file build => Gõ lệnh serve -s /build để chạy file đã được build
    -   Trên môi trường production nó sẽ gom hết css lại thành một file (mini file) để tối ưu hiệu năng
        -   Giải thích: Mỗi một file css sẽ gửi đi một request http được gửi đi, tính chất của request http sẽ thực hiện kết nối và đóng kết nối mỗi lần nó tải file => Tốn càng nhiều thời gian nếu càng nhiều file
    -   Tuy nhiên có một vấn đề là: Sau khi import nhiều file css khác nhau nhưng cuối cùng nó vẫn được gộp lại trong một file (Cùng phạm vi) => Việc đặt trùng tên Css ở các file khác nhau dẫn tới ảnh hưởng css của các file đó

    => Cần có cách đặt tên hợp lý (BEM)

    -   Trong thực tế người ta sẽ không style trong một file, vì khi số lượng component nhiều lên thì rất khó xóa / chỉnh sửa/ thêm css cho từng component
    -   Cách dùng chuẩn là tạo một components, mỗi component nhỏ sẽ có 2 file: index.js và componentName.css

```jsx

// App.js
import React from 'react'
import './App.css'
function App() {
    return (
        <h3 className='redText'>Css inline</h3>
    )
}
export default App

// App.css
.redText {
  color: red;
}
```

<span style="color: yellow">**Css module**</span>

-   Là khái niệm giúp ta có thể tạo ra các file Css hoạt động một cách độc lập và không bị ảnh hưởng tới nhau (khi có nhiều component và có nhiều file css đi kèm, có thể đặt trùng class, css selector mà nó sẽ không bị ảnh hường tới nhau)
-   Vấn đề:
-   Cấu trúc file:
-   src
    -   App.js
    -   components
        -   Heading
            -   index.js
            -   Heading.css
        -   Paragraph
            -   index.js
            -   Paragraph.css

```js
// App.js
import React from 'react'
import Heading from './Heading'
import Paragraph from './Paragraph'
function App() {
    return (
        <>
            <Heading />
            <Paragraph />
        </>
    )
}
export default App

// Heading.js
import './Heading.css'
import React from 'react'
function Heading() {
    return (
        <h3 className="heading">Hello anh em F8</h3>
    )
}
export default Heading

// Heading.css
.heading {
  color: red;
}

// Paragraph.js
import React from 'react'
import './Paragraph.css'
function Paragraph() {
    return (
        <h3>Đây là nội dung của paragraph</h3>
    )
}
export default Paragraph

// Paragraph.css
.heading {
  font-size: 46px;
}
```

-   Trong đoạn code trên, mặc dù chúng ta css tại file Paragraph thế nhưng file Heading vẫn bị ảnh hưởng do Css cho heading tại file Paragraph
-   Có 2 cách fix là dùng:
    -   Css module
    -   Styled component
-   Tìm hiểu Css module trước:

    -   Khi dùng css module cần đổi tên file thành ComponentsName.module.css
    -   Cần chỉnh sửa lại cách import file Css
        -   Lý do: khi tạo một dự án bởi create-react-app thì webpack nó đã được hỗ trợ sẵn để css module rồi chỉ cần đặt tên theo đúng format thì nó sẽ tự động nhận diện và lấy content của file css và export ra một object
        -   Object này chứa các keys là class cũ của các bạn và value tương ứng sẽ được chuyển đổi theo quy ước: nameComponent_className\_\_code... (dùng thuật toán B64 mã hóa dựa trên cái đường dẫn (path) tới file css đó)
        -   Truy cập bằng cách dùng object file css đó export ra chọc tới key là className cũ là được

-   Ví dụ:
-   Cấu trúc file:
-   src
    -   App.js
    -   components
        -   Heading
            -   index.js
            -   Heading.module.css
        -   Paragraph
            -   index.js
            -   Paragraph.module.css

```js
// App.js
import React from 'react'
import Heading from './Heading'
import Paragraph from './Paragraph'
function App() {
    return (
        <>
            <Heading />
            <Paragraph />
        </>
    )
}
export default App

// Heading.js
import styles from './Heading.module.css'
// styles này là một object
import React from 'react'
function Heading() {
    return (
        <h3 className={styles.heading}>Hello anh em F8</h3>
    )
}
export default Heading

// Heading.module.css
.heading {
  color: red;
}

// Paragraph.js
import React from 'react'
import styles from './Paragraph.module.css'
function Paragraph() {
    return (
        <h3>Đây là nội dung của paragraph</h3>
    )
}
export default Paragraph

// Paragraph.css
.heading {
  font-size: 46px;
}
```

=> Giải quyết được vấn đề do tên class được thay đổi theo tên component và một đoạn mã hóa

-   Hạn chế của css module:
    -   Không có tính kế thừa do chỉ dùng được một class đấy cho một file cố định vì nó bị đổi tên class => Muốn đặt trùng class cũng không được
-   Ưu điểm:
    -   Không bị trùng nhau
    -   Giúp css đi cùng component (Hoạt động độc lập, khi không dùng đến chỉ việc không import file Js nữa là tự nhiên cả Js và css đều không hoạt động => Không gây ra thừa css)
-   Giải quyết: Kết hợp cách sử dụng bình thường và css module
-   Lưu ý:
    -   Không được sử dụng tagName hoặc thẻ css riêng biệt trong file (Ví dụ: \*, h1, h3, p, ...) vì nó không thể mã hóa, Lúc này nó sẽ không còn tác dụng css riêng biệt mà sẽ css tất cả các component như cách thường luôn
    -   Khi dùng theo kiểu css module thì chúng ta sẽ đặt tên class ban đầu theo kiểu camelCase vì khi chúng ta dùng object.(truy cập key của object) thì sẽ hợp lý hơn và giúp dễ quản lí hơn, khi cần sửa thì chỉ cần expect trang web lên, nhìn vào tên là biết nó đang nằm ở component nào.
-   Giải quyết vấn đề kế thừa
    -   Có thể tạo file index.css (import vào File cao nhất là index.js ý), tuy nhiên không nên dùng cách này do không đồng nhất và không có tính component hóa
    -   Cách khác:
-   Cấu trúc file
-   src
    -   GlobalStyles
        -   index.js
        -   GlobalStyles.css
    -   Heading
        -   Heading.module.css
        -   index.js
    -   Paragraph
        -   index.js
        -   Paragraph.module.css
-   index.js

```js
// - GlobalStyles
    // index.js
import './GlobalStyles.css'
function GlobalStyles({ children }) {
    return children
}
export default GlobalStyles
    // GlobalStyles.css
/* Css ở đây */
.d-flex {
  display: flex;
}

// Heading
    // index.js
import style from './Heading.module.css'
import React from 'react'
console.log(style)
function Heading() {
    return (
        <h3 className={style.heading}>Hello anh em F8</h3>
    )
}
export default Heading
    // Heading.module.css
.heading {
  color: red;
}

// Paragraph
    // index.js
import React from 'react'
import './Paragraph.module.css'
function Paragraph() {
    return (
        <h3>Đây là nội dung của paragraph</h3>
    )
}
export default Paragraph
    // Paragraph.module.css
.heading {
  font-size: 46px;
}
```

<span style="color:yellow">Cách dùng CLSX và ClassNames</span>

-   Di chuyển nhanh tới file viết component bằng cách giữ ctr (window hoặc command Mac) rồi chọn vào component đó
-   Lưu ý: props className nhận dữ liệu là kiểu chuỗi => Muốn một elm có nhiều class thì chỉ cần dùng template string và ngăn chúng là một dấu cách
-   Cách làm:
-   Cài đặt clsx
-   Cấu trúc file:
-   src
    -   Button
        -   index.js
        -   Button.module.css
    -   GlobalsStyles
        -   index.js
        -   GlobalsStyles.css

```js
// - Button
//         - index.js
import React from 'react'
import styles from './Button.module.css'
console.log(styles)
function Button(props) {
    return (
        <>
            <button className={styles.btn}>Click me!</button>
            <button className={`${styles.btn} ${styles.active}`}>Click me!</button>
            {/* <button className={[styles.btn, styles.active].join(" ")}>Click me!</button> */}
        </>
    )
}
export default Button
//         - Button.module.css
.btn {
  padding: 4px 16px;
  border: 2px solid #ccc;
  border-radius: 4px;
}
.active {
  background: red;
}

// - GlobalsStyles
//         - index.js
import './GlobalStyles.css'
function GlobalStyles({ children }) {
    return children
}
export default GlobalStyles
//         -   GlobalsStyles.css
/* Css ở đây */
.d-flex {
  display: flex;
}

```

-   Tuy nhiên trình bày theo cách trên rất xấu, thường thì người ta hay sử dụng hai thư viện là classnames và clsx
-   Clsx

```js
// Button.js
import clsx from 'clsx';
import styles from './Button.module.css';
console.log(styles);
function Button(props) {
    return (
        <>
            <button className={styles.btn}>Click me!</button>
            <button className={clsx(styles.btn, styles.active)}>
                Click me!
            </button>
        </>
    );
}
export default Button;
```

-   Class động

```js
// Button.js
import clsx from 'clsx'
import styles from './Button.module.css'
function Button(props) {
    return (
        <>
            <button className={styles.btn}>Click me!</button>
            <button className={clsx(styles.btn, {
                [styles.active]: true
            })}>Click me!</button>
        </>
    )
}
export default Button

// Xử lý theo props hoặc muốn thêm class global vào
// App.js
import React from 'react'
import GlobalStyles from './GlobalStyles'
import Button from './Button'
function App() {
    return (
        <GlobalStyles>
            <Button primary />
            <Button />
        </GlobalStyles>
    )
}
export default App

// Button.js
import clsx from 'clsx'
import styles from './Button.module.css'
function Button({ primary }) {
    const classes = clsx(styles.btn, 'd-flex', { [styles.primary]: primary })
    // Nếu muốn dùng class global động:
    // const classes = clsx(styles.btn, { 'd-flex': true }, { [styles.primary]: primary })
    return (
        <>
            <button className={clsx(classes)}>Click me!</button>
        </>
    )
}
export default Button
```

<span style="background-color: yellow">Install Sass để dùng scss</span>

-   Trong dự án tạo bởi create-react-app thì nó sẽ hỗ trợ viết bằng css và sass
-   Cài thư viện sass: gg search
-   Với thư viện này, nó cần tạo một file loader để cấu hình cho webpack => Yêu cầu phải tắt development server đi
-   Sau khi cài xong thì tìm hiểu về sass
-   Ví dụ:

```js
// App.js
import React from 'react'
import GlobalStyles from './GlobalStyles'
import Button from './Button'
function App() {
    return (
        <GlobalStyles>
            <Button primary />
            <Button disabled />
        </GlobalStyles>
    )
}
export default App

// Button
    // index.js
import clsx from 'clsx'
import styles from './Button.module.scss'
function Button({ primary, disabled }) {
    const classes = clsx(styles.btn, { [styles.disabled]: disabled })
    return (
        <>
            <button className={clsx(classes)}>Click me!</button>
        </>
    )
}
export default Button
```

```css
/* Button.module.scss */
.btn {
    padding: 4px 16px;
    border: 2px solid #ccc;
    border-radius: 4px;
    cursor: pointer;
    &:hover {
        background: #fff;
    }
}
.primary {
    background: blue;
}

.disabled {
    color: #ccc;
    cursor: none;
}
```

<span style="background-color: yellow">React Router V6 | Định tuyến trong ReactJS</span>

-   Tạo ra cơ chế định tuyến cho những ứng dụng được viết bởi reactJs
-   Định tuyến và cho phép di chuyển qua lại giữa các trang trong website
-   cần install thư viện về
-   Gói toàn bộ trang web bằng BrowerRouter (Một trang web chỉ có một thằng này thôi nhé)

```js
import { BrowserRouter as Router } from 'react-router-dom';
// import BrowserRouter rồi đổi tên thành Router (Bước này bonus)
ReactDOM.render(
    <React.StrictMode>
        <Router>
            <App />
        </Router>
    </React.StrictMode>,
    document.getElementById('root')
);
```

-   Ví dụ full:

-   Cấu trúc file:
-   src
    -   components
        -   Header
            -   index.js
    -   pages
        -   Contact.js
        -   Home.js
        -   News.js
        -   NoMath.js
    -   index.js
    -   App.js

```js
// - components
    // - Header
            // - index.js
import { Link } from "react-router-dom"
import { Outlet } from "react-router"
function Header() {
    return (
        <nav>
            <ul>
                <li>
                    <Link to="/">Home</Link>
                </li>
                <li>
                    <Link to="/news">News</Link>
                </li>
                <li>
                    <Link to="/contact">Contact</Link>
                </li>
            </ul>
            <Outlet />
        </nav>
    )
}
export default Header

// - pages
//         - Contact.js

function Contact() {
    return (
        <>
            <h3>Contact</h3>
        </>
    )
}
export default Contact

//         - Home.js

function Home() {
    return (
        <>
            <h3>Home</h3>
        </>
    )
}
export default Home

//        - News.js

function News() {
    return (
        <>
            <h3>News</h3>
        </>
    )
}
export default News

//        - NoMath.js

import { Link } from "react-router-dom";

function NoMatch() {
    return (
        <div>
            <h2>Nothing to see here!</h2>
            <p>
                <Link to="/">Go to the home page</Link>
            </p>
        </div>
    )
}
export default NoMatch

// - index.js
import React from "react";
import { BrowserRouter as Router } from "react-router-dom";
import ReactDOM from "react-dom";
import App from "./App";
import reportWebVitals from "./reportWebVitals";
ReactDOM.render(
  <React.StrictMode>
    <Router>
      <App />
    </Router>
  </React.StrictMode>,
  document.getElementById("root")
);
reportWebVitals();

// App.js
import React from 'react'
import { Routes, Route } from 'react-router'
import Header from './components/Header.js'
import Contact from './pages/Contact'
import Home from './pages/Home'
import News from './pages/News'
import NoMatch from './pages/NoMatch.js'
function App() {
    return (
        <div>
            <h3>Welcome you come my app</h3>
            <Routes>
                <Route path="/header" element={<Header />}>
                    <Route index path="/" element={<Home />} />
                    <Route path="news" element={<News />} />
                    <Route path="contact" element={<Contact />} />
                    <Route path="*" element={<NoMatch />} />
                </Route>
            </Routes>
        </div>
    )
}
export default App
```

-   Một ví dụ về react-router (Tự thay đổi url theo path để thây kết quả)

```js
import { Routes, Route, Outlet } from 'react-router-dom';
import { useParams } from 'react-router';
function App() {
    return (
        <Routes>
            <Route path="invoices" element={<Invoices />}>
                <Route path=":invoiceId" element={<Invoice />} />
                <Route path="sent" element={<SentInvoices />} />
            </Route>
        </Routes>
    );
}

function Invoices() {
    return (
        <div>
            <h1>Invoices</h1>
            <Outlet />
        </div>
    );
}

function Invoice() {
    let { invoiceId } = useParams(); //Trả về param hiện tại
    return <h1>Invoice {invoiceId}</h1>;
}

function SentInvoices() {
    return <h1>Sent Invoices</h1>;
}

export default App;
```

-   Khi một parent route có nhiều route con, nhưng url đang ở parent route => Muốn hiển thị mặc định một route khi đang ở route mẹ thì:

```js
import { Routes, Route, Link, Outlet } from 'react-router-dom';

function App() {
    return (
        <Routes>
            <Route path="/" element={<Layout />}>
                <Route index element={<Invoices />} />
                <Route path="invoices" element={<Invoices />} />
                <Route path="dashboard" element={<Dashboard />} />
            </Route>
        </Routes>
    );
}

function Layout() {
    return (
        <div>
            <h1>Welcome to the app!</h1>
            <nav>
                <Link to="invoices">Invoices</Link> |{' '}
                <Link to="dashboard">Dashboard</Link>
            </nav>
            <div className="content">
                <Outlet />
            </div>
        </div>
    );
}

function Invoices() {
    return <h1>This is invoices</h1>;
}

function Dashboard() {
    return <h1>This is Dashboard</h1>;
}

export default App;
```

-   Route nhiều cấp, muốn show 2 route trong một route cha

```js
import { Routes, Route, Link, Outlet } from 'react-router-dom';

function Home() {
    return <h1>Home</h1>;
}

function Dashboard() {
    return (
        <div>
            <h1>Dashboard</h1>
            <nav>
                <Link to="invoices">Invoices</Link> <Link to="team">Team</Link>
            </nav>
            <hr />
            <Outlet />
        </div>
    );
}

function Invoices() {
    return <h1>Invoices</h1>;
}

function Team() {
    return <h1>Team</h1>;
}

function App() {
    return (
        <Routes>
            <Route path="/" element={<Home />} />
            <Route path="dashboard" element={<Dashboard />}>
                <Route path="invoices" element={<Invoices />} />
                <Route path="team" element={<Team />} />
            </Route>
        </Routes>
    );
}

export default App;
```

-   Có thể có một Routes nằm sâu trong một thành phần của Routes cha, nó hoạt động như một Routes bình thường
-   Tuy nhiên trong Route chứa Routes cần một dấu \* để url của route con luôn khớp với cha của nó

```js
import { Routes, Route } from 'react-router-dom';
import Home from './pages/Home';
import Contact from './pages/Contact';
import News from './pages/News';
function App() {
    return (
        <Routes>
            <Route path="/" element={<Home />} />
            <Route path="dashboard/*" element={<Dashboard />} />
        </Routes>
    );
}

function Dashboard() {
    return (
        <div>
            <p>Look, more routes!</p>
            <Routes>
                <Route path="/" element={<Contact />} />
                <Route path="invoices" element={<News />} />
            </Routes>
        </div>
    );
}

export default App;
```

-   Làm một app kế toán:
    -   có chức năng search, hiển thị từng trang thanh toán, ...
    -   Lên trang chủ của react-router-dom 6 có source (Hoặc vào code sandbox)
