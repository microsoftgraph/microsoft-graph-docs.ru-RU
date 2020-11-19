---
title: Тип ресурса Микрософттуннелконфигуратион
description: Объект, представляющий коллекцию параметров туннеля Microsoft
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4cd85d798085ed5d8caf12ae2becc58e2bf10a33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302026"
---
# <a name="microsofttunnelconfiguration-resource-type"></a>Тип ресурса Микрософттуннелконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий коллекцию параметров туннеля Microsoft

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Микрософттуннелконфигуратионс](../api/intune-mstunnel-microsofttunnelconfiguration-list.md)|Коллекция [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Список свойств и связей объектов [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Получение Микрософттуннелконфигуратион](../api/intune-mstunnel-microsofttunnelconfiguration-get.md)|[микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Чтение свойств и связей объекта [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Создание Микрософттуннелконфигуратион](../api/intune-mstunnel-microsofttunnelconfiguration-create.md)|[микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Создание нового объекта [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|
|[Удаление Микрософттуннелконфигуратион](../api/intune-mstunnel-microsofttunnelconfiguration-delete.md)|Нет|Удаляет объект [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md).|
|[Обновление Микрософттуннелконфигуратион](../api/intune-mstunnel-microsofttunnelconfiguration-update.md)|[микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Обновление свойств объекта [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор Микрософттуннелконфигуратион|
|displayName|String|Отображаемое имя Микрософттуннелконфигуратион|
|description|String|Описание Микрософттуннелконфигуратион|
|сетью|String|Подсеть, которая будет использоваться для выделения виртуального адреса для клиентов.|
|днссерверс|Коллекция строк|DNS-серверы, которые будут использоваться клиентами;|
|дефаултдомаинсуффикс|String|Приложение домена по умолчанию, которое будет использоваться клиентами.|
|раутесинклуде|Коллекция строк|Маршрутизации, которые будут маршрутизироваться сервером|
|раутесексклуде|Коллекция строк|Подмножества маршрутов, которые не будут маршрутизироваться сервером|
|сплитднс|Коллекция строк|Домены, которые будут разрешены с помощью предоставленных DNS-серверов|
|листенпорт|Int32|Порт, прослушиваемый портами TCP и UPD на сервере|
|адванцедсеттингс|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Дополнительные параметры, которые могут быть применены к серверу|
|lastUpdateDateTime|DateTimeOffset|При последнем обновлении Микрософттуннелконфигуратион|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности.|

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
  ]
}
```




