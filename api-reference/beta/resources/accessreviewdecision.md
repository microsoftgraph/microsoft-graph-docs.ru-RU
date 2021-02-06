---
title: Тип ресурса accessReviewDecision
description: AccessReviewDecision представляет решение о проверке доступа Azure AD для доступа определенной сущности.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c33849920a06154f0c2a0ac781dcd5cdf64fa51f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133520"
---
# <a name="accessreviewdecision-resource-type"></a>Тип ресурса accessReviewDecision

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции [проверки](accessreviews-root.md) доступа Azure AD эта функция представляет решение о проверке доступа Azure AD для доступа `accessReviewDecision` определенной сущности.  В рамках проверки доступа или экземпляра рецензии на повторяющийся доступ имеется один экземпляр для `accessReviewDecision` каждого проверяемого пользователя.  Например, если группа имеет двух гостей и одного не из них в качестве участников, а для нее выполняется проверка доступа гостей, то будут два объекта принятия решений для проверки доступа.  Если рецензент изменяет свое решение или другой рецензент переопределяет его, то `accessReviewDecision` обновляется.


## <a name="methods"></a>Методы

Нет.  Объекты этого типа автоматически создаются функцией при инициализации проверки доступа и не могут быть удалены.  Их можно получить из проверки доступа с помощью [решений](../api/accessreview-listdecisions.md) и [связей mydecisions.](../api/accessreview-listmydecisions.md)

## <a name="properties"></a>Свойства

В этой таблице иллюстрируют базовые свойства объектов этого типа. 

| Свойство                        | Тип                         | Описание                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | ИД решения в рамках проверки доступа.                                                                                     |
| `accessReviewId`                |`String`                      | Созданный функцией ид проверки доступа.                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| Удостоверение проверяющего. Если рекомендация использовалась в качестве отзыва, userPrincipalName пуст.                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | Дата и время последнего отзыва для этого права доступа.                                                                         |
| `reviewResult`                  |`String`                      | Результат проверки, один из `NotReviewed` `Deny` , или `DontKnow` `Approve` .                                                                                    |
| `justification`                 |`String`                      | Бизнес-обоснование проверяемой, если она предоставлена.                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| После завершения проверки, если результаты были применены вручную, удостоверение пользователя, который применил решение. Если отзыв был применен автоматически, userPrincipalName пуст.                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | Дата и время принятия решения об отзыве.                                                          |
| `applyResult`                   |`String`                      | Результат применения решения, один из `NotApplied` `Success` , , или `Failed` `NotFound` `NotSupported` .                      |
| `accessRecommendation`          |`String`                      | Рекомендация, сгенерированная функцией, показанная рецензенту, одна из или `Approve` `Deny` `NotAvailable` . |


Кроме того, могут присутствовать дополнительные свойства в зависимости от типа объекта, обладания доступом, который был решен.  Например, если решением для проверки доступа является членство определенного пользователя в группе или доступ к приложению, пользователь, который потенциально собирается получить доступ, будет удален с помощью этих свойств:

| Свойство                        | Тип                         | Описание                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | ИД пользователя, доступ к которым был рассмотрен.                                                                                    |
| `userDisplayName`                            |`String`                      | Отображаемого имени пользователя, доступ к которым был рассмотрен.                                                                                     |
| `userPrincipalName`                            |`String`                      | Имя пользователя, доступ к которым был проанализировано.                                                                                     |



## <a name="relationships"></a>Связи

Отсутствуют.  Объекты этого типа можно получить из проверки доступа с помощью решений и связей [mydecisions](../api/accessreview-listmydecisions.md) объекта [accessReview.](accessreview.md) [](../api/accessreview-listdecisions.md)

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список решений accessReview](../api/accessreview-listdecisions.md) |      [Коллекция accessReviewDecision](accessreviewdecision.md)| Получите решения accessReview.|
|[Список решений accessReview](../api/accessreview-listmydecisions.md) |     [Коллекция accessReviewDecision](accessreviewdecision.md)| Как рецензент получите мои решения по accessReview.|

## <a name="json-representation"></a>Представление в формате JSON

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


