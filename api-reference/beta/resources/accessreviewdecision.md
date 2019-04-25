---
title: Тип ресурса АкцессревиевдеЦисион
description: В функции рецензирования Access в `accessReviewDecision` Azure AD — представляет решение для проверки доступа к определенному объекту в Azure AD.  При просмотре доступа или экземпляре повторяющейся проверки доступа существует один `accessReviewDecision` проверенный пользователь.  Например, если в группе есть два гостей и один не гость, а для этой группы выполняется проверка доступа для гостей, то будут доступны два объекта решения для проверки доступа.  Если проверяющий изменяет свое решение или другой проверяющий переопределяет их, `accessReviewDecision` то обновляется.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9642c8a51e4e9efe1a1748243b0e24aeff07cfa0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535779"
---
# <a name="accessreviewdecision-resource-type"></a>Тип ресурса АкцессревиевдеЦисион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции рецензирования [Access](accessreviews-root.md) в `accessReviewDecision` Azure AD — представляет решение для проверки доступа к определенному объекту в Azure AD.  При просмотре доступа или экземпляре повторяющейся проверки доступа существует один `accessReviewDecision` проверенный пользователь.  Например, если в группе есть два гостей и один не гость, а для этой группы выполняется проверка доступа для гостей, то будут доступны два объекта решения для проверки доступа.  Если проверяющий изменяет свое решение или другой проверяющий переопределяет их, `accessReviewDecision` то обновляется.


## <a name="methods"></a>Методы

Нет.  Объекты этого типа автоматически создаются компонентом при инициализации проверки доступа и не могут быть удалены.  Они могут извлекаться из проверки доступа с помощью связей " [решения](../api/accessreview-listdecisions.md) " и " [мидеЦисионс](../api/accessreview-listmydecisions.md) ".

## <a name="properties"></a>Свойства

В этой таблице показаны основные свойства объектов этого типа. 

| Свойство                        | Тип                         | Описание                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | Идентификатор решения в рамках проверки доступа.                                                                                     |
| `accessReviewId`                |`String`                      | Созданный компонентом идентификатор проверки доступа.                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| Удостоверение проверяющего.                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | Дата и время, когда было предоставлено Последнее рецензирование для этого права доступа.                                                                         |
| `reviewResult`                  |`String`                      | Результат проверки.                                                                                    |
| `justification`                 |`String`                      | Деловое обоснование проверяющего, если оно указано.                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| По завершении проверки, если результаты были вручную применены, удостоверение пользователя, который применил решение.                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | Дата и время применения решения проверки.                                                          |
| `applyResult`                   |`String`                      | Результат `NotApplied`применения решения, один из, `Success` `Failed`, `NotFound` или. `NotSupported`                      |
| `accessRecommendation`          |`String`                      | Созданная с помощью функции рекомендация, показанная рецензенту, один из `Approve` `Deny` или `NotAvailable`. |


Кроме того, могут присутствовать дополнительные свойства в зависимости от типа объекта, которому назначен доступ.  Например, если решение "Проверка доступа" является участником группы определенного пользователя или доступом к приложениям, то пользователь, который может получить доступ к нему, будет удален с помощью следующих свойств:

| Свойство                        | Тип                         | Описание                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | Идентификатор пользователя, доступ к которому был проверен.                                                                                    |
| `userDisplayName`                            |`String`                      | Отображаемое имя пользователя, доступ к которому был проверен.                                                                                     |
| `userPrincipalName`                            |`String`                      | Имя участника пользователя, для которого был проверен доступ.                                                                                     |



## <a name="relationships"></a>Связи

Отсутствуют.  Объекты этого типа можно получить из проверки доступа с помощью отношений [решений](../api/accessreview-listdecisions.md) и [МидеЦисионс](../api/accessreview-listmydecisions.md) в объекте [акцессревиев](accessreview.md) .

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список решений Акцессревиев](../api/accessreview-listdecisions.md) |      Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)| Получение решений для Акцессревиев.|
|[Список моих решений Акцессревиев](../api/accessreview-listmydecisions.md) |     Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)| В качестве проверяющего получите мое решение Акцессревиев.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviewdecision.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
