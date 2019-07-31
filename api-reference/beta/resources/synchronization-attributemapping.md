---
title: Тип ресурса Аттрибутемаппинг
description: Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 09ed298022e687354f7fa9905ee25f5c38f2fdfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964840"
---
# <a name="attributemapping-resource-type"></a>Тип ресурса Аттрибутемаппинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.

## <a name="properties"></a>Свойства

| Свойство                  | Тип                      | Описание    |
|:--------------------------|:--------------------------|:---------------|
|Значение               | String                    |Значение по умолчанию, используемое в **** случае, если свойство Source `null`было оценено. Необязательно.|
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
  "suppressions": []
}
-->
