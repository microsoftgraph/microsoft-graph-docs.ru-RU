---
title: Обновление Организатионалбрандингпропертиес
description: Обновление свойств объекта Организатионалбрандингпропертиес.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd8eb2976fc3e8309f804714babbd45474574455
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524465"
---
# <a name="update-organizationalbrandingproperties"></a>Обновление Организатионалбрандингпропертиес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Organization.ReadWrite.All |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |
| Content — Language  | Языковой стандарт. Необязательный параметр.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|баккграундколор|String|Цвет, который будет отображаться вместо фонового изображения в подключениях с низкой пропускной способностью. Рекомендуется использовать основной цвет эмблемы баннера или цвет вашей организации. Укажите в шестнадцатеричном формате (например, белый #FFFFFF).|
|Изображение|Stream|Изображение, отображаемое в качестве фона страницы входа. файлы PNG или jpg не больше 1920x1080 и меньше 300kb. Изображение меньшего размера уменьшит требования к пропускной способности и сделает загрузку страниц более производительной.|
|баннерлого|Stream|На странице входа отображается плакатная эмблема компании. файлы PNG или jpg не больше 36x245px. Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.|
|сигнинпажетекст|String|Текст, который отображается в нижней части поля входа. Вы можете использовать эту возможность для передачи дополнительных сведений, таких как номер телефона в службу поддержки или юридический отчет. Этот текст должен быть Юникодом и не превышать 1024 символов.|
|скуарелого|Stream|Квадратная версия логотипа компании. Эта функция отображается в режиме готовности к работе с Windows 10 (OOBE) и при включенном развертывании Windows. файлы PNG или jpg не имеют размер больше 240x240px и не больше 10Kb. Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.|
|усернамехинттекст|String|Строка, которая отображается как подсказка в текстовом поле имя пользователя на экране входа. Этот текст должен быть Юникодом без ссылок или кода и не может содержать более 64 символов.|

Свойство **ID** игнорируется при передаче.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 OK`.

## <a name="examples"></a>Примеры
### <a name="example-1-update-default-branding"></a>Пример 1: обновление фирменной символики по умолчанию
Если фирменная символика уже существует, то функция PATCH заменяет только указанные свойства, оставляя неопределенные свойства без изменений. 
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
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

В этом случае значения/брандинг по умолчанию обновляются, но при локализации значения не изменяются.

### <a name="example-2-update-bannerlogo-for-default-branding"></a>Пример 2: Update Баннерлого для фирменной символики по умолчанию
Следующий запрос обновляет логотип баннера для фирменной символики по умолчанию.
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
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

### <a name="example-3-update-localized-branding"></a>Пример 3: обновление локализованной фирменной символики
Если указан заголовок Content-Language, создается локализация, связанная с языком содержимого, если она еще не существует, а затем она обновляется с использованием указанных значений. Фирменная символика по умолчанию не изменяется.
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
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

После этого запроса локализация fr обновляется новым значением Баккграундколор, но в/брандинг. по умолчанию не вносятся изменения.

### <a name="example-4-replace-default-branding-and-all-localizations"></a>Пример 4: замена фирменного стиля по умолчанию и всех локализаций
Если фирменная символика уже существует, при РАЗМЕЩЕНии будут заменены фирменные настройки по умолчанию и все локализации.
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
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

В соответствии с этим запросом фирменная символика по умолчанию имеет только указанный Баккграундколор и имеет только одну локализацию с идентификатором fr, а также набор Баккграундколор.
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
