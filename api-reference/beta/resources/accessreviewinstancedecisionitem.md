---
title: Тип ресурса accessReviewInstanceDecisionItem
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10166dc9da512bf74a0b4e5ad97f4797cdf6c317
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159201"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет решение о проверке [доступа](accessreviewsv2-root.md) Azure AD для экземпляра проверки. Это решение представляет определение доступа пользователя или директора-службы для данного экземпляра [проверки доступа.](accessreviewinstance.md)

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Список accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [Коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Перечисляет все accessReviewInstanceDecisionItem для определенного accessReviewInstance. |
|[Список accessReviewInstanceDecisionItems, ожидающих утверждения](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [коллекция accessReviewInstanceDecisionItem;](accessreviewinstancedecisionitem.md) | Получите все accessReviewInstanceDecisionItems, присвоенные вызыванию пользователю, для определенного accessReviewInstance. |
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для любых объектов accessReviewInstanceDecisionItems, в которые назначен вызывающий пользователь, вызывающий пользователь может записать решение, обновив объект решения. |

## <a name="properties"></a>Свойства
| Свойство | Тип |  Описание |
| :---------------| :---- | :---------- |
| id | String | Идентификатор решения. |
| accessReviewId | String | Идентификатор родительского accessReviewInstance. |
| reviewedBy | [userIdentity](useridentity.md) | Идентификатор проверяемого. |
| reviewedDateTime | DateTimeOffset | Дата и время проверки. |
| decision | String | Результат проверки. Возможные значения: `Approve` , , , или `Deny` `NotReviewed` `DontKnow` . |
| обоснование | String | Обоснование принятия решения о проверке. |
| appliedBy | [userIdentity](useridentity.md) | Идентификатор пользователя, который применил решение. |
| appliedDateTime | DateTimeOffset | Дата и время, когда было применено решение об утверждении. |
| applyResult | String | Результат применения решения. Возможные значения: `NotApplied` , , , , или `Success` `Failed` `NotFound` `NotSupported` . |
| recommendation | String | Системная рекомендация для решения об утверждении. Возможные значения: `Approve` , `Deny` , или `NotAvailable` .  |
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | Цель конкретного решения. Целевые объекты принятия решений могут быть разных типов , каждый из которых имеет собственные свойства. См. [accessReviewInstanceDecisionItemTarget.](accessreviewinstancedecisionitemtarget.md) |

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| экземпляр |[accessReviewInstance](accessreviewinstance.md) | С каждым решением связан только один accessReviewInstance. Экземпляр является родительским элементом элемента решения, представляющим повторение проверки доступа, на которое было принято решение. |


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
