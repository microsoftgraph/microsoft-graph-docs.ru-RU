---
title: Список Микрософттуннелконфигуратионс
description: Список свойств и связей объектов Микрософттуннелконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab1de746c6b289083ceb7256cc8382df36a0f7d2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242348"
---
# <a name="list-microsofttunnelconfigurations"></a>Список Микрософттуннелконфигуратионс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 950

{
  "value": [
    {
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
      ]
    }
  ]
}
```




