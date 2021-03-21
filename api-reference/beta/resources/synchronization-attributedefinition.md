---
title: тип ресурса attributeDefinition
description: Описывает атрибут объекта.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a9c50721c1ee19505edc2507313cc346a6adabfd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956816"
---
# <a name="attributedefinition-resource-type"></a>тип ресурса attributeDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает атрибут объекта.

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|якорь         |Boolean    | `true` если атрибут должен использоваться в качестве якоря для объекта. Атрибуты Anchor должны иметь уникальное значение, определяющие объект, и должны быть неоменяемыми. Значение по умолчанию: `false`. Один и только один атрибуты объекта должны быть назначены в качестве якоря для поддержки синхронизации. |
|caseExact      |Boolean    |`true` если значение этого атрибута должно рассматриваться как чувствительное к делу. Этот параметр влияет на то, как механизм синхронизации обнаруживает изменения атрибута.|
|flowNullValues |Boolean    |"True", чтобы разрешить значения null для атрибутов.|
|метаданные       |[коллекция metadataEntry](../resources/synchronization-metadataentry.md)   |Дополнительные свойства расширения. Если не упомянуть явно, значения метаданных не следует менять.|
|многооценная    |Boolean    |`true` если атрибут может иметь несколько значений. Значение по умолчанию: `false`.|
|мутируемость     |мутируемость     |Мутируемость атрибута. Возможные значения:  `ReadWrite` `ReadOnly` , , `Immutable` `WriteOnly` . Значение по умолчанию: `ReadWrite`.|
|name           |String     |Имя атрибута. Должно быть уникальным в определении объекта. Значение null не допускается.|
|Обязательный       |Boolean    |`true` если атрибут необходим. Объект не может быть создан, если отсутствуют какие-либо из необходимых атрибутов. Если во время синхронизации необходимый атрибут не имеет значения, будет использоваться значение по умолчанию. Если по умолчанию значение не установлено, синхронизация зафиксировать ошибку.|
|referencedObjects|[коллекция referencedObject](../resources/synchronization-referencedobject.md) |Для атрибутов с типом перечислены ссылки на объекты (например, атрибут будет `reference` `manager` перечисляться как `User` объект со ссылкой).|
|type           |attributeType     |Тип значения атрибута. Возможные значения: `String` `Integer` , , , `Reference` , `Binary` `Boolean` `DateTime` . Значение по умолчанию: `String`.|

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


