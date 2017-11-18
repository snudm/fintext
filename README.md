
# Setting For New Products

### 1. `PRODUCT.html` 새로운 페이지 생성

기존에 존재하는 내용을 복사해오기 (BTIC/WBFS)
- 해당 Product에 해당하는 post만 나오도록 설정
```django
{% for post in site.categories.PRODUCT %}
```
- 상황에 맞게 고치기

### 2. `_includes/header.html`에 Tab 추가
- Button
```django
<li><a href="{{ site.baseurl }}/PRODUCT">PRODUCT</a></li>
```

- Dropdown
```django
<div class="dropdown">
  <button class="btn btn-default dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown" aria-haspopup="true" aria-expanded="true">
  PRODUCT <!--내용-->
  <span class="caret"></span> <!--화살표-->
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenu1"> <!-- 드랍다운 하위 아이템 내용 -->
    <li><a href="{{ site.baseurl }}/PRODUCT#section1">Section 1</a></li> <!--# 이후에PRODUCT.html에 있는 해당 section의 id를 입력 -->
    <li role="separator" class="divider"></li> <!-- 구분선 -->
    <li><a href="{{ site.baseurl }}/PRODUCT#section2">Section 2</a></li>
    <li><a href="{{ site.baseurl }}/PRODUCT#section3">Section 3</a></li>
  </ul>
</div>

```

`_includes/footer.html'에 Tab 추가 하기


# Theme : *Airspace* for Jekyll
![screenshot](screenshots/home.png "Description goes here")

This Jekyll theme is a port of ThemeFisher's Airspace template. It is released under ThemeFisher's free license, which requires attribution.
