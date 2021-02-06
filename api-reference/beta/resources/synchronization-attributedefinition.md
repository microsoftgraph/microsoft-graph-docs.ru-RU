---
title: Тип ресурса attributeDefinition
description: Описывает атрибут объекта.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 34503f3edf15542db449d56e5211cd33b3d9132e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128815"
---
# <a name="attributedefinition-resource-type"></a>Тип ресурса attributeDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает атрибут объекта.

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|anchor         |Boolean    | `true` если атрибут должен использоваться в качестве привязки для объекта. Атрибуты привязки должны иметь уникальное значение, идентифицирующие объект, и должны быть неуменяемыми. Значение по умолчанию: `false`. Один и только один атрибуты объекта должны быть назначены в качестве привязки для поддержки синхронизации. |
|caseExact      |Boolean    |`true` если значение этого атрибута должно рассматриваться как чувствительный к делу. Этот параметр влияет на то, как механизм синхронизации обнаруживает изменения атрибута.|
|flowNullValues |Boolean    |Значение true позволяет использовать значения null для атрибутов.|
|метаданные       |[Коллекция metadataEntry](../resources/synchronization-metadataentry.md)   |Дополнительные свойства расширения. Если не было явно упомянуто, значения метаданных не следует менять.|
|multivalued    |Boolean    |`true` если атрибут может иметь несколько значений. Значение по умолчанию: `false`.|
|mutability     |Строка     |Мутируемость атрибута. Возможные значения:  `ReadWrite` , , , `ReadOnly` `Immutable` `WriteOnly` . Значение по умолчанию: `ReadWrite`.|
|name           |String     |Имя атрибута. Должен быть уникальным в определении объекта. Значение null не допускается.|
|Обязательный       |Boolean    |`true` если атрибут является требуемым. Объект не может быть создан, если отсутствуют какие-либо из необходимых атрибутов. Если во время синхронизации необходимый атрибут не имеет значения, будет использоваться значение по умолчанию. Если значение по умолчанию не установлено, при синхронизации будет записана ошибка.|
|referencedObjects|[коллекция referencedObject](../resources/synchronization-referencedobject.md) |Для атрибутов с типом перечисляются объекты, на которые ссылается ссылка (например, атрибут будет перечислен как объект, на `reference` `manager` который `User` ссылается ссылка).|
|type           |Строка     |Тип значения атрибута. Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`. Значение по умолчанию: `String`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "flowNullValues": true,
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


