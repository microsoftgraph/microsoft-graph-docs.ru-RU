---
title: Список teamworkDeviceOperations
description: Получите список операций, связанных с устройством с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 998eef1ff0e90fa76456a1b3af7b2cb104d0fb21
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343409"
---
# <a name="list-teamworkdeviceoperations"></a>Список teamworkDeviceOperations
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список операций[,](../resources/teamworkdeviceoperation.md) которые работают на устройстве с Microsoft Teams [включенной поддержкой](../resources/teamworkdevice.md).

[!INCLUDE [teamworkdevice-api-disclaimer](../../includes/teamworkdevice-api-disclaimer.md)]

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamworkDevice.Read.All, TeamworkDevice.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|TeamworkDevice.Read.All, TeamworkDevice.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/devices/{teamworkDeviceId}/operations
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$top`, `$select` и `$skipToken` для настройки отклика.

### <a name="supported-query-patterns"></a>Поддерживаемые шаблоны запросов

| Шаблон                | Синтаксис                                 | Примечания |
| ---------------------- | -------------------------------------- | ----- |
| Pagination на стороне сервера | `@odata.nextLink`                      | В ответе вы получите маркер продолжения, если набор результатов охватывает несколько страниц. |
| Ограничение страницы                 | `/devices({deviceId})/operations?$top=10` | Получите операции для устройства с размером страницы 10. Ограничение страницы по умолчанию — 20. Максимальное ограничение страницы — 50. |

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной `200 OK` работы этот метод возвращает код отклика и коллекцию объектов [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamworkdeviceoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/operations
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamworkdeviceoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamworkdeviceoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamworkdeviceoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamworkdeviceoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamworkdeviceoperation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-teamworkdeviceoperation-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDeviceOperation",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teamwork/devices('18129e1f')/operations",
  "@odata.count": 1,
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamworkDeviceOperation",
      "id": "eab261f8-61f8-eab2-f861-b2eaf861b2ea",
      "status": "successful",
      "operationType": "deviceDiagnostics",
      "error": {
        "code": null,
        "message": "Unknown"
      },
      "startedDateTime": "2021-06-19T12-01-03.45Z",
      "completedDateTime": "2021-06-19T12-01-03.45Z",
      "createdDateTime": "2021-06-19T12-01-03.45Z",
      "lastActionDateTime": "2021-06-19T12-01-03.45Z",
      "createdBy": {
        "application": null,
        "device": null,
        "user": {
          "id": "2a610f6f-adf6-4205",
          "displayName": "Evan Lewis",
          "userIdentityType": "aadUser"
        }
      },
      "lastActionBy": {
        "application": null,
        "device": null,
        "user": {
          "id": "2a610f6f-adf6-4205",
          "displayName": "Evan Lewis",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

