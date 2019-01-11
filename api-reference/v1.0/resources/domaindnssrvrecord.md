---
title: Тип ресурса domainDnsSrvRecord
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 655dc6fcbccdcb6e1794c94d97dd8e7fc4837f04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835793"
---
# <a name="domaindnssrvrecord-resource-type"></a>Тип ресурса domainDnsSrvRecord

Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка| Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.|
|isOptional|Boolean| Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись SRV на узле DNS. |
|label|String| Значение, используемое при настройке свойства *name* записи SRV на узле DNS. |
|nameTarget|String| Значение, используемое при настройке свойства *Target* записи SRV на узле DNS. |
|port|Int32| Значение, используемое при настройке свойства *port* записи SRV на узле DNS. |
|priority|Int32| Значение, используемое при настройке свойства *priority* записи SRV на узле DNS. |
|protocol|String| Значение, используемое при настройке свойства *protocol* для записи SRV на узле DNS. |
|recordType|String|  Тип записи DNS. Это свойство всегда имеет значение *Srv*. Ключ. |
|service|String| Значение, используемое при настройке свойства *service* для записи SRV на узле DNS. |
|supportedService|String| Служба или компонент Microsoft Online Services, зависящие от этой записи типа SRV.</br></br>Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*. |
|ttl|Int32| Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null. |
|weight|Int32| Значение, используемое при настройке свойства *weight* записи SRV на узле DNS. |

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
