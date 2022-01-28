---
title: Get teamworkDeviceConfiguration
description: Сведения о конфигурации устройства с Microsoft Teams с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 026c005636efa76d8d783b701916789ee438d4f4
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262680"
---
# <a name="get-teamworkdeviceconfiguration"></a>Get teamworkDeviceConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите сведения [](../resources/teamworkdeviceconfiguration.md) о конфигурации устройства с [Microsoft Teams, включая](../resources/teamworkdevice.md) версии программного обеспечения, конфигурацию периферийных устройств (например, камеру, дисплей, микрофон и динамик), конфигурацию оборудования и Microsoft Teams конфигурацию клиента.

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
GET /teamwork/devices/{teamworkDeviceId}/configuration
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

В случае успешной `200 OK` работы этот метод возвращает код отклика и объект [teamworkDeviceConfiguration](../resources/teamworkdeviceconfiguration.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_teamworkdeviceconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/e19229ed-29ed-e192-ed29-92e1ed2992e1/configuration
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDeviceConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDeviceConfiguration",
    "id": "e19229ed-29ed-e192-ed29-92e1ed2992e1",
    "softwareVersions": {
      "adminAgentSoftwareVersion": "2020.7.10.1",
      "operatingSystemSoftwareVersion": "10.8.9.10",
      "teamsClientSoftwareVersion": "4.5.6.7",
      "firmwareSoftwareVersion": null,
      "partnerAgentSoftwareVersion": null
    },
    "displayConfiguration": {
      "displayCount": 1,
      "isDualDisplayModeEnabled": true,
      "isContentDuplicationAllowed": false,
      "configuredDisplays": [
        {
          "isOptional": false
        },
        {
          "isOptional": true
        }
      ],
      "inBuiltDisplayScreenConfiguration": null
    },
    "cameraConfiguration": {
      "contentCameraConfiguration": {
        "isContentCameraOptional": true,
        "isContentEnhancementEnabled": false,
        "isContentCameraInverted": false
      }
    },
    "speakerConfiguration": {
      "isSpeakerOptional": false,
      "isCommunicationSpeakerOptional": false
    },
    "microphoneConfiguration": {
      "isMicrophoneOptional": false
    },
    "teamsClientConfiguration": {
      "accountConfiguration": {
        "supportedClient": "teamsOnly",
        "onPremisesCalendarSyncConfiguration": {
          "smtpAddress": "john@contoso.com",
          "domainUserName": null,
          "domain": "contoso.com"
        }
      },
      "featuresConfiguration": {
        "isAutoScreenShareEnabled": false,
        "isHideMeetingNamesEnabled": false,
        "isBluetoothBeaconingEnabled": true,
        "isSendLogsAndFeedbackEnabled": true,
        "emailToSendLogsAndFeedback": "john@contoso.com"
      }
    },
    "hardwareConfiguration": {
      "processorModel": "Intel(R) Core(TM) i5-7300U CPU @ 2.60GHz"
    },
    "systemConfiguration": null,
    "createdDateTime": "2021-03-19T19:00:04.000Z",
    "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
    "createdBy": null,
    "lastModifiedBy": null
  }
}
```

