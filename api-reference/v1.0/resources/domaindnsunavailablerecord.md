---
title: тип ресурса domainDnsUnavailableRecord
description: Указывает, что службыConfigurationRecords не могут быть созданы.
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: cda989c9033818efe7f750467783bb5f2ce517a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123764"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>тип ресурса domainDnsUnavailableRecord

Пространство имен: microsoft.graph

При запросе службы свойств навигацииConfigurationRecords для объекта домена вы можете получить обратно одно или несколько объектов [DomainDnsCnameRecord,](domaindnscnamerecord.md) [DomainDnsMxRecord,](domaindnsmxrecord.md) [DomainDnsSrvRecord](domaindnssrvrecord.md)и/или  [](domain.md) [объекты DomainDnsTxtRecord.](domaindnstxtrecord.md) Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен может использоваться Microsoft Online Services. Если создание таких сущностей невозможно, возвращается объект DomainDnsUnavailableRecord. Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)

## <a name="methods"></a>Методы
Прямые запросы на этот ресурс не поддерживаются. Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|Строка|Предоставляет причину, по которой **возвращается объект DomainDnsUnavailableRecord.** |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

