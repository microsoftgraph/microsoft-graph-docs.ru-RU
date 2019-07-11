---
title: Тип ресурса Експрессионинпутобжект
description: 'Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [синчронизатионсчема: парсикспрессион](../api/synchronization_synchronizationschema_parseexpression.md) выполняет оценку выражения.'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b5fb11471757328bf0b84ae5ea0977d43587d7e4
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621384"
---
# <a name="expressioninputobject-resource-type"></a>Тип ресурса Експрессионинпутобжект

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект, который будет использоваться в качестве входных тестовых данных, когда действие [парсикспрессион](../api/synchronization-synchronizationschema-parseexpression.md) выполняет оценку выражения.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|RDLC|[Обжектдефинитион](synchronization-objectdefinition.md)|Определение тестового объекта.|
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
