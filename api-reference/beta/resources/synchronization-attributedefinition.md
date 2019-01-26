---
title: Тип ресурса attributeDefinition
description: Описывает атрибут объекта.
localization_priority: Normal
ms.openlocfilehash: 30c9d6b2f57aaadd9ef17982b1affa765bbfbec0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571865"
---
# <a name="attributedefinition-resource-type"></a>Тип ресурса attributeDefinition

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает атрибут объекта.

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|привязки         |Boolean    | `true`Если атрибут должен использоваться для привязки для объекта. Атрибуты привязки должны иметь уникальное значение, идентифицирующее объект и должны быть постоянным. Значение по умолчанию: `false`. Один и только один из атрибутов объекта должен быть назначен для привязки для поддержки синхронизации. |
|caseExact      |Boolean    |`true`Если значение этого атрибута следует учитывать регистр. Этот параметр влияет на как обработчик синхронизации обнаружены изменения в атрибуте.|
|метаданные       |[metadataEntry](../resources/synchronization-metadataentry.md) коллекции |Расширение дополнительные свойства. Если не указан явно, значения метаданных не должно изменяться.|
|многозначные    |Boolean    |`true`Если атрибут может содержать несколько значений. Значение по умолчанию: `false`.|
|изменения     |Строка     |Изменения атрибута. Возможные значения: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`. Значение по умолчанию: `ReadWrite`.|
|name           |Строка     |Имя атрибута. Должно быть уникальным в рамках определения объекта. Значение null не допускается.|
|Обязательный       |Boolean    |`true`Если атрибут является обязательным. Объект не может быть создан, если какие-либо обязательные атрибуты отсутствуют. Если во время синхронизации, обязательный атрибут не имеет значения, будет использоваться значение по умолчанию. Если значение по умолчанию не задано, синхронизация будет записана ошибка.|
|referencedObjects|[referencedObject](../resources/synchronization-referencedobject.md) коллекции |Для атрибутов с `reference` введите объекты списков (например, `manager` атрибут будет содержать `User` как указанный объект).|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
