---
title: Тип ресурса Синчронизатионруле
description: Определяет способ выполнения синхронизации для обработчика синхронизации, в том числе объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге и как атрибуты должно быть преобразовано при синхронизации из источника с целевым каталогом.
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453646"
---
# <a name="synchronizationrule-resource-type"></a>Тип ресурса Синчронизатионруле

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет способ выполнения синхронизации для обработчика синхронизации, в том числе объекты, которые необходимо синхронизировать и в каком направлении, как объекты из исходного каталога должны сопоставляться с объектами в целевом каталоге и как атрибуты должно быть преобразовано при синхронизации из источника с целевым каталогом.

>**Примечание:** Правила синхронизации определяют синхронизацию в одном направлении — из исходного каталога в конечный каталог. Исходные и целевые каталоги определяются как часть свойств правила.

Правила синхронизации обновляются в рамках [схемы синхронизации](synchronization-synchronizationschema.md).

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание    |
|:--------------|:----------|:---------------|
|редактируем       |Boolean    |`true`значение, если правило синхронизации может быть изменено; `false` если это правило доступно только для чтения и не должно изменяться.|
|id             |Строка     |Идентификатор правила синхронизации. Допустимые значения: один из идентификаторов, распознаваемый обработчиком синхронизации. Поддерживаемые идентификаторы правил можно найти в шаблоне синхронизации, возвращенном API.|
|метаданных       |Коллекция [стрингкэйстрингвалуепаир](synchronization-stringkeystringvaluepair.md) |Дополнительные свойства расширения. Если вы не укажете в явной форме команду поддержки, значения метаданных не должны изменяться.|
|name           |String     |Понятное имя правила синхронизации. Значение null не допускается.|
|Обжектмаппингс |Коллекция [обжектмаппинг](synchronization-objectmapping.md)    |Коллекция сопоставлений объектов, поддерживаемых правилом. Сообщает обработчику синхронизации, какие объекты должны синхронизироваться.|
|priority       |Целое число    |Приоритет относительно других правил в [синчронизатионсчема](synchronization-synchronizationschema.md). Правила с наименьшим номером приоритета будут обработаны первыми.|
|Саурцедиректоринаме       |Строка    |Имя исходного каталога. Должно сопоставляться с одним из определений каталога в [синчронизатионсчема](synchronization-synchronizationschema.md).|
|Таржетдиректоринаме       |Строка    |Имя целевого каталога. Должно сопоставляться с одним из определений каталога в [синчронизатионсчема](synchronization-synchronizationschema.md).|

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
