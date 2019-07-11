---
title: Тип ресурса Аттрибутедефинитион
description: Описывает атрибут объекта.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 73e218ffce2d77d0e0f716d86c74e60224fb15fb
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620404"
---
# <a name="attributedefinition-resource-type"></a>Тип ресурса Аттрибутедефинитион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает атрибут объекта.

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|сами         |Boolean    | `true`значение, если атрибут должен использоваться в качестве привязки объекта. Атрибуты привязки должны иметь уникальное значение, определяющее объект, и должны быть неизменными. Значение по умолчанию: `false`. Только один из атрибутов объекта должен быть назначен в качестве привязки для поддержки синхронизации. |
|Касиксакт      |Boolean    |`true`Если значение этого атрибута должно обрабатываться с учетом регистра. Этот параметр влияет на то, как обработчик синхронизации обнаруживает изменения атрибута.|
|метаданных       |Коллекция [метадатаентри](../resources/synchronization-metadataentry.md)   |Дополнительные свойства расширения. Если явно не указано иное, значения метаданных не должны изменяться.|
|многозначных    |Boolean    |`true`Если атрибут может иметь несколько значений. Значение по умолчанию: `false`.|
|измен     |String     |Изменяемость атрибута. `ReadWrite`Возможные значения: `ReadOnly`,, `Immutable`,. `WriteOnly` Значение по умолчанию: `ReadWrite`.|
|name           |String     |Имя атрибута. Должно быть уникальным в пределах определения объекта. Значение null не допускается.|
|Обязательный       |Boolean    |`true`Если атрибут является обязательным. Объект не может быть создан, если отсутствует необходимый атрибут. Если во время синхронизации атрибуту required не присвоено значение, будет использоваться значение по умолчанию. Если значение по умолчанию не задано, то при синхронизации будет записано сообщение об ошибке.|
|Референцедобжектс|Коллекция [референцедобжект](../resources/synchronization-referencedobject.md) |Для атрибутов с `reference` типом перечисляет объекты, на которые имеются ссылки (например `manager` , атрибут будет `User` указан в качестве упоминаемого объекта).|
|type           |String     |Тип значения атрибута. Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`. Значение по умолчанию: `String`.|

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
