---
title: Тип ресурса accessReviewDecision (не рекомендуется)
description: AccessReviewDecision представляет Azure AD проверки доступа для доступа определенной сущности.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb85de238c852d1e4e397cd142e7bb4863e3f2a1
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820800"
---
# <a name="accessreviewdecision-resource-type-deprecated"></a>Тип ресурса accessReviewDecision (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

В Azure AD [проверки](accessreviews-root.md) `accessReviewDecision` доступа объект представляет Azure AD проверки доступа определенной сущности.  В рамках проверки доступа или экземпляра повторяющейся проверки доступа имеется по `accessReviewDecision` одному для каждого проверяемого пользователя.  Например, если в группе есть два гостя и один не гостевой в качестве участников, а для этой группы выполняется проверка доступа гостей, то будут два объекта принятия решений для проверки доступа.  Если рецензент изменяет свое решение или другой рецензент переопределяет его, `accessReviewDecision` то он обновляется.


## <a name="methods"></a>Методы

Нет.  Объекты этого типа автоматически создаются компонентом при инициализации проверки доступа и не могут быть удалены.  Их можно получить из проверки доступа с [помощью решений](../api/accessreview-listdecisions.md) и [связей mydecisions](../api/accessreview-listmydecisions.md) .

## <a name="properties"></a>Свойства

В этой таблице показаны базовые свойства объектов этого типа. 

| Свойство                        | Тип                         | Описание                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | Идентификатор решения в рамках проверки доступа.                                                                                     |
| `accessReviewId`                |`String`                      | Созданный компонентом идентификатор проверки доступа.                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| Удостоверение рецензента. Если рекомендация использовалась в качестве проверки, userPrincipalName пуст.                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | Дата и время последней проверки этого права доступа.                                                                         |
| `reviewResult`                  |`String`                      | Результат проверки, один из `NotReviewed`, `Deny`или `DontKnow` `Approve`.                                                                                    |
| `justification`                 |`String`                      | Бизнес-обоснование рецензента, если оно предоставлено.                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| По завершении проверки, если результаты были применены вручную, удостоверение пользователя, который применил решение. Если проверка была применена автоматически, userPrincipalName пуст.                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | Дата и время применения решения о проверке.                                                          |
| `applyResult`                   |`String`                      | Результат применения решения, один из `NotApplied`, `Success`или `NotSupported``Failed``NotFound` .                      |
| `accessRecommendation`          |`String`                      | Рекомендация, созданная функцией, показанная рецензенту, одна из `Approve``Deny` `NotAvailable`или . |


Кроме того, могут присутствовать дополнительные свойства в зависимости от типа объекта, который обладает доступом, который был принято решением.  Например, если решение о проверке доступа является членством определенного пользователя в группе или доступом к приложению, пользователь, который потенциально собирается удалить доступ, определяется с помощью следующих свойств:

| Свойство                        | Тип                         | Описание                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | Идентификатор пользователя, доступ которого был просмотрено.                                                                                    |
| `userDisplayName`                            |`String`                      | Отображаемое имя пользователя, доступ которого был просмотрено.                                                                                     |
| `userPrincipalName`                            |`String`                      | Имя участника-пользователя пользователя, доступ которого был просмотрено.                                                                                     |



## <a name="relationships"></a>Связи

Отсутствуют.  Объекты этого типа можно получить из проверки доступа с помощью решений [](../api/accessreview-listdecisions.md) и [связей mydecisions](../api/accessreview-listmydecisions.md) объекта [accessReview](accessreview.md).

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод списка решений accessReview](../api/accessreview-listdecisions.md) |      [Коллекция accessReviewDecision](accessreviewdecision.md)| Получение решений accessReview.|
|[Вывод списка решений accessReview](../api/accessreview-listmydecisions.md) |     [Коллекция accessReviewDecision](accessreviewdecision.md)| Как рецензент получите мои решения о accessReview.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


