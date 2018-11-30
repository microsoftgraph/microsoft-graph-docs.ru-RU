---
title: Тип ресурса attributeMapping
description: Определяет, как значения для атрибута заданный целевой поток во время синхронизации.
ms.openlocfilehash: e4fd8ba0aece448f358d51373dfca0157759a23e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078180"
---
# <a name="attributemapping-resource-type"></a>Тип ресурса attributeMapping

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Определяет, как значения для атрибута заданный целевой поток во время синхронизации.

## <a name="properties"></a>Свойства

| Свойство                  | Тип                      | Описание    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | String                    |По умолчанию значение для использования в случае, если свойство **source** проверялись `null`. Необязательный атрибут.|
|exportMissingReferences    |String                     |Только для внутреннего использования.|
|flowBehavior               |attributeFlowBehavior      |Определяет, когда этот атрибут, должны быть экспортированы в конечный каталог. Возможные значения: `FlowWhenChanged` и `FlowAlways`. Значение по умолчанию: `FlowWhenChanged`. |
|flowType                   |attributeFlowType          |Определяет, когда этот атрибут следует обновить в целевой каталог. Возможные значения: `Always` (по умолчанию), `ObjectAddOnly` (только если создается новый объект), `MultiValueAddOnly` (только при изменении добавляет новые значения это многозначный атрибут). |
|matchingPriority           |Int32                      |Если больше 0, этот атрибут будет использоваться для выполнения первоначальной совпадение объектов между исходный и конечный каталоги. Обработчик синхронизации попытается найти соответствующий объект, с помощью атрибута с наименьшее значение сначала совпадающих приоритет. Если не найден, атрибута с помощью следующего соответствия приоритет будет использоваться и так далее до совпадения или исключаются соответствующие атрибуты. Только атрибуты, которые должны иметь уникальные значения, такие как электронной почтой, следует использовать в качестве соответствующие атрибуты.|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта. |
|targetAttributeName        |String                     |Имя атрибута для конечного объекта. |

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->