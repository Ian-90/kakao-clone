# kakao-clone

- [[이론+실전] 코코아톡 클론 코딩](https://academy.nomadcoders.co/p/kakaoclone_total) - HTML과 CSS를 이용하여, kakao clone하는 수업

---

## HTML(Hyper Text Markup Language)

### 1. HTML은 무엇인가 ?

- 웹사이트에서 각 요소가 무엇을 뜻하는지 알려주는 언어

- tag를 이용해서 작성

### 2. tag

- tag의 생김새 - <name attribute="value">Content</name>
- 열린 tag와 닫힌 tag가 항상 쌍으로 있어야 한다.
- example

```html
<div>hello</div>
<a href="http://google.com">Go to google</a>
```

### 3. html 문서 작성

```html
<!DOCTYPE html>
<html>
  <head>
    <title>This is my title</title>
  </head>
  <body>
    <h1>Big Title</h1>
    <h6>Small Title</h6>
  </body>
</html>
```

- `<!DOCTYPE html>` - 브라우저에게 html 문서임을 알려준다.
- `<head></head>` - 브라우저에게 웹사이트에 관한 필요한 정보를 제공
- `<body></body>` - 사람들이 읽는 컨텐츠 제공

### 4. meta tag

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="description" content="Welcome to HTML" />
    <meta name="author" content="Ian" />
    <title>This is my title</title>
  </head>
  <body>
    <h1>Big Title</h1>
    <h6>Small Title</h6>
  </body>
</html>
```

- meta tag - 추가정보라는 의미
- `<meta charset="utf-8">` - 브라우저에게 작성된 문서가 어떤 언어로 작성되었는지 알려준다.
- `<meta name="description" content="Welcome to HTML" />` - 검색엔진에서 검색할 때, 요약되서 나오는 내용
- `<meta name="author" content="Ian" />` - 브라우저에게 문서 작성자를 알려준다.

### 5. semantic tag와 non-semantic tag

- [semantic](https://www.w3schools.com/html/html5_semantic_elements.asp) - 의미가 있는 tag (header, nav, section, article, footer 등등..)

```html
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="description" content="Welcome to HTML" />
    <meta name="author" content="Ian" />
    <title>This is my title</title>
  </head>
  <body>
    <header>
      <h1>Big Title</h1>
    </header>
    <section>
      <div>Whatever</div>
    </section>
    <footer>
      <span>Something else</span>
    </footer>
  </body>
</html>
```

- non-semantic - 아무 의미가 없는 tag (div, span 등등...)

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="description" content="Welcome to HTML" />
    <meta name="author" content="Ian" />
    <title>This is my title</title>
  </head>
  <body>
    <h1>Big Title</h1>
    <div>Whatever</div>
    <span>Something else</span>
    <h6>Small Title</h6>
  </body>
</html>
```

### 6. tag에 이름을 주는법(id 와 class)

```html
<html>
  <head>
    <meta charset="utf-8" />
    <meta name="description" content="Welcome to HTML" />
    <meta name="author" content="Ian" />
    <title>This is my title</title>
  </head>
  <body>
    <section>
      <header id="headerNumberOne" class="defaultHeader">
        <h1>Big Title</h1>
      </header>
    </section>
    <div>
      <header id="diffrentHeader" class="defaultHeader">
        Title of the unkown container
      </header>
    </div>
  </body>
</html>
```

- css를 사용하기 위해서 id와 class를 사용한다.

|        |                    id                     |                 class |
| ------ | :---------------------------------------: | --------------------: |
| 사용성 | element마다 한개만 가져야 한다. 고유하다. | 여러개 사용 가능하다. |
