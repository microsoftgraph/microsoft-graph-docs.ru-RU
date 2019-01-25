---
title: Тип ресурса synchronizationRule
description: Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517927"
---
# <a name="synchronizationrule-resource-type"></a>Тип ресурса synchronizationRule

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.

>**Примечание:** Правила синхронизации определение синхронизации в одном направлении - из исходного каталога в конечный каталог. Исходный и целевой каталоги определены как часть свойств правила.

Правила синхронизации обновляются в процессе [синхронизации схемы](synchronization-synchronizationschema.md).

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|изменения       |Логическое    |`true`Если можно настроить правила синхронизации; `false` Если это правило доступно только для чтения и не должно изменяться.|
|id             |String     |Идентификатор правила синхронизации. Должен быть один из идентификаторов, распознаваемых обработчик синхронизации. Поддерживается правило, которое идентификаторы можно найти в шаблоне синхронизации, возвращаемых API.|
|Метаданные       |[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) коллекции |Расширение дополнительные свойства. Если не указано явно группой поддержки, значения метаданных не должно изменяться.|
|name           |String     |Понятное имя правила синхронизации. Значение null не допускается.|
|objectMappings |[objectMapping](synchronization-objectmapping.md) коллекции    |Коллекция сопоставления объектов, поддерживаемых правило. Указывает обработчик синхронизации объектов, которые должны быть синхронизированы.|
|priority       |Целое число    |Приоритет относительно других правил в [synchronizationSchema](synchronization-synchronizationschema.md). Правила с наименьшим номером приоритет будут обрабатываться в первую очередь.|
|sourceDirectoryName       |String    |Имя исходного каталога. Должно соответствовать одному из определений каталога в [synchronizationSchema](synchronization-synchronizationschema.md).|
|targetDirectoryName       |String    |Имя в конечный каталог. Должно соответствовать одному из определений каталога в [synchronizationSchema](synchronization-synchronizationschema.md).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationrule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
