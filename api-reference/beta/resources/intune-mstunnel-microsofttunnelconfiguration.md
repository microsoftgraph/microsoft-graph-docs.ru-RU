---
title: тип ресурса microsoftTunnelConfiguration
description: Сущность, представляюая коллекцию параметров Microsoft Tunnel
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d560899a8f47448fd9377d7810125d10a6777960
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344843"
---
# <a name="microsofttunnelconfiguration-resource-type"></a>тип ресурса microsoftTunnelConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляюая коллекцию параметров Microsoft Tunnel

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список microsoftTunnelConfigurations](../api/intune-mstunnel-microsofttunnelconfiguration-list.md)|[коллекция microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Список свойств и связей объектов [microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|
|[Получите microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-get.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Чтение свойств и связей объекта [microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|
|[Создание microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-create.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Создайте [новый объект microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|
|[Удаление microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-delete.md)|Нет|Удаляет [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md).|
|[Обновление microsoftTunnelConfiguration](../api/intune-mstunnel-microsofttunnelconfiguration-update.md)|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Обновление свойств объекта [microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id MicrosoftTunnelConfiguration|
|displayName|Строка|Имя отображения MicrosoftTunnelConfiguration|
|description|String|Описание MicrosoftTunnelConfiguration|
|сеть|Строка|Подсеть, которая будет использоваться для выделения виртуального адреса для клиентов|
|dnsServers|Коллекция String|DNS-серверы, которые будут использоваться клиентами|
|defaultDomainSuffix|String|Приложение домена по умолчанию, которое будет использоваться клиентами|
|routesInclude|Коллекция String|Маршруты, которые будут маршрутить сервер|
|routesExclude|Коллекция String|Подмышы маршрутов, которые не будут маршрутиться сервером|
|splitDNS|Коллекция String|Домены, которые будут разрешены с помощью предоставленных dns-серверов|
|listenPort|Int32|Порт, который будут прослушивать TCP и UPD на сервере|
|advancedSettings|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Дополнительные параметры, которые могут быть применены к серверу|
|lastUpdateDateTime|DateTimeOffset|При последнем обновлении MicrosoftTunnelConfiguration|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|
|отключениеUDPConnections|Boolean|При задавке отключенияUDPConnections, клиенты и VPN-сервер не будут использовать connctions DTLS для обработки данных tansfer.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "network": "String",
  "dnsServers": [
    "String"
  ],
  "defaultDomainSuffix": "String",
  "routesInclude": [
    "String"
  ],
  "routesExclude": [
    "String"
  ],
  "splitDNS": [
    "String"
  ],
  "listenPort": 1024,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "lastUpdateDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "disableUDPConnections": true
}
```




