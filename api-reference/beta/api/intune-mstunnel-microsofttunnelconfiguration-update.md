---
title: Обновление microsoftTunnelConfiguration
description: Обновление свойств объекта microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f81e06a1ca75f53e35d64745a3aed937f28eced6
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64628968"
---
# <a name="update-microsofttunnelconfiguration"></a>Обновление microsoftTunnelConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса предоставляем представление JSON для [объекта MicrosoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .

В следующей таблице показаны свойства, необходимые при создании [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Id MicrosoftTunnelConfiguration|
|displayName|Строка|Имя отображения MicrosoftTunnelConfiguration|
|description|Строка|Описание MicrosoftTunnelConfiguration|
|сеть|Строка|Подсеть, которая будет использоваться для выделения виртуального адреса для клиентов|
|dnsServers|Коллекция String|DNS-серверы, которые будут использоваться клиентами|
|defaultDomainSuffix|Строка|Приложение домена по умолчанию, которое будет использоваться клиентами|
|routesInclude|Коллекция String|Маршруты, которые будут маршрутить сервер|
|routesExclude|Коллекция String|Подмышы маршрутов, которые не будут маршрутиться сервером|
|splitDNS|Коллекция объектов string|Домены, которые будут разрешены с помощью предоставленных dns-серверов|
|listenPort|Int32|Порт, который будут прослушивать TCP и UPD на сервере|
|advancedSettings|Коллекция [keyValuePair](../resources/intune-mstunnel-keyvaluepair.md)|Дополнительные параметры, которые могут быть применены к серверу|
|lastUpdateDateTime|DateTimeOffset|При последнем обновлении MicrosoftTunnelConfiguration|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|
|отключениеUdpConnections|Логическое|При наборе disableUdpConnections клиенты и VPN-сервер не будут использовать подключения DTLS для данных tansfer.|



## <a name="response"></a>Отклик
В случае успешной `200 OK` работы этот метод возвращает код отклика и обновленный [объект microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
Content-type: application/json
Content-length: 782

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
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
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 831

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
  ],
  "disableUdpConnections": true
}
```




