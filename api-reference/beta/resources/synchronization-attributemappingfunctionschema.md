---
title: Тип ресурса Аттрибутемаппингфунктионсчема
description: Описывает функцию, которая может использоваться в сопоставлении атрибутов для преобразования значений во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b655d9cfac5835f6887c54c5a6bcbf79887d586
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078082"
---
# <a name="attributemappingfunctionschema-resource-type"></a>Тип ресурса Аттрибутемаппингфунктионсчема

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает функцию, которая может использоваться в [сопоставлении атрибутов](synchronization-attributemapping.md) для преобразования значений во время синхронизации.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список](../api/synchronization-synchronizationschema-functions.md) | Коллекция [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md)|Список поддерживаемых функций сопоставления атрибутов.|

## <a name="properties"></a>Свойства

| Свойство                   | Тип                      | Описание    |
|:---------------------------|:-------------------------|:---------------|
|name                        |String                    |Имя оператора. |
|parameters                  |Коллекция [аттрибутемаппингпараметерсчема](../resources/synchronization-attributemappingparameterschema.md)  |Коллекция параметров функции.|

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
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


