---
title: Тип ресурса accessReviewInstanceDecisionItemAzureRoleResource
description: Представляет роли ресурсов Azure, для которых доступ представлен через объект accessReviewInstanceDecisionItem.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d607463664ee5c106e373a7bb568bfd32cd3c0a0
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697885"
---
# <a name="accessreviewinstancedecisionitemazureroleresource-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItemAzureRoleResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет роли ресурсов Azure, для которых доступ представлен через [объект accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . **accessReviewInstanceDecisionItemAzureRoleResource** — это открытый тип, который позволяет передавать другие свойства.

Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| displayName | Строка | Отображаемое имя роли Azure. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | String | Идентификатор ресурса элемента принятия решения. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Строка | Тип ресурса. Тип всегда будет иметь значение `AzureRole`.  Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| область | [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md) | Сведения об области, с помощью которая связана эта роль. |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
  }
}
```
