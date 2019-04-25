---
title: Тип ресурса Аттрибутемаппинг
description: Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582118"
---
# <a name="attributemapping-resource-type"></a>Тип ресурса Аттрибутемаппинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.

## <a name="properties"></a>Свойства

| Свойство                  | Тип                      | Описание    |
|:--------------------------|:--------------------------|:---------------|
|Значение               | String                    |Значение по умолчанию, используемое в **** случае, если свойство Source `null`было оценено. Необязательный параметр.|
|Експортмиссингреференцес    |String                     |Только для внутреннего использования.|
|Фловбехавиор               |Аттрибутефловбехавиор      |Определяет, когда этот атрибут должен быть экспортирован в целевой каталог. Возможные значения: `FlowWhenChanged` и `FlowAlways`. Значение по умолчанию: `FlowWhenChanged`. |
|Фловтипе                   |Аттрибутефловтипе          |Определяет, когда этот атрибут должен быть обновлен в целевом каталоге. Возможные значения: `Always` (по умолчанию) `ObjectAddOnly` (только при создании нового объекта) `MultiValueAddOnly` (только когда изменение добавляет новые значения в атрибут с несколькими значениями). |
|Матчингприорити           |Int32                      |Если значение больше 0, этот атрибут будет использоваться для выполнения начального сопоставления объектов между исходным и целевым каталогами. Обработчик синхронизации попытается найти совпадающий объект с использованием атрибута с наименьшим значением приоритета совпадения первыми. Если этот параметр не найден, будет использоваться атрибут с соответствующим приоритетом, и поэтому при обнаружении совпадения и других атрибутах совпадения не осталось. В качестве искомых атрибутов следует использовать только те атрибуты, которые должны иметь уникальные значения (например, электронная почта).|
|source                     |[Аттрибутемаппингсаурце](synchronization-attributemappingsource.md)     | Определяет способ извлечения (или преобразования) значения из исходного объекта. |
|Таржетаттрибутенаме        |String                     |Имя атрибута в целевом объекте. |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
