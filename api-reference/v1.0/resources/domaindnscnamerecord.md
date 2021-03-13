---
title: тип ресурса domainDnsCnameRecord
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2834aad1d0f46552eefbf2afba30b08f21924369
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761390"
---
# <a name="domaindnscnamerecord-resource-type"></a>тип ресурса domainDnsCnameRecord

Пространство имен: microsoft.graph

Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)


## <a name="methods"></a>Методы
Прямые запросы на этот ресурс не поддерживаются. Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|canonicalName|String| Каноническое имя записи CNAME. Используется для настройки записи CNAME в DNS-хозяйке. |
|id|String| Уникальный идентификатор, присвоенный этому объекту. Не является недействительным, только для чтения|
|isOptional|Boolean| Если это не так, запись CNAME должна быть настроена клиентом в хосте DNS, чтобы Microsoft Online Services правильно работать с доменом. Не является недействительным |
|label|String| Значение, используемого при настройке *псевдонима/хоста/имени* записи CNAME в хосте DNS. |
|recordType|String| Тип записи DNS. Значение всегда *CName*. Key|
|supportedService|String| Microsoft Online Service или функция, зависимая от этой записи CNAME.</br></br>Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Значение, используемого при настройке свойства "время на жизнь" записи CNAME в хосте DNS. Не является недействительным |

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

