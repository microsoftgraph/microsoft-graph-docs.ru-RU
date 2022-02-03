---
title: Get teamworkDevice
description: Получите свойства устройства с Microsoft Teams, включая тип устройства, детали оборудования, состояние активности и сведения о состоянии здоровья.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 645ae373d0c0e13f7d1a17df6de8dd74e42a63d5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343335"
---
# <a name="get-teamworkdevice"></a>Get teamworkDevice
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите свойства устройства с Microsoft Teams [включенной поддержкой](../resources/teamworkdevice.md). Например, этот метод можно использовать для получения сведений о типе устройства, оборудовании, состоянии активности и состоянии здоровья для устройства, включенного для Teams.

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
GET /teamwork/devices/{teamworkDeviceId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Эта операция поддерживает параметр запроса `$select` [OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и [объект teamworkDevice](../resources/teamworkdevice.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworkdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworkdevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworkdevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworkdevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworkdevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-teamworkdevice-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-teamworkdevice-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDevice",
    "id": "0f3ce432-e432-0f3c-32e4-3c0f32e43c0f",
    "deviceType": "CollaborationBar",
    "hardwareDetail": {
      "serialNumber": "0189",
      "uniqueId": "5abcdefgh",
      "macAddresses": [],
      "manufacturer": "yealink",
      "model": "vc210"
    },
    "notes": "CollaborationBar device.",
    "companyAssetTag": "Tag1",
    "healthStatus": "Healthy",
    "activityState": "Idle",
    "createdDateTime": "2021-06-19T19:01:04.185Z",
    "createdBy": null,
    "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
    "lastModifiedBy": null,
    "currentUser": {
      "id": "2a610f6f-adf6-4205",
      "displayName": "Evan Lewis",
      "userIdentityType": "aadUser"
    }
  }
}
```

