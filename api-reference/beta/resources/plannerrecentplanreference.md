---
title: тип ресурса plannerRecentPlanReference
description: 'Тип **ресурса plannerRecentPlanReference** покаяется ссылкой на планировщикПлан, который недавно был просмотрен пользователем. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8a8fbf3ce9f39c49dde4bbeee96a3aab15a00077
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720979"
---
# <a name="plannerrecentplanreference-resource-type"></a>тип ресурса plannerRecentPlanReference

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип **ресурса plannerRecentPlanReference** покаяется ссылкой на [планировщикПлан,](plannerplan.md) который недавно был просмотрен пользователем. **ПланировщикRecentPlanReferences** для пользователя явно поддерживается приложениями. Любое приложение, которое реализует функцию последних планов, должно записывать, когда пользователь последний раз просматривал план, и обновлять записи **plannerRecentPlanReference** соответственно.
Приложения должны отметить, что записи **plannerRecentPlanReference** могут ссылаться на планировщикПланы, которые удаляются, что пользователь больше не может получить доступ или которые были обновлены с другим названием. 
Мы рекомендуем приложениям уведомлять пользователей о несоответствиях и поддерживать записи в курсе.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|Дата и время последнего просмотра плана пользователем. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|planTitle|String|Название плана во время просмотра пользователем.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


