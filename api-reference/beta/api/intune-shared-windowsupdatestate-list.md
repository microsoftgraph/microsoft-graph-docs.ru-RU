---
title: Список Виндовсупдатестатес
description: Список свойств и связей объектов Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f0f0db89147d674115c44de6ae8d3faf39aeb65
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457910"
---
# <a name="list-windowsupdatestates"></a>Список Виндовсупдатестатес

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
| &nbsp; &nbsp; **Конфигурация устройства** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
| &nbsp;&nbsp; **Обновление программного обеспечения** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений||
| &nbsp; &nbsp; **Конфигурация устройства** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
| &nbsp;&nbsp; **Обновление программного обеспечения** | DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 630

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateState",
      "id": "3d92af00-af00-3d92-00af-923d00af923d",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "status": "pendingInstallation",
      "qualityUpdateVersion": "Quality Update Version value",
      "featureUpdateVersion": "Feature Update Version value",
      "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
    }
  ]
}
```








