---
title: accessReviewInstanceDecisionItem type
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 968af49a9033ea749522132204d63b4f55ba25c7
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469243"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

>[!NOTE]
>Свойство `target` будет обесценилось в v1.0 и заменено `principal` свойствами и `resource` .

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
| reviewedDateTime | DateTimeOffset | Время, затмив время проверки. |
| решение | String | Результат проверки. Возможные значения: `Approve` `Deny` , , или `NotReviewed` `DontKnow` . |
| обоснование | String | Обоснование решения по пересмотру. |
| appliedBy | [userIdentity](useridentity.md) | Идентификатор пользователя, который применил решение. |
| appliedDateTime | DateTimeOffset | Время, за которое было применено решение об утверждении. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| applyResult | String | Результат применения решения. Возможные значения: `NotApplied` , , , , или `Success` `Failed` `NotFound` `NotSupported` . |
| рекомендация | String | Сгенерированная системой рекомендация для принятия решения об утверждении. Возможные значения: `Approve` `Deny` , или `NotAvailable` .  |
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | Цель этого конкретного решения. Целевые показатели принятия решений могут быть разных типов , каждый из которых имеет свои собственные свойства. См. [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). |
|основной|[identity](../resources/identity.md)|Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. Это свойство представляет сведения о принципе. Например, если элемент решения представляет доступ пользователя "Bob" к группе "Sales", то основным элементом является "Bob", а ресурсом является "Sales". Основные принципы могут быть двух типов : userIdentity и servicePrincipalIdentity.|
|resource|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. Это свойство представляет сведения о ресурсе. Например, если элемент решения представляет доступ пользователя "Bob" к группе "Sales", то основным является Боб, а ресурсом является "Sales". Ресурсы могут быть нескольких типов. См. [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|

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
  "id": "String (identifier)",
  "accessReviewId": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "reviewedDateTime": "String (timestamp)",
  "decision": "String",
  "justification": "String",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "String (timestamp)",
  "applyResult": "String",
  "recommendation": "String",
  "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  },
  "principal": {
    "@odata.type": "microsoft.graph.identity"
  },
  "resource": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
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
