---
title: Тип ресурса accessReviewInstanceDecisionItem
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 633e095d0fbb2843c888e52f1d71bb0eda1c4644
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697894"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет Azure AD [проверки доступа](accessreviewsv2-overview.md) для экземпляра проверки. Это решение представляет собой определение доступа пользователя или субъекта-службы для данного экземпляра [проверки доступа](accessreviewinstance.md).  Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление объектов accessReviewInstanceDecisionItems](../api/accessreviewinstance-list-decisions.md) | [Коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Получение списка объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.|
|[Получение объекта accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Чтение свойств и связей объекта [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Нет. | Для любых объектов accessReviewInstanceDecisionItems, для которых вызывающему пользователю назначен рецензент, вызывающий пользователь может записать решение, исправив объект принятия решения. |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Извлекает все [объекты accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) , где вызывающее использование является рецензентом для данного [объекта accessReviewInstance](accessreviewinstance.md).|
|[Вывод списка объектов accessReviewInstanceDecisionItems, ожидающих утверждения (не рекомендуется)](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . | Получение всех объектов accessReviewInstanceDecisionItems, назначенных вызывающему пользователю, для определенного объекта accessReviewInstance. Этот метод является устаревшим и заменяется [filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md). |

## <a name="properties"></a>Свойства
| Свойство | Тип |  Описание |
| :---------------| :---- | :---------- |
|accessReviewId|String|Идентификатор родительского объекта accessReviewInstance. Поддерживает `$select`. Только для чтения.|
|appliedBy|[userIdentity](../resources/useridentity.md)|Идентификатор пользователя, который применил решение. Только для чтения.|
|appliedDateTime|DateTimeOffset|Метка времени, когда было применено решение об утверждении. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда используется во время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.  Поддерживает `$select`. Только для чтения.|
|applyResult|Строка|Результат применения решения. Возможные значения: `New`, `AppliedSuccessfully`, и `AppliedSuccessfullyButObjectNotFound` `AppliedWithUnknownFailure``ApplyNotSupported`. Поддерживает , `$select``$orderby`и `$filter` (`eq`только). Только для чтения.|
|Решение|Строка|Результат проверки. Возможные значения: `Approve`, `Deny`, или `NotReviewed``DontKnow`. Поддерживает , `$select``$orderby`и `$filter` (`eq`только). |
|id|String| Идентификатор решения. Наследуется от [сущности](../resources/entity.md). Поддерживает `$select`. Только для чтения.|
|Обоснование|Строка|Обоснование, оставленные рецензентом при принятии решения.|
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | Целевой объект этого конкретного решения. Целевые объекты принятия решений могут иметь разные типы — каждый со своими собственными свойствами. См [. accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). Только для чтения. <br/> Это свойство было заменено свойствами `principal` и свойствами `resource` в версии 1.0.|
|Основной|[identity](../resources/identity.md)|Каждый элемент принятия решений в проверке доступа представляет доступ субъекта к ресурсу. Это свойство представляет сведения о субъекте. Например, если элемент принятия решений представляет доступ пользователя Bob к группе "Продажи", то субъект — "Боб", а ресурс — "Sales". Субъекты могут иметь два типа: userIdentity и servicePrincipalIdentity. Поддерживает `$select`. Только для чтения.|
|principalLink|Строка|Ссылка на основной объект. Пример: `https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`. Только для чтения.|
|Рекомендации|String|Созданная системой рекомендация для принятия решения об утверждении на основе последнего интерактивного входа в клиент. Рекомендуем утвердить, если вход выполняется в течение 30 дней с начала проверки. Рекомендуется запретить вход, если срок действия входа превышает 30 дней с начала проверки. В противном случае рекомендация недоступна. Возможные значения: `Approve`, или `Deny``NoInfoAvailable`. Поддерживает , `$select``$orderby`и `$filter` (`eq`только). Только для чтения.|
|resource|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|Каждый элемент принятия решений в проверке доступа представляет доступ субъекта к ресурсу. Это свойство представляет сведения о ресурсе. Например, если элемент принятия решения представляет доступ пользователя "Bob" к группе "Продажи", то субъектом является Боб, а ресурс — "Sales". Ресурсы могут иметь несколько типов. См [. accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md). Только для чтения.|
|resourceLink|String|Ссылка на ресурс. Например, `https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8`. Поддерживает `$select`. Только для чтения.|
|reviewedBy|[userIdentity](../resources/useridentity.md)| Идентификатор рецензента. Поддерживает `$select`. Только для чтения.|
|reviewedDateTime|DateTimeOffset| Метка времени, когда было принято решение о проверке. Поддерживает `$select`. Только для чтения.|
|principalResourceMembership|[decisionItemPrincipalResourceMembership](../resources/decisionItemPrincipalResourceMembership.md)| Каждый элемент решения в проверке доступа представляет членство участника в ресурсе. Это свойство предоставляет сведения о членстве. Например, имеет ли субъект прямой или косвенный доступ к ресурсу. Поддерживает `$select`. Только для чтения.|


## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
| экземпляр |[accessReviewInstance](accessreviewinstance.md) | С каждым решением связан ровно один объект accessReviewInstance. Экземпляр является родительским элементом элемента принятия решения, представляющим периодичность проверки доступа, в которых принимается решение. |
| insights |[Коллекция governanceInsight](governanceinsight.md) | Аналитические сведения — это рекомендации рецензентам по утверждению или отклонению решения. С **accessReviewInstanceDecisionItem может быть связано несколько аналитических сведений**. |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
  "principalResourceMembership": {
    "@odata.type": "microsoft.graph.decisionItemPrincipalResourceMembership"
  },
  "resourceLink": "String"
}
```
