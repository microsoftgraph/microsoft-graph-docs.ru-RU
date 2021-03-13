---
title: тип ресурса domainDnsSrvRecord
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5b3355115f11937584879725073cd4a4c279c62d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761676"
---
# <a name="domaindnssrvrecord-resource-type"></a>тип ресурса domainDnsSrvRecord

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)

## <a name="methods"></a>Методы
Прямые запросы на этот ресурс не поддерживаются. Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, присвоенный этому объекту. Не является недействительным, только для чтения.|
|isOptional|Boolean| Если это неверно, запись SRV должна быть настроена клиентом на хост DNS, чтобы Microsoft Online Services правильно работать с доменом. |
|label|String| Значение, используемого при настройке *свойства* имени записи SRV в хосте DNS. |
|nameTarget|String| Значение, используемого при настройке *целевого* свойства записи SRV в хосте DNS. |
|порт|Int32| Значение, используемого при  настройке свойства порта записи SRV в хосте DNS. |
|priority|Int32| Значение, используемое при настройке *приоритетного* свойства записи SRV в хосте DNS. |
|протокол|String| Значение, используемого при настройке свойства *протокола* записи SRV в DNS-хозяйне. |
|recordType|String|  Тип записи DNS. Значение всегда *Srv*. Key |
|service|String| Значение, используемого при  настройке свойства службы записи SRV в DNS-хозяйне. |
|supportedService|String| Microsoft Online Service или функция, зависимая от этой записи SRV.</br></br>Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|ttl|Int32| Значение, используемого при настройке свойства "время на *жизнь"* записи SRV в DNS-хозяйне. Не является недействительным |
|weight|Int32| Значение, используемого при  настройке свойства веса записи SRV в хосте DNS. |

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


