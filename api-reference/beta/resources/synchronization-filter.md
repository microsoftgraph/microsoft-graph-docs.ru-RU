---
title: Тип ресурса Filter
description: Определяет, какие объекты должны быть подготовлены для приложения. Например, вам может потребоваться предоставить только пользователей, которые находятся в США. При наличии фильтра областей объекты, которые не соответствуют фильтру, будут пропущены во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582124"
---
# <a name="filter-resource-type"></a>Тип ресурса Filter

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, какие объекты должны быть подготовлены для приложения. Например, вам может потребоваться предоставить только пользователей, которые находятся в США. При наличии фильтра областей объекты, которые не соответствуют фильтру, будут пропущены во время синхронизации.

Фильтр является частью [сопоставления объектов](synchronization-objectmapping.md). Он состоит из нескольких наборов групп фильтров, а каждая группа фильтра содержит одно или несколько предложений. Объект рассматривается в области для группы (Группа оценивается как `true`) только в `true`том случае, если все предложения группы оцениваются.

Объект рассматривается в области для набора групп (набор групп оценивается как `true`), если для `true`каждой из групп в наборе вычислена значение.

Дополнительные сведения см в разделе [Подготовка приложений на основе атрибутов с помощью фильтров областей](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Категорифилтерграупс|Коллекция [филтерграуп](synchronization-filtergroup.md)|`*Experimental*`Набор групп фильтров, используемый, чтобы определить, принадлежит ли данный объект и должен ли он обрабатываться как часть этого сопоставления объектов. Объект считается в области действия, *Если любая из групп в коллекции оценивается как `true` *.|
|groups|Коллекция [филтерграуп](synchronization-filtergroup.md)|Набор групп фильтров, используемый для определения того, находится ли заданный объект в области для подготовки. **Это фильтр, который следует использовать в большинстве случаев**. Если объект, используемый для выполнения этого фильтра, в данный момент, а затем объект или фильтр изменились так, что фильтр не удовлетворен более длинным, такой объект * будет передано. Объект считается в области действия, *Если любая из групп в коллекции оценивается как `true` *.|
|Инпутфилтерграупс|Коллекция [филтерграуп](synchronization-filtergroup.md)|`*Experimental*`Набор групп фильтров, используемый для фильтрации объектов на раннем этапе чтения их из каталога. Если объект не соответствует этому фильтру, он не будет обрабатываться далее. Важно понимать, что если объект, используемый для выполнения этого фильтра, в данный момент, а затем объект или фильтр изменился, так как фильтр больше не удовлетворен, такой объект *не*передается. Объект считается в области действия, *Если любая из групп в коллекции оценивается как `true` *. |

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
