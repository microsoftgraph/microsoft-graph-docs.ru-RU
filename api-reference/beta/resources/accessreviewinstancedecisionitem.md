---
title: accessReviewInstanceDecisionItem type
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3b8e653c05e428bf0f1dc4efa8e1efb8cb4e2815
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224239"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

>[!NOTE]
>Свойство `target` будет обесценилось в v1.0 и заменено `principal` `resource` свойствами и свойствами.

Представляет решение о проверке доступа к Azure [AD](accessreviewsv2-root.md) в экземпляре проверки. Это решение является определением доступа пользователя или директора службы для данного [экземпляра обзора доступа.](accessreviewinstance.md) accessReviewInstanceDecisionItem является открытым типом и позволяет передавать другие свойства.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[List accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection | Получите список объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.|
|[Get accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для любого accessReviewInstanceDecisionItems, на который вызывается пользователь, на который назначен рецензент, вызывающий пользователь может записать решение, заплатив объект решения. |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Извлекает все [объекты accessReviewInstanceDecisionItems,](accessreviewinstancedecisionitem.md) где использование вызовов является рецензентом для данного [accessReviewInstance.](accessreviewinstance.md)|
|[List accessReviewInstanceDecisionItems pending approval (deprecated)](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Получите все accessReviewInstanceDecisionItems, назначенные вызываемой пользователю, для определенного accessReviewInstance. Этот метод отмещается и заменяется [фильтромByCurrentUser.](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md) |

## <a name="properties"></a>Свойства
| Свойство | Тип |  Описание |
| :---------------| :---- | :---------- |
|accessReviewId|Строка|Идентификатор родителя accessReviewInstance. Поддерживает `$select`. Только для чтения.|
|appliedBy|[userIdentity](../resources/useridentity.md)|Идентификатор пользователя, который применил решение. Только для чтения.|
|appliedDateTime|DateTimeOffset|Время, за которое было применено решение об утверждении. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.  Поддерживает `$select`. Только для чтения.|
|applyResult|Строка|Результат применения решения. Возможные значения: `New` `AppliedSuccessfully` , , и `AppliedWithUnknownFailure` `AppliedSuccessfullyButObjectNotFound` `ApplyNotSupported` . Поддерживает `$select` и `$orderby` `$filter` `eq` (только). Только для чтения.|
|решение|Строка|Результат проверки. Возможные значения: `Approve` `Deny` , , или `NotReviewed` `DontKnow` . Поддерживает `$select` и `$orderby` `$filter` `eq` (только). |
|id|Строка| Идентификатор решения. Наследуется от [сущности](../resources/entity.md). Поддерживает `$select`. Только для чтения.|
|обоснование|Строка|Обоснование, оставленное рецензентом при принятии решения.|
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | Цель этого конкретного решения. Целевые показатели принятия решений могут быть разных типов , каждый из которых имеет свои собственные свойства. См. [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). Только для чтения.|
|основной|[identity](../resources/identity.md)|Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. Это свойство представляет сведения о принципе. Например, если элемент решения представляет доступ пользователя "Bob" к группе "Sales", то основным элементом является "Bob", а ресурсом является "Sales". Основные принципы могут быть двух типов : userIdentity и servicePrincipalIdentity. Поддерживает `$select`. Только для чтения.|
|principalLink|Строка|Ссылка на основной объект. Пример: `https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`. Только для чтения.|
|рекомендация|Строка|Сгенерированная системой рекомендация для решения об утверждении, основанном на последнем интерактивном входе в клиент. Рекомендуется утвердить, если вход в нее находится в течение тридцати дней с начала проверки. Рекомендуется отказать, если вход превышает 30 дней с начала проверки. Рекомендация недоступна в противном случае. Возможные значения: `Approve` `Deny` , или `NoInfoAvailable` . Поддерживает `$select` и `$orderby` `$filter` `eq` (только). Только для чтения.|
|resource|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. Это свойство представляет сведения о ресурсе. Например, если элемент решения представляет доступ пользователя "Bob" к группе "Sales", то основным является Боб, а ресурсом является "Sales". Ресурсы могут быть нескольких типов. См. [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md). Только для чтения.|
|resourceLink|Строка|Ссылка на ресурс. Например, `https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8`. Поддерживает `$select`. Только для чтения.|
|reviewedBy|[userIdentity](../resources/useridentity.md)| Идентификатор рецензента. Поддерживает `$select`. Только для чтения.|
|reviewedDateTime|DateTimeOffset| Время, за которое было принято решение о проверке. Поддерживает `$select`. Только для чтения.|

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
  "principalLink": "String",
  "resource": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
  },
  "resourceLink": "String"
}
```
