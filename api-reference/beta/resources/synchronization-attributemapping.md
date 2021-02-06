---
title: Тип ресурса attributeMapping
description: Определяет поток значений для заданного целевого атрибута во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b5f120075b082e50a0f94f05907b413a4c4c4ec6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128752"
---
# <a name="attributemapping-resource-type"></a>Тип ресурса attributeMapping

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет поток значений для заданного целевого атрибута во время синхронизации.

## <a name="properties"></a>Свойства

| Свойство                  | Тип                      | Описание    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | Строка                    |Значение по умолчанию, используемее в случае, если свойство источника было оценено как  `null` . Необязательный параметр.|
|exportMissingReferences    |String                     |Только для внутреннего использования.|
|flowBehavior               |attributeFlowBehavior      |Определяет, когда этот атрибут должен экспортироваться в целевой каталог. Возможные значения: `FlowWhenChanged` и `FlowAlways` . Значение по умолчанию: `FlowWhenChanged`. |
|flowType                   |attributeFlowType          |Определяет время обновления этого атрибута в целевом каталоге. Возможные значения: (по умолчанию) (только при добавлении нового объекта) (только при добавлении новых значений в атрибут с несколькими `Always` `ObjectAddOnly` `MultiValueAddOnly` значениями). |
|matchingPriority           |Int32                      |Если больше 0, этот атрибут будет использоваться для первоначального совпадения объектов между исходным и целевым каталогами. Механизм синхронизации попытается найти совпадающий объект с помощью атрибута с наименьшим значением приоритета. Если этот атрибут не найден, будет использоваться атрибут с следующим совпадающий приоритетом и так далее до тех пор, пока совпадение не будет найдено или больше совпадающие атрибуты не будут оставлены. В качестве совпадающих атрибутов следует использовать только те атрибуты, которые должны иметь уникальные значения, например электронную почту.|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | Определяет, как значение должно быть извлечено (или преобразовано) из объекта-источника. |
|targetAttributeName        |Строка                     |Имя атрибута в целевом объекте. |

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": []
}
-->


