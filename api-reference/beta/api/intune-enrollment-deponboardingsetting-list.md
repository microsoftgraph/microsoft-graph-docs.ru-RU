---
title: Список depOnboardingSettings
description: Свойства списка и связей объектов depOnboardingSetting.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 64b15a19943ee5d03861ffc39b2e74a006b12936
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394154"
---
# <a name="list-deponboardingsettings"></a>Список depOnboardingSettings

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Свойства списка и связей объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .

## <a name="prerequisites"></a>Предварительные требования
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depOnboardingSetting",
      "id": "40342229-2229-4034-2922-344029223440",
      "appleIdentifier": "Apple Identifier value",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
      "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
      "shareTokenWithSchoolDataSyncService": true,
      "lastSyncErrorCode": 1,
      "tokenType": "dep",
      "tokenName": "Token Name value",
      "syncedDeviceCount": 1,
      "dataSharingConsentGranted": true
    }
  ]
}
```




