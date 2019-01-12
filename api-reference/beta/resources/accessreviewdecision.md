---
title: Тип ресурса accessReviewDecision
description: В Azure AD access дается обзор компонента, `accessReviewDecision` представляет Azure AD access review принятия решения об доступа к конкретной сущности.  В рамках проверки доступа, или экземпляр повторяющейся проверки доступа, существует один `accessReviewDecision` на проверенные пользователя.  К примеру Если группы имеет два Гости и один не гостевая-как члены и обзор доступа с гостевым выполняется для этой группы будет двух объектов решений проверки доступа.  Если проверяющий изменяет их принятия решений или другой редактор переопределяет их, а затем `accessReviewDecision` обновляется.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b10a53726e12c37a598f8df735a3f70174c807
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977558"
---
# <a name="accessreviewdecision-resource-type"></a>Тип ресурса accessReviewDecision

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `accessReviewDecision` представляет Azure AD access review принятия решения об доступа к конкретной сущности.  В рамках проверки доступа, или экземпляр повторяющейся проверки доступа, существует один `accessReviewDecision` на проверенные пользователя.  К примеру Если группы имеет два Гости и один не гостевая-как члены и обзор доступа с гостевым выполняется для этой группы будет двух объектов решений проверки доступа.  Если проверяющий изменяет их принятия решений или другой редактор переопределяет их, а затем `accessReviewDecision` обновляется.


## <a name="methods"></a>Methods

Нет.  Объекты данного типа автоматически создаются с помощью функции при доступе просмотрите инициализирует и не может быть удалена.  Они могут быть получены из проверки доступа с помощью [решения](../api/accessreview-listdecisions.md) и [mydecisions](../api/accessreview-listmydecisions.md) связи.

## <a name="properties"></a>Свойства

В данной таблице представлены основные свойства объектов этого типа. 

| Свойство                        | Тип                         | Описание                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | Идентификатор решения в рамках проверки доступа.                                                                                     |
| `accessReviewId`                |`String`                      | Идентификатор созданного компонента проверки доступа.                                                                                       |
| `reviewedBy`                    |[удостоверению пользователя](useridentity.md)| Удостоверение проверяющий.                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | Дата и время последней проверки базы данных для доступа к справа было задано.                                                                         |
| `reviewResult`                  |`String`                      | Результат проверки.                                                                                    |
| `justification`                 |`String`                      | Деловое обоснование рецензента, если указано.                                                                         |
| `appliedBy`                     |[удостоверению пользователя](useridentity.md)| После завершения проверки, если результаты были применены вручную, пользователь идентификатор пользователя, который применяется решение.                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | Дата и время, когда была применена Обзор решения.                                                          |
| `applyResult`                   |`String`                      | Результат применения принятия решений, один из `NotApplied`, `Success`, `Failed`, `NotFound` или `NotSupported`.                      |
| `accessRecommendation`          |`String`                      | Рекомендация созданный компонент-показано проверяющему, один из `Approve`, `Deny` или `NotAvailable`. |


Кроме того в зависимости от типа объекта имеет доступ, которое было принято решение после объекта может присутствовать дополнительные свойства.  Например если решение проверки доступа членство в группах конкретному пользователю или доступ к приложениям, пользователи, которые потенциально будут иметь доступ удалены идентифицируется через эти свойства:

| Свойство                        | Тип                         | Описание                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | Идентификатор пользователя, которого доступа прошел проверку.                                                                                    |
| `userDisplayName`                            |`String`                      | Отображаемое имя пользователя, которого доступа прошел проверку.                                                                                     |
| `userPrincipalName`                            |`String`                      | Имя пользователя участника пользователя, которого доступа прошел проверку.                                                                                     |



## <a name="relationships"></a>Связи

Нет.  Объекты данного типа можно извлечь из проверки доступа с помощью [решения](../api/accessreview-listdecisions.md) и [mydecisions](../api/accessreview-listmydecisions.md) связи объекта [accessReview](accessreview.md) .

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список accessReview решения](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md) коллекции| Получите решения accessReview.|
|[Мои accessReview решения](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md) коллекции| В качестве читателя получите Мои решения accessReview.|

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

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
