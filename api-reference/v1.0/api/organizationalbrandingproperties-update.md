---
title: Обновление организационнойБрендингПредложений
description: Обновление свойств организационного объектаBrandingProperties.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 95bf7425fff3ac48bd74920d7792e56d0d360f82
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547227"
---
# <a name="update-organizationalbrandingproperties"></a>Обновление организационнойБрендингПредложений

Обновление свойств организационного [объектаBrandingProperties.](../resources/organizationalbrandingproperties.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{tenant id}/branding/{property name}
PUT /organization/{tenant id}/branding/{property name}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |
| Контент-язык  | место действия. Необязательно.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|фонКолор|String|Цвет, который появится вместо фонового изображения в соединениях с низкой пропускной способностью. Основной цвет вашего логотипа баннера или цвета организации рекомендуется использовать здесь. Укажите это в шестигодной (например, белый #FFFFFF).|
|backgroundImage|Stream|Изображение, которое отображается в качестве фона знака на странице. .png или .jpg больше, чем 1920x1080 и меньше, чем 300kb. Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более выполнения.|
|баннерЛого|Stream|Баннерная версия логотипа вашей компании, которая появляется на странице ва-г. .png или .jpg не больше 36x245px. Мы рекомендуем использовать прозрачное изображение без обивки вокруг логотипа.|
|знакInPageText|String|Текст, который появляется в нижней части окна. Вы можете использовать это для передачи дополнительной информации, такой как номер телефона в службу поддержки или юридическое заявление. Этот текст должен быть Unicode и не превышать 1024 символов.|
|squareLogo|Stream|Квадратная версия логотипа вашей компании. Это отображается Windows 10 вне коробки (OOBE) и когда Windows автопилот включен для развертывания. .png или .jpg не более 240x240px и не более 10kb в размере. Мы рекомендуем использовать прозрачное изображение без обивки вокруг логотипа.|
|имя пользователяХитТекст|String|Строка, которая показывает, как намек в текстовом ящике имени пользователя на знаке на экране. Этот текст должен быть Unicode, без ссылок или кода, и не может превышать 64 символов.|

Свойство **id** игнорируется при его совеществе.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры
### <a name="example-1-update-default-branding"></a>Пример 1: Обновление брендинга по умолчанию
Если брендинг уже существует, `PATCH` заменит только указанные свойства, оставляя неопределенные свойства без изменений. 
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_1"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

В этом случае значения брендинга по умолчанию обновляются, но значения не меняются при локализации.

### <a name="example-2-update-bannerlogo-for-default-branding"></a>Пример 2: Обновление bannerLogo для брендинга по умолчанию
Следующий запрос обновляет логотип баннера для брендинга по умолчанию.
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_2"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a>Пример 3: Обновление локализованного брендинга
Если **указан заголовок Content-Language,** локализация, связанная с **Content-Language, сначала** создается, если его еще нет, а затем обновляется с использованием указанных значений. Брендинг по умолчанию не изменился.
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_3"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

После этого запроса локализация `fr` обновляется с новым значением **backgroundColor, но никаких** изменений в брендинг по умолчанию не велась.

### <a name="example-4-replace-default-branding-and-all-localizations"></a>Пример 4: Заменить брендинг по умолчанию и все локализации
Если брендинг уже существует, `PUT` заменит брендинг по умолчанию и любые локализации.
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_4"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

После этого запроса, брендинг по умолчанию имеет **только фонКолор** указан и имеет ровно одну локализацию **с идентификатором** `fr` , также с **набором backgroundColor.**
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
