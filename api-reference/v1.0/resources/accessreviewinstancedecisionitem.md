---
title: accessReviewInstanceDecisionItem type
description: Представляет решение о accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4b29eb37f7088185f64b790a15458fa7b30dd7db185bf04903fabaf8d78d124f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163917"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem type

Пространство имен: microsoft.graph

Представляет решение о проверке доступа к Azure [AD](accessreviewsv2-root.md) в экземпляре проверки. Это решение представляет определение доступа удостоверения к ресурсу для данного [accessReviewInstance](accessreviewinstance.md).

Каждый элемент решения является системным на основе родительского [accessReviewInstance.](accessreviewinstance.md)

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[List accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Получите список объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.|
|[Get accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[Обновление accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Обновление свойств объекта [accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection|Возвращает элементы решения, для которых вызываемая пользователь является рецензентом.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessReviewId|String|Идентификатор родителя accessReviewInstance. Поддерживает `$select`. Только для чтения.|
|appliedBy|[userIdentity](../resources/useridentity.md)|Идентификатор пользователя, который применил решение. Только для чтения.|
|appliedDateTime|DateTimeOffset|Время, за которое было применено решение об утверждении. Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.  Поддерживает `$select`. Только для чтения.|
|applyResult|String|Результат применения решения. Возможные значения: `New` `AppliedSuccessfully` , , и `AppliedWithUnknownFailure` `AppliedSuccessfullyButObjectNotFound` `ApplyNotSupported` . Поддерживает `$select` и `$orderby` `$filter` `eq` (только). Только для чтения.|
|решение|String|Результат проверки. Возможные значения: `Approve` `Deny` , , или `NotReviewed` `DontKnow` . Поддерживает `$select` и `$orderby` `$filter` `eq` (только). |
|id|String| Идентификатор решения. Наследуется от [сущности](../resources/entity.md). Поддерживает `$select`. Только для чтения.|
|обоснование|String|Обоснование, оставленное рецензентом при принятии решения.|
|основной|[identity](../resources/identity.md)|Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. Это свойство представляет сведения о принципе. Например, если элемент решения представляет доступ пользователя "Bob" к группе "Sales", то основным элементом является "Bob", а ресурсом является "Sales". Основные принципы могут быть двух типов : userIdentity и servicePrincipalIdentity. Поддерживает `$select`. Только для чтения.|
|principalLink|String|Ссылка на основной объект. Например, `https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`. Только для чтения.|
|рекомендация|String|Сгенерированная системой рекомендация для решения об утверждении, основанном на последнем интерактивном входе в клиент. Рекомендуется утвердить, если вход в нее находится в течение тридцати дней с начала проверки. Рекомендуется отказать, если вход превышает 30 дней с начала проверки. Рекомендация недоступна в противном случае. Возможные значения: `Approve` `Deny` , или `NoInfoAvailable` . Поддерживает `$select` и `$orderby` `$filter` `eq` (только). Только для чтения.|
|resource|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. Это свойство представляет сведения о ресурсе. Например, если элемент решения представляет доступ пользователя "Bob" к группе "Sales", то основным является Боб, а ресурсом является "Sales". Ресурсы могут быть нескольких типов. См. [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md). Только для чтения.|
|resourceLink|String|Ссылка на ресурс. Например, https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8 ". Поддерживает `$select`. Только для чтения.|
|reviewedBy|[userIdentity](../resources/useridentity.md)| Идентификатор рецензента. Поддерживает `$select`. Только для чтения.|
|reviewedDateTime|DateTimeOffset| Время, за которое было принято решение о проверке. Поддерживает `$select`. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
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
