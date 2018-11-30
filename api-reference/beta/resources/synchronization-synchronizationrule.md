---
title: Тип ресурса synchronizationRule
description: Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.
ms.openlocfilehash: c860228637a6cc3ad9137851408379bd7f779c75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076746"
---
# <a name="synchronizationrule-resource-type"></a>Тип ресурса synchronizationRule

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Определяет, как следует выполнять синхронизацию для обработчика синхронизации, включая объектов для синхронизации и направление, как объекты из исходного каталога должны совпадать с объектами в целевом каталоге и как атрибуты должен быть преобразован при их в случае синхронизации из источника в конечный каталог.

>**Примечание:** Правила синхронизации определение синхронизации в одном направлении - из исходного каталога в конечный каталог. Исходный и целевой каталоги определены как часть свойств правила.

Правила синхронизации обновляются в процессе [синхронизации схемы](synchronization-synchronizationschema.md).

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Description    |
|:--------------|:----------|:---------------|
|изменения       |Логический    |`true`Если можно настроить правила синхронизации; `false` Если это правило доступно только для чтения и не должно изменяться.|
|id             |String     |Идентификатор правила синхронизации. Должен быть один из идентификаторов, распознаваемых обработчик синхронизации. Поддерживается правило, которое идентификаторы можно найти в шаблоне синхронизации, возвращаемых API.|
|метаданные       |[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) коллекции |Расширение дополнительные свойства. Если не указано явно группой поддержки, значения метаданных не должно изменяться.|
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->