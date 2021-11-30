---
title: тип ресурса attributeMapping
description: Определяет, как должны поступать значения для данного целевого атрибута во время синхронизации.
ms.localizationpriority: medium
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d66937d1951bd3fa65db6f17b70fd0df2a6de534
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224772"
---
# <a name="attributemapping-resource-type"></a>тип ресурса attributeMapping

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как должны поступать значения для данного целевого атрибута во время синхронизации.

## <a name="properties"></a>Свойства

| Свойство                  | Тип                      | Описание    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | Строка                    |Значение по умолчанию, используемая в случае оценки свойства источника до  `null` . Необязательный параметр.|
|exportMissingReferences    |Логическое                     |Только для внутреннего использования.|
|flowBehavior               |attributeFlowBehavior      |Определяет, когда этот атрибут следует экспортировать в целевой каталог. Возможные значения: `FlowWhenChanged` и `FlowAlways` . Значение по умолчанию: `FlowWhenChanged`. |
|flowType                   |attributeFlowType          |Определяет, когда этот атрибут должен быть обновлен в целевом каталоге. Возможные значения: (по умолчанию) (только при добавлении нового объекта) (только при добавлении новых значений в `Always` `ObjectAddOnly` атрибут с `MultiValueAddOnly` несколькими значениями). |
|matchingPriority           |Int32                      |Если больше 0, этот атрибут будет использоваться для выполнения начального совпадения объектов между исходными и целевыми каталогами. Сначала механизм синхронизации будет пытаться найти совпадающий объект с помощью атрибута с наименьшим значением приоритета. Если его не найти, будет использоваться атрибут со следующим приоритетом совпадения и так далее до тех пор, пока не будет найден совпадение или не останется больше совпадающих атрибутов. В качестве совпадающих атрибутов следует использовать только атрибуты, которые должны иметь уникальные значения, например электронную почту.|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | Определяет, как должно извлекать (или преобразовываться) значение из объекта-источника. |
|targetAttributeName        |Строка                     |Имя атрибута на целевом объекте. |

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
  "exportMissingReferences": "Boolean",
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


