---
title: Получите microsoftTunnelConfiguration
description: Чтение свойств и связей объекта microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6c0220944c2e68d63589c7bb2ac562bf36e93c7
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630648"
---
# <a name="get-microsofttunnelconfiguration"></a>Получите microsoftTunnelConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `200 OK` отклика и [объект microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 912

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
    "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
    "displayName": "Display Name value",
    "description": "Description value",
    "network": "Network value",
    "dnsServers": [
      "Dns Servers value"
    ],
    "defaultDomainSuffix": "Default Domain Suffix value",
    "routesInclude": [
      "Routes Include value"
    ],
    "routesExclude": [
      "Routes Exclude value"
    ],
    "splitDNS": [
      "Split DNS value"
    ],
    "listenPort": 10,
    "advancedSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "disableUdpConnections": true
  }
}
```




