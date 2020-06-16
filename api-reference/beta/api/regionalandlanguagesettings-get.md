---
title: Получение ресурса Регионаландлангуажесеттингс
description: Получение свойств объекта Регионаландлангуажесеттингс пользователя
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: 493af1c75e20552e9fb420402365894a04717e17
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744242"
---
# <a name="get-regionalandlanguagesettings"></a>Получение Регионаландлангуажесеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств объекта [регионаландлангуажесеттингс](../resources/regionalAndLanguageSettings.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                   |Разрешение (по крайней мере для самых привилегированных)     |
|----------------------------------|---------------------------------------------- |
|Делегированные (рабочая или учебная учетная запись)|User. Read, User. Read. ALL                        |
|Делегированная учетная запись (личная учетная запись)      |User. Read, User. Read. ALL              |
|Для приложений                       |User. Read, User. Read. ALL              |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /settings/regionalAndLanguageSettings
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Вы можете использовать `$select` для получения определенных свойств регионаландлангуажесеттингс, включая те, которые не возвращаются по умолчанию.

Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {токен}. Обязательный.|
| Content-Type   | application/json |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [регионаландлангуажесеттингс](../resources/regionalandlanguagesettings.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a>Пример 1. Получение свойств вошедшего пользователя

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_regionalAndLanguageSettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/regionalAndLanguageSettings
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "get_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "defaultDisplayLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "authoringLanguages": [
        {
            "locale": "fr-FR",
            "displayName": "French (France)"
        },
        {
            "locale": "de-DE",
            "displayName": "German (Germany)"
        },
    ],
    "defaultTranslationLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "defaultSpeechInputLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "defaultRegionalFormat": {
        "locale": "en-GB",
        "displayName": "English (United Kingdom)"
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

<!--
{
  "type": "#page.annotation",
  "description": "Get regionalAndLanguageSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
