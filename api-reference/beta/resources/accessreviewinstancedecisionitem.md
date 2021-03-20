---
title: accessReviewInstanceDecisionItem type
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e5d9b64faafb7dfe4ec4e6f3487643e62885236a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952818"
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
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Отсутствуют. | Для любого accessReviewInstanceDecisionItems, на который вызывается пользователь, на который назначен рецензент, вызывающий пользователь может записать решение, заплатив объект решения. |

## <a name="properties"></a>Свойства
| Свойство | Тип |  Описание |
| :---------------| :---- | :---------- |
| id | Строка | Идентификатор решения. |
| accessReviewId | Строка | Идентификатор родителя accessReviewInstance. |
| reviewedBy | [userIdentity](useridentity.md) | Идентификатор рецензента. |
| reviewedDateTime | DateTimeOffset | Время, затмив время проверки. |
| решение | Строка | Результат проверки. Возможные значения: `Approve` `Deny` , , или `NotReviewed` `DontKnow` . |
| обоснование | Строка | Обоснование решения по пересмотру. |
| appliedBy | [userIdentity](useridentity.md) | Идентификатор пользователя, который применил решение. |
| appliedDateTime | DateTimeOffset | Время, за которое было применено решение об утверждении. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| applyResult | Строка | Результат применения решения. Возможные значения: `NotApplied` , , , , или `Success` `Failed` `NotFound` `NotSupported` . |
| рекомендация | Строка | Сгенерированная системой рекомендация для принятия решения об утверждении. Возможные значения: `Approve` `Deny` , или `NotAvailable` .  |
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
