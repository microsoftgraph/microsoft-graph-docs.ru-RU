---
title: тип ресурса domainDnsCnameRecord
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 63151892c0e4d18e692cf740bd8b0bb711dcd1e2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062770"
---
# <a name="domaindnscnamerecord-resource-type"></a>тип ресурса domainDnsCnameRecord

Пространство имен: microsoft.graph

Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)


## <a name="methods"></a>Методы
Прямые запросы на этот ресурс не поддерживаются. Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|canonicalName|Строка| Каноническое имя записи CNAME. Используется для настройки записи CNAME в DNS-хозяйке. |
|id|Строка| Уникальный идентификатор, присвоенный этому объекту. Не является недействительным, только для чтения|
|isOptional|Логический| Если это не так, запись CNAME должна быть настроена клиентом в хосте DNS, чтобы Microsoft Online Services правильно работать с доменом. Не является недействительным |
|подпись|String| Значение, используемого при настройке *псевдонима/хоста/имени* записи CNAME в хосте DNS. |
|recordType|String| Тип записи DNS. Значение всегда *CName*. Key|
|supportedService|String| Microsoft Online Service или функция, зависимая от этой записи CNAME.</br></br>Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Значение, используемого при настройке свойства "время на жизнь" записи CNAME в хосте DNS. Не является недействительным |

## <a name="relationships"></a>Отношения
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

