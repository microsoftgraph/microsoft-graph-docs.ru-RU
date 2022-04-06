---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
author: sandeo-MSFT
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 32bbd1e31a02662f31abaff2ed61845ec663d52f
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63670567"
---
# <a name="list-devices"></a>Список устройств

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка устройств, зарегистрированных в каталоге. 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------- |:------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись) | Device.Read.All, Directory.Read.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select` и `$top` для настройки отклика. Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

## <a name="request-headers"></a>Заголовки запросов

| Имя | Описание |
|:---- |:----------- |
| Авторизация  | Bearer {token}. Обязательный. |
| ConsistencyLevel | необязательный. Этот заголовок и `$count` требуются при использовании `$search` или определенном использовании `$filter`. Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries). |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-a-list-of-devices"></a>Пример 1. Получить список устройств

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-devices-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-devices-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
> Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-devices"></a>Пример 2. Получить только количество устройств

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$count`. Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

>**Примечание.** В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

294
```



### <a name="example-3-list-all-devices-and-return-only-their-id-and-extensionattributes-properties"></a>Пример 3. Список всех устройств и возвращение только их свойств id и extensionAttributes

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_select"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$select=id,extensionAttributes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-select-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-select-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-select-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-select-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-devices-select-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-devices-select-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices(id,extensionAttributes)",
    "value": [
        {
            "id": "6a59ea83-02bd-468f-a40b-f2c3d1821983",
            "extensionAttributes": {
                "extensionAttribute1": null,
                "extensionAttribute2": null,
                "extensionAttribute3": null,
                "extensionAttribute4": null,
                "extensionAttribute5": null,
                "extensionAttribute6": null,
                "extensionAttribute7": null,
                "extensionAttribute8": null,
                "extensionAttribute9": null,
                "extensionAttribute10": null,
                "extensionAttribute11": null,
                "extensionAttribute12": null,
                "extensionAttribute13": null,
                "extensionAttribute14": null,
                "extensionAttribute15": null
            }
        }
    ]
}
```

### <a name="example-4-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a>Пример 4. $filter и $top для получения одного устройства с именем отображения, которое начинается с "a", включая количество возвращенных объектов

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`. Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

>**Примечание.** В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.
<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#devices",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0",
      "hostNames":[]
    },
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000001",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Microsoft",
      "Model":"Surface",
      "operatingSystemVersion":"windows10EnterpriseN",
      "hostNames":["device_1.contoso.onmicrosoft.com", "device_1"]
    }
  ]
}
```

### <a name="example-5-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a>Пример 5. Использование $search для получения устройств с именами отображения, которые содержат буквы "Android", включая количество возвращенных объектов

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$search` и строка запроса `$count=true`. Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

>**Примечание.** В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#devices",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0",
      "hostNames":[]
    }
  ]
}
```

### <a name="example-6-get-devices-using-filter-on-extensionattributes"></a>Пример 6. Получить устройства с помощью фильтра на extensionAttributes

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. Для этого запроса требуется заглавная строка **ConsistencyLevel** `eventual` `$count=true` и строка запроса, так как свойство extensionAttributes `$filter` поддерживает только с расширенными параметрами запроса. Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).

>**Примечание.** В настоящее время параметры `$count` и `$search` недоступны в клиентах Azure AD B2C.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_by_extensionAttribute"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=extensionAttributes/extensionAttribute1 eq 'BYOD-Device'&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-by-extensionattribute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-by-extensionattribute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-by-extensionattribute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-by-extensionattribute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-devices-by-extensionattribute-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-devices-by-extensionattribute-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices",
    "@odata.count": 1,
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/6a59ea83-02bd-468f-a40b-f2c3d1821983/Microsoft.DirectoryServices.Device",
            "id": "6a59ea83-02bd-468f-a40b-f2c3d1821983",
            "accountEnabled": true,
            "approximateLastSignInDateTime": "2021-10-21T06:36:56Z",
            "createdDateTime": "2021-09-21T15:16:30Z",
            "deviceId": "eab73519-780d-4d43-be6d-a4a89af2a348",
            "displayName": "DESKTOP-LK3PESR",
            "operatingSystem": "Windows",
            "operatingSystemVersion": "10.0.19043.1237",
            "alternativeSecurityIds": [
                {
                    "type": 2,
                    "identityProvider": null,
                    "key": "WAA1ADAAOQA6AD...ADQAMwB5AGEAcQBnAD0A"
                }
            ],
            "extensionAttributes": {
                "extensionAttribute1": "BYOD-Device",
                "extensionAttribute2": null,
                "extensionAttribute3": null,
                "extensionAttribute4": null,
                "extensionAttribute5": null,
                "extensionAttribute6": null,
                "extensionAttribute7": null,
                "extensionAttribute8": null,
                "extensionAttribute9": null,
                "extensionAttribute10": null,
                "extensionAttribute11": null,
                "extensionAttribute12": null,
                "extensionAttribute13": null,
                "extensionAttribute14": null,
                "extensionAttribute15": null
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


