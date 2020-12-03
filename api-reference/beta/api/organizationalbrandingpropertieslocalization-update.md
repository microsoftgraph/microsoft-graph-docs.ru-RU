---
title: Обновление локализованных организатионалбрандингпропертиес
description: Обновление свойств объекта организатионалбрандингпропертиес для определенной локализации.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 78e6ae581b1a4c0cbfd5fbff2f3814532c7491bb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49523970"
---
# <a name="update-localized-organizationalbrandingproperties"></a>Обновление локализованных организатионалбрандингпропертиес

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) для определенной локализации.

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
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
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
|id|String|Языковой стандарт для обновления фирменного стиля для|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 OK`.

## <a name="examples"></a>Примеры

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a>Пример 1: Настройка **баннерлого** для локализации FR с помощью метода PUT

Следующий запрос обновляет логотип баннера для локализации fr. Использование метода PUT, если локализация fr не существует, возвращается значение "404 Not Found". Если полезная нагрузка содержит свойство ID или заголовок Content-Language, и они не совпадают с идентификатором в URL-адресе, возвращается неверный запрос.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
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
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a>Пример 2: обновление **баннерлого** для локализации FR с использованием исправления

Следующий запрос обновляет логотип баннера для локализации fr.  С помощью PATCH, если указанная локализация еще не существует, она создается и в нее записывается свойство.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
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



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a>Пример 3: замена значения по умолчанию фирменной символикой на пустую строку

Если значение свойства при локализации равно null, значение будет унаследовано от фирменной символики по умолчанию. Чтобы избежать этого, задайте пустую строку или строку, содержащую только пробелы в локализованной фирменной символике.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
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

После этого запроса Усернамехинттекст для локализации будет пустым вместо того, чтобы наследовать значение из фирменной символики по умолчанию.

### <a name="example-4-replace-french-localization-with-put"></a>Пример 4: замена французской локализации на PUT

Чтобы выполнить обновление при локализации с помощью метода PUT, мы должны добавить все свойства в тексте вместе со свойством, которое необходимо обновить при замене существующего объекта новым. Для других свойств, которые не входят в текст полезных данных PUT, будет задано значение NULL. В примере ниже показано, что сохраняются только свойства Баккграундколор и Сигнинпажетекст обновляются, в то время как для других задано значение null.
Если указанная локализация еще не существует, укажите URL-адрес, указывающий на то, что локализация будет создана.
Если полезная нагрузка содержит свойство ID или заголовок Content-Language, и они не совпадают с идентификатором в URL-адресе, то возникает ошибочный запрос.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
