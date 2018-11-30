---
title: Тип ресурса attributeMappingFunctionSchema
description: Описываются функции, которая может использоваться в Отображение атрибута для преобразования значения во время синхронизации.
ms.openlocfilehash: 9760669bb29700bfa79c1cd375857b4fd673879b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078710"
---
# <a name="attributemappingfunctionschema-resource-type"></a>Тип ресурса attributeMappingFunctionSchema

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Описываются функции, который может использоваться в [сопоставление атрибутов](synchronization-attributemapping.md) для преобразования значения во время синхронизации.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[List](../api/synchronization-synchronizationschema-functions.md) | [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) коллекции|Список поддерживаемых атрибут сопоставления функций.|

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:-------------------------|:---------------|
|name                        |String                    |Имя оператора. |
|parameters                  |[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) коллекции  |Коллекция параметров функции.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->