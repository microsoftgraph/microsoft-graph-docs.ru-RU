---
title: Обновление Регионаландлангуажесеттингс
description: Обновление региональных и языковых параметров пользователя
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: c84023c281dcda00db756a80f5d14668d213e727
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744245"
---
# <a name="update-regionalandlanguagesettings"></a>Обновление Регионаландлангуажесеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление некоторых или всех свойств объекта [регионаландлангуажесеттингс](../resources/regionalAndLanguageSettings.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                   |Разрешение (по крайней мере для самых привилегированных)     |
|----------------------------------|---------------------------------------------- |
|Делегированные (рабочая или учебная учетная запись)|User. ReadWrite, User. ReadWrite. ALL             |
|Делегированная учетная запись (личная учетная запись)      |User. ReadWrite, User. ReadWrite. ALL             |
|Для приложений                       |User. ReadWrite, User. ReadWrite. ALL             |

## <a name="http-request"></a>HTTP-запрос

Чтобы обновить региональные и языковые параметры пользователя, выполните указанные ниже действия.
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

Обновление подмножества свойств региональных и языковых параметров пользователя:
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса
 **Put**: в теле запроса добавьте объект [регионаландлангуажесеттингс](../resources/regionalAndLanguageSettings.md) .
 
 **Patch**: указывайте только значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.
 
## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код ответа 200 и обновленный объект Регионаландлангуажесеттингс

## <a name="example"></a>Пример

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a>Пример 1: обновление всего объекта Регионаландлангуажесеттингс пользователя, выполнившего вход в систему

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
    }
}
```

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a>Пример 2: Обновление выбранных свойств вошедшего пользователя

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

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
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
