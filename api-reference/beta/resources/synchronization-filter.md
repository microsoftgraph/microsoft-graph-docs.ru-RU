---
title: Тип ресурса Filter
description: Определяет, какие объекты, следует подготовить к приложению. Например может потребоваться только подготовки пользователей, которые расположены в США. Если фильтр области видимости, объекты, которые не удовлетворяют фильтра будет пропущено во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516681"
---
# <a name="filter-resource-type"></a>Тип ресурса Filter

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, какие объекты, следует подготовить к приложению. Например может потребоваться только подготовки пользователей, которые расположены в США. Если фильтр области видимости, объекты, которые не удовлетворяют фильтра будет пропущено во время синхронизации.

Фильтр является частью [сопоставление объектов](synchronization-objectmapping.md). Состоит из нескольких наборов групп фильтра, и каждой группе фильтра содержит одно или несколько предложений. Объект считается в области действия группы (рассчитано группы для `true`) только в том случае, если все предложения группе вычисляются для `true`.

Объект считается в области действия для набора группы (набор групп вычисляется для `true`) Если какие-либо группы в наборе оценивается `true`.

Для получения дополнительных сведений см. [Подготовка с помощью области видимости фильтры приложения на основе атрибутов](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|categoryFilterGroups|[filterGroup](synchronization-filtergroup.md) коллекции|`*Experimental*`Используются для определения, является ли указанный объект принадлежит группе установлен фильтр и будут обрабатываться как часть этого сопоставления объектов. Объект считается в области *Если какие-либо группы в коллекции оценивается `true` *.|
|группы|[filterGroup](synchronization-filtergroup.md) коллекции|Фильтровать набор группы, используемый в том, является ли указанный объект в области действия для подготовки. **Это фильтр, который должен использоваться в большинстве случаев**. Объект, используемый для удовлетворения этот фильтр в данный момент и затем объект или фильтр был изменен, поэтому этот фильтр не больше, удовлетворены такого объекта * будет получить отзыва подготовить к работе». Объект считается в области *Если какие-либо группы в коллекции оценивается `true` *.|
|inputFilterGroups|[filterGroup](synchronization-filtergroup.md) коллекции|`*Experimental*`Фильтровать набор группы, используемый для фильтрации объектов на ранней стадии чтения их из каталога. Если объект не удовлетворяют этот фильтр, которые не будут обрабатываться Дополнительно. Важно понимать, что если объект используются для удовлетворения этот фильтр в данный момент, а затем объект или фильтр изменен, этот фильтр больше не выполняется, например объекта *будет не получите отзыва подготовить к работе*. Объект считается в области *Если какие-либо группы в коллекции оценивается `true` *. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
