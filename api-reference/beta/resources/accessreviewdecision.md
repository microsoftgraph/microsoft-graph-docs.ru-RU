---
title: Тип ресурса accessReviewDecision
description: В Azure AD access дается обзор компонента, `accessReviewDecision` представляет Azure AD access review принятия решения об доступа к конкретной сущности.  В рамках проверки доступа, или экземпляр повторяющейся проверки доступа, существует один `accessReviewDecision` на проверенные пользователя.  К примеру Если группы имеет два Гости и один не гостевая-как члены и обзор доступа с гостевым выполняется для этой группы будет двух объектов решений проверки доступа.  Если проверяющий изменяет их принятия решений или другой редактор переопределяет их, а затем `accessReviewDecision` обновляется.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9642c8a51e4e9efe1a1748243b0e24aeff07cfa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517402"
---
# <a name="accessreviewdecision-resource-type"></a>Тип ресурса accessReviewDecision

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `accessReviewDecision` представляет Azure AD access review принятия решения об доступа к конкретной сущности.  В рамках проверки доступа, или экземпляр повторяющейся проверки доступа, существует один `accessReviewDecision` на проверенные пользователя.  К примеру Если группы имеет два Гости и один не гостевая-как члены и обзор доступа с гостевым выполняется для этой группы будет двух объектов решений проверки доступа.  Если проверяющий изменяет их принятия решений или другой редактор переопределяет их, а затем `accessReviewDecision` обновляется.


## <a name="methods"></a>Методы

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



## <a name="relationships"></a>Отношения

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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviewdecision.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
