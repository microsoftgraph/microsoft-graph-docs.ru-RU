---
title: Тип ресурса domainDnsUnavailableRecord
description: При запросе свойство навигации **serviceConfigurationRecords** для сущности домена, может получать один или несколько DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord или DomainDnsTxtRecord сущности. Эти сущности указывает, какие записи DNS, необходимо добавить в файл зоны домена, прежде чем домена можно использовать с Microsoft Online Services. Когда не возможно для создания таких сущностей, возвращается DomainDnsUnavailableRecord сущности. Наследуется от DomainDnsRecord сущности.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99da0448d75375b84bb37c05102c1f702c222a25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982794"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>Тип ресурса domainDnsUnavailableRecord

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
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
