# Payloads для gruyere

## Payload 1

При переходе по ссылке `[https://google-gruyere.appspot.com/624951287337740559451525490507763176737/example]`. Параметр `example` можно заменить на пейлоад `<script>alert(document.cookies)</script>` для выполнения Reflected XSS инъекции в элементе `<div id="search-query-param">...</div>`, который покажет куки файлы пользователя

## Payload 2

Если при создании нового снипетта вставить в поле `<img src=1 onerror=alert(1)>`, алерт будет выполняться каждый раз, когда пользователь заходит на страницу "Snippets" или на главную (Stored XSS)

## Payload 3

Если в профиле в поле homepage ввести `<script>alert(document.cookies)</script>`, то при переходе по ссылке homepage с главной будет появляться алерт (Stored XSS)

## Payload 4

При переходе по адресу `https://https://google-gruyere.appspot.com/584100228911668795158296871158315456069/newaccount.gtl` `newaccount.gtl` можно заменить на пейлоад `<span>payload</span>` , и выведется надпись payload (Reflected XSS)

## Payload 5

На странице добавления нового сниппета можно вставить в поле ввода `<a onmouseover="alert('xss')" href="#"><p>наведи на текст</p></a>` (Stored XSS)

## Payload 6

Если в профиле в поле homepage ввести `<img src=1 onerror=alert(1)>`, то при переходе по ссылке homepage с главной будет появляться алерт (Stored XSS)
