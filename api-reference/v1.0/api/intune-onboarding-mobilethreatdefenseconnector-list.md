---
title: Список объектов mobileThreatDefenseConnector
description: Список свойств и связей объектов mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40fc0270cb2057f92e0200a2b72db198fa3a4cc41b7a4c2ee32e8d9a01e9fa29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155598"
---
# <a name="list-mobilethreatdefenseconnectors"></a>Список объектов mobileThreatDefenseConnector

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
      "id": "e4bede14-de14-e4be-14de-bee414debee4",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "available",
      "androidEnabled": true,
      "iosEnabled": true,
      "androidDeviceBlockedOnMissingPartnerData": true,
      "iosDeviceBlockedOnMissingPartnerData": true,
      "partnerUnsupportedOsVersionBlocked": true,
      "partnerUnresponsivenessThresholdInDays": 6
    }
  ]
}
```




