---
title: accessReviewInstanceDecisionItemAzureRoleResource type
description: Представляет роли ресурсов Azure, для которых доступ представлен через объект accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c8975a623deb763f5a83a22ff49bf28b122325a7
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162316"
---
# <a name="accessreviewinstancedecisionitemazureroleresource-resource-type"></a>accessReviewInstanceDecisionItemAzureRoleResource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет роли ресурсов Azure, для которых доступ представлен через [объект accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) **accessReviewInstanceDecisionItemAzureRoleResource** — это открытый тип, который позволяет передавать другие свойства.

Наследует [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| displayName | Строка | Отображение имени роли Azure. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | Строка | Идентификатор ресурса элемента решения. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Строка | Тип ресурса. Тип всегда будет `AzureRole` .  Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| область | [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md) | Сведения о области, с которую связана эта роль. |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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
