---
title: Тип ресурса domainDnsUnavailableRecord
description: При запросе свойство навигации **serviceConfigurationRecords** для сущности домена, может получать один или несколько DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord или DomainDnsTxtRecord сущности. Эти сущности указывает, какие записи DNS, необходимо добавить в файл зоны домена, прежде чем домена можно использовать с Microsoft Online Services. Когда не возможно для создания таких сущностей, возвращается DomainDnsUnavailableRecord сущности. Наследуется от DomainDnsRecord сущности.
localization_priority: Normal
ms.openlocfilehash: 064fd294a89b48f6b7cfba58fa3d1076bf74a7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836185"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>Тип ресурса domainDnsUnavailableRecord

Когда вы запрашиваете объект [Domain](domain.md) в свойстве навигации **serviceConfigurationRecords**, то может быть возвращен один или несколько объектов [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) или [DomainDnsTxtRecord](domaindnstxtrecord.md). Эти объекты указывают, какие записи DNS необходимо добавить в файл зоны домена, чтобы службы Microsoft Online Services могли использовать этот домен. Если не удается создать такие объекты, то вместо них будет возвращен объект DomainDnsUnavailableRecord. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|описание|String|Указывает причину, по которой возвращен объект **DomainDnsUnavailableRecord**. |

## <a name="relationships"></a>Связи
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
