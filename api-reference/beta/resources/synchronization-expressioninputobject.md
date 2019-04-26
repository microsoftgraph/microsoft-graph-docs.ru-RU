---
title: Тип ресурса Експрессионинпутобжект
description: 'Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) выполняет оценку выражения.'
localization_priority: Normal
ms.openlocfilehash: 90d394639de7050eaed3b696dd8526e144cac03d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345607"
---
# <a name="expressioninputobject-resource-type"></a>Тип ресурса Експрессионинпутобжект

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|RDLC|[Обжектдефинитион](synchronization-objectdefinition.md)|Определение тестового объекта.|
|properties|Коллекция [стрингкэйобжектвалуепаир](synchronization-stringkeyobjectvaluepair.md)|Значения свойств тестового объекта.|

## <a name="json-representation"></a>Представление в формате JSON

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
