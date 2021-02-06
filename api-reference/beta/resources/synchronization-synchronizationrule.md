---
title: Тип ресурса synchronizationRule
description: Определяет, как должна выполняться синхронизация для обдвижки синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 94697fede9ab9055b1a477cfd94edea88f207331
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135999"
---
# <a name="synchronizationrule-resource-type"></a>Тип ресурса synchronizationRule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как должна выполняться синхронизация для обдвижка синхронизации, включая объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходных каталогов должны быть соединяются с объектами в целевом каталоге и как атрибуты должны преобразовываться при их синхронизации из источника в целевой каталог.

>**Примечание.** Правила синхронизации определяют синхронизацию в одном направлении — от каталога источника к целевому. Исходный и целевой каталоги определяются как часть свойств правила.

Правила синхронизации обновляются в рамках [схемы синхронизации.](synchronization-synchronizationschema.md)

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|редактируемый       |Boolean    |`true` если правило синхронизации можно настроить; `false` если это правило является только для чтения и не должно быть изменено.|
|id             |Строка     |Идентификатор правила синхронизации. Должен быть одним из идентификаторов, распознается механизмом синхронизации. Поддерживаемые идентификаторы правил можно найти в шаблоне синхронизации, возвращаемом API.|
|метаданные       |[Коллекция stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) |Дополнительные свойства расширения. Если группа поддержки явно не проинструктировали ее, значения метаданных не следует менять.|
|name           |String     |Понятное для человека имя правила синхронизации. Значение null не допускается.|
|objectMappings |[Коллекция objectMapping](synchronization-objectmapping.md)    |Коллекция сопоставлений объектов, поддерживаемых правилом. Сообщает механизму синхронизации, какие объекты следует синхронизировать.|
|priority       |Целое число    |Приоритет относительно других правил в [synchronizationSchema.](synchronization-synchronizationschema.md) Правила с наименьшим номером приоритета будут обрабатываться в первую очередь.|
|sourceDirectoryName       |Строка    |Имя каталога источника. Должно соответствовать одному из определений каталогов в [synchronizationSchema.](synchronization-synchronizationschema.md)|
|targetDirectoryName       |Строка    |Имя целевого каталога. Должно соответствовать одному из определений каталогов в [synchronizationSchema.](synchronization-synchronizationschema.md)|

## <a name="json-representation"></a>Представление в формате JSON

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
  "suppressions": []
}
-->


