---
title: Тип ресурса attributeMapping
description: Определяет, как значения для атрибута заданный целевой поток во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641878"
---
# <a name="attributemapping-resource-type"></a>Тип ресурса attributeMapping

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как значения для атрибута заданный целевой поток во время синхронизации.

## <a name="properties"></a>Свойства

| Свойство                  | Тип                      | Описание    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | String                    |По умолчанию значение для использования в случае, если свойство **source** проверялись `null`. Необязательный параметр.|
|exportMissingReferences    |String                     |Только для внутреннего использования.|
|flowBehavior               |attributeFlowBehavior      |Определяет, когда этот атрибут, должны быть экспортированы в конечный каталог. Возможные значения: `FlowWhenChanged` и `FlowAlways`. Значение по умолчанию: `FlowWhenChanged`. |
|flowType                   |attributeFlowType          |Определяет, когда этот атрибут следует обновить в целевой каталог. Возможные значения: `Always` (по умолчанию), `ObjectAddOnly` (только если создается новый объект), `MultiValueAddOnly` (только при изменении добавляет новые значения это многозначный атрибут). |
|matchingPriority           |Int32                      |Если больше 0, этот атрибут будет использоваться для выполнения первоначальной совпадение объектов между исходный и конечный каталоги. Обработчик синхронизации попытается найти соответствующий объект, с помощью атрибута с наименьшее значение сначала совпадающих приоритет. Если не найден, атрибута с помощью следующего соответствия приоритет будет использоваться и так далее до совпадения или исключаются соответствующие атрибуты. Только атрибуты, которые должны иметь уникальные значения, такие как электронной почтой, следует использовать в качестве соответствующие атрибуты.|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта. |
|targetAttributeName        |String                     |Имя атрибута для конечного объекта. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
