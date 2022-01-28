---
title: Get teamworkDeviceOperation
description: Сведения о длительной операции async на устройстве с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 42b8b2467a45b31158dcbbe3c3b3db0712e5ebf2
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262674"
---
# <a name="get-teamworkdeviceoperation"></a>Get teamworkDeviceOperation
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о длительной операции async на устройстве с Microsoft Teams [включенной поддержкой](../resources/teamworkdeviceoperation.md).

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
GET /teamwork/devices/{teamworkDeviceId}/operations/{teamworkDeviceOperationId}
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

В случае успешной работы этот метод возвращает код `200 OK` отклика и объект [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_teamworkdeviceoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/operations/eab261f8-61f8-eab2-f861-b2eaf861b2ea
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDeviceOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDeviceOperation",
    "id": "eab261f8-61f8-eab2-f861-b2eaf861b2ea",
    "status": "successful",
    "operationType": "deviceRestart",
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
}
```

