---
title: accessReviewInstanceDecisionItem type
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 228fbe473fe65fe84c9dfa7c62f3689681d47e39
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443190"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет решение о проверке доступа к Azure [AD](accessreviewsv2-root.md) в экземпляре проверки. Это решение представляет определение доступа пользователя или директора службы для данного экземпляра [обзора доступа.](accessreviewinstance.md)

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[List accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection | Списки всех accessReviewInstanceDecisionItem для определенного accessReviewInstance. |
|[Список accessReviewInstanceDecisionItems до утверждения](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Получите все accessReviewInstanceDecisionItems, назначенные вызываемой пользователю, для определенного accessReviewInstance. |
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для любого accessReviewInstanceDecisionItems, на который вызывается пользователь, на который назначен рецензент, вызывающий пользователь может записать решение, заплатив объект решения. |

## <a name="properties"></a>Свойства
| Свойство | Тип |  Описание |
| :---------------| :---- | :---------- |
| id | String | Идентификатор решения. |
| accessReviewId | String | Идентификатор родителя accessReviewInstance. |
| reviewedBy | [userIdentity](useridentity.md) | Идентификатор рецензента. |
| reviewedDateTime | DateTimeOffset | DateTime при просмотре. |
| решение | String | Результат проверки. Возможные значения: `Approve` `Deny` , , или `NotReviewed` `DontKnow` . |
| обоснование | String | Обоснование решения по пересмотру. |
| appliedBy | [userIdentity](useridentity.md) | Идентификатор пользователя, который применил решение. |
| appliedDateTime | DateTimeOffset | DateTime, когда было применено решение об утверждении. |
| applyResult | String | Результат применения решения. Возможные значения: `NotApplied` , , , , или `Success` `Failed` `NotFound` `NotSupported` . |
| рекомендация | String | Сгенерированная системой рекомендация для принятия решения об утверждении. Возможные значения: `Approve` `Deny` , или `NotAvailable` .  |
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | Цель этого конкретного решения. Целевые показатели принятия решений могут быть разных типов , каждый из которых имеет свои собственные свойства. См. [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| экземпляр |[accessReviewInstance](accessreviewinstance.md) | Существует точно один accessReviewInstance, связанный с каждым решением. Экземпляр является родителем элемента решения, представляющего повторение проверки доступа, на которое принимается решение. |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "openType": true
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
 "id": "string (identifier)",
 "accessReviewId": "string",
 "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
 },
 "reviewedDateTime": "string (timestamp)",
 "decision": "string",
 "justification": "string",
 "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
 "appliedDateTime": "DateTimeOffset",
 "applyResult": "string",
 "recommendation": "string",
 "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstanceDecisionItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
