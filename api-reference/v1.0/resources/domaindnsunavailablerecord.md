---
title: Тип ресурса domainDnsUnavailableRecord
description: Когда вы запрашиваете свойство навигации **serviceConfigurationRecords** для объекта Domain, вы можете получить одну или несколько сущностей Домаинднскнамерекорд, Домаинднсмксрекорд, домаинднссрврекорд и/или домаинднсткстрекорд. Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен можно будет использовать в Microsoft Online Services. Если невозможно создать такие сущности, возвращается сущность DomainDnsUnavailableRecord. Наследуется от объекта DomainDnsRecord.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50616237d446f2feb22dd394e018a9a23bfe850b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531577"
---
# <a name="domaindnsunavailablerecord-resource-type"></a>Тип ресурса domainDnsUnavailableRecord

Пространство имен: microsoft.graph

Когда вы запрашиваете свойство навигации **serviceConfigurationRecords** для объекта [domain](domain.md) , вы можете получить одну или несколько сущностей [домаинднскнамерекорд](domaindnscnamerecord.md), [домаинднсмксрекорд](domaindnsmxrecord.md), [домаинднссрврекорд](domaindnssrvrecord.md)и/или [домаинднсткстрекорд](domaindnstxtrecord.md) . Эти сущности указывают, какие записи DNS необходимо добавить в файл зоны домена, прежде чем домен можно будет использовать в Microsoft Online Services. Если невозможно создать такие сущности, возвращается сущность DomainDnsUnavailableRecord. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|String|Предоставляет причину, по которой возвращается объект **DomainDnsUnavailableRecord** . |

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
