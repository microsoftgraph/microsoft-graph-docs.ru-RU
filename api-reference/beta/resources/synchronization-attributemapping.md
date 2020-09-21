---
title: Тип ресурса Аттрибутемаппинг
description: Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7573773737f4ff4380a446cf62107e8ac26642ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078099"
---
# <a name="attributemapping-resource-type"></a>Тип ресурса Аттрибутемаппинг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.

## <a name="properties"></a>Свойства

| Свойство                  | Тип                      | Описание    |
|:--------------------------|:--------------------------|:---------------|
|Значение               | String                    |Значение по умолчанию, используемое в случае, если свойство **Source** было оценено `null` . Необязательное свойство.|
|експортмиссингреференцес    |String                     |Только для внутреннего использования.|
|фловбехавиор               |аттрибутефловбехавиор      |Определяет, когда этот атрибут должен быть экспортирован в целевой каталог. Возможные значения: `FlowWhenChanged` и `FlowAlways` . Значение по умолчанию: `FlowWhenChanged`. |
|фловтипе                   |аттрибутефловтипе          |Определяет, когда этот атрибут должен быть обновлен в целевом каталоге. Возможные значения: `Always` (по умолчанию) ( `ObjectAddOnly` только при создании нового объекта) `MultiValueAddOnly` (только когда изменение добавляет новые значения в атрибут с несколькими значениями). |
|матчингприорити           |Int32                      |Если значение больше 0, этот атрибут будет использоваться для выполнения начального сопоставления объектов между исходным и целевым каталогами. Обработчик синхронизации попытается найти совпадающий объект с использованием атрибута с наименьшим значением приоритета совпадения первыми. Если этот параметр не найден, будет использоваться атрибут с соответствующим приоритетом, и поэтому при обнаружении совпадения и других атрибутах совпадения не осталось. В качестве искомых атрибутов следует использовать только те атрибуты, которые должны иметь уникальные значения (например, электронная почта).|
|source                     |[аттрибутемаппингсаурце](synchronization-attributemappingsource.md)     | Определяет способ извлечения (или преобразования) значения из исходного объекта. |
|таржетаттрибутенаме        |String                     |Имя атрибута в целевом объекте. |

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
  "suppressions": []
}
-->


