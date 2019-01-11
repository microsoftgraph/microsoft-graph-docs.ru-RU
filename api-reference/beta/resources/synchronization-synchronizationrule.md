---
title: Тип ресурса synchronizationRule
description: Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.
localization_priority: Normal
ms.openlocfilehash: a739db59a68ece026f9f13dfd22bafce8112f6b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856159"
---
# <a name="synchronizationrule-resource-type"></a>Тип ресурса synchronizationRule

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.

>**Примечание:** Правила синхронизации определение синхронизации в одном направлении - из исходного каталога в конечный каталог. Исходный и целевой каталоги определены как часть свойств правила.

Правила синхронизации обновляются в процессе [синхронизации схемы](synchronization-synchronizationschema.md).

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|изменения       |Логический    |`true`Если можно настроить правила синхронизации; `false` Если это правило доступно только для чтения и не должно изменяться.|
|id             |Строка     |Идентификатор правила синхронизации. Должен быть один из идентификаторов, распознаваемых обработчик синхронизации. Поддерживается правило, которое идентификаторы можно найти в шаблоне синхронизации, возвращаемых API.|
|метаданные       |[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) коллекции |Расширение дополнительные свойства. Если не указано явно группой поддержки, значения метаданных не должно изменяться.|
|name           |Строка     |Понятное имя правила синхронизации. Значение null не допускается.|
|objectMappings |[objectMapping](synchronization-objectmapping.md) коллекции    |Коллекция сопоставления объектов, поддерживаемых правило. Указывает обработчик синхронизации объектов, которые должны быть синхронизированы.|
|priority       |Целое число    |Приоритет относительно других правил в [synchronizationSchema](synchronization-synchronizationschema.md). Правила с наименьшим номером приоритет будут обрабатываться в первую очередь.|
|sourceDirectoryName       |Строка    |Имя исходного каталога. Должно соответствовать одному из определений каталога в [synchronizationSchema](synchronization-synchronizationschema.md).|
|targetDirectoryName       |Строка    |Имя в конечный каталог. Должно соответствовать одному из определений каталога в [synchronizationSchema](synchronization-synchronizationschema.md).|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
