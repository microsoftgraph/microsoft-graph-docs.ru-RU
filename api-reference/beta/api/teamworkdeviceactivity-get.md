---
title: Получить teamworkDeviceActivity
description: Получите состояние активности устройства с Microsoft Teams с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: cd55e6e939aa96c2ce879b657fcf4ebe9e38b196
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262686"
---
# <a name="get-teamworkdeviceactivity"></a>Получить teamworkDeviceActivity
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите [состояние активности](../resources/teamworkdeviceactivity.md) устройства с Microsoft Teams с включенной [поддержкой](../resources/teamworkdevice.md). 

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
GET /teamwork/devices/{teamworkDeviceId}/activity
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Эта операция поддерживает параметры `$select` `$expand` [запроса oData и OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и [объект teamworkDeviceActivity](../resources/teamworkdeviceactivity.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_teamworkdeviceactivity"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/1ae3fe60-fe60-1ae3-60fe-e31a60fee31a/activity
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDeviceActivity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDeviceActivity",
    "id": "1ae3fe60-fe60-1ae3-60fe-e31a60fee31a",
    "activePeripherals": {
      "roomCamera": null,
      "contentCamera": null,
      "speaker": {
        "id": "Headset Earphone (Logitech SmartDock)",
        "displayName": "Headset Earphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
      "communicationSpeaker": {
        "id": "Headset Earphone (Logitech SmartDock)",
        "displayName": "Headset Earphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
      "microphone": {
        "id": "Headset Microphone (Logitech SmartDock)",
        "displayName": "Headset Microphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
    },
    "createdDateTime": "2021-03-19T19:00:04.000Z",
    "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
    "createdBy": null,
    "lastModifiedBy": null
  }
}
```

