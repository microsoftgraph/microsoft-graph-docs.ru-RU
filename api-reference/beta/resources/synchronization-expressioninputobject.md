---
title: Тип ресурса Експрессионинпутобжект
description: Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие Синчронизатионсчема Парсикспрессион выполняет оценку выражения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9727f50b05eb8cdb5319883dd0058a91d9383cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968361"
---
# <a name="expressioninputobject-resource-type"></a>Тип ресурса Експрессионинпутобжект

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|RDLC|[обжектдефинитион](synchronization-objectdefinition.md)|Определение тестового объекта.|
|properties|Коллекция [стрингкэйобжектвалуепаир](synchronization-stringkeyobjectvaluepair.md)|Значения свойств тестового объекта.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


