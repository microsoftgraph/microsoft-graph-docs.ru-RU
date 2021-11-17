---
title: Обновление regionalAndLanguageSettings
description: Обновление региональных и языковых параметров пользователя.
author: jasonbro
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: eed6912edd9252f73cec917098111024a634d5e0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996894"
---
# <a name="update-regionalandlanguagesettings"></a>Обновление regionalAndLanguageSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновим некоторые или все свойства объекта [regionalAndLanguageSettings.](../resources/regionalAndLanguageSettings.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                   |Разрешение (от наименее до самых привилегированных)     |
|----------------------------------|---------------------------------------------- |
|Делегированные (рабочая или учебная учетная запись)|User.ReadWrite, User.ReadWrite.All             |
|Делегированная (личная учетная запись)      |User.ReadWrite, User.ReadWrite.All             |
|Для приложений                       |User.ReadWrite, User.ReadWrite.All             |

## <a name="http-request"></a>HTTP-запрос

Обновление всех региональных и языковых параметров пользователя:
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

Обновление подмножество свойств региональных и языковых параметров пользователя:
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса
 **PUT.** В теле запроса поставьте [объект regionalAndLanguageSettings.](../resources/regionalAndLanguageSettings.md)
 
 **PATCH.** Только поставляем значения для соответствующих полей, которые должны быть обновлены. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.
 
## <a name="response"></a>Ответ

В случае успеха этот метод возвращает код ответа 200 и обновленный **объект regionalAndLanguageSettings.**

## <a name="example"></a>Пример

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a>Пример 1. Обновление всего объекта regionalAndLanguageSettings для подписанного пользователя

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_regionalAndLanguageSettings"
}-->
```http
PUT https://graph.microsoft.com/beta/me/settings/regionalandlanguagesettings
Content-type: application/json

{
    "defaultDisplayLanguage": {
        "locale": "en-US"
    },
    "authoringLanguages": [
        {
            "locale": "fr-FR"
        },
        {
            "locale": "de-DE"
        }
    ],
    "defaultTranslationLanguage": {
        "locale": "en-US"
    },
    "defaultSpeechInputLanguage": {
        "locale": "en-US"
    },
    "defaultRegionalFormat": {
        "locale": "en-GB"
    },
    "regionalFormatOverrides": {
        "calendar": "Gregorian Calendar",
        "firstDayOfWeek": "Sunday",
        "shortDateFormat": "yyyy-MM-dd",
        "longDateFormat": "dddd, MMMM d, yyyy",
        "shortTimeFormat": "HH:mm",
        "longTimeFormat": "h:mm:ss tt",
        "timeZone": "Pacific Standard Time"
    },
    "translationPreferences": {
        "translationBehavior": "Yes",
        "languageOverrides": [
            {
                "languageTag": "fr",
                "translationBehavior": "Yes" 
            }
        ]
     }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/put-regionalandlanguagesettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a>Пример 2. Обновление выбранных свойств подписанного пользователя

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_regionalAndLanguageSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/settings/regionalandlanguagesettings
Content-type: application/json

{
  "authoringLanguages": [
    {
     "locale": "en-US" },
    {
     "locale": "es-MX" }
  ],
  "defaultRegionalFormat": {
     "locale": "en-US"
   }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/patch-regionalandlanguagesettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "name": "patch_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update regionalAndLanguageSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


