---
title: Создание accessReview
description: В функции обзоров доступа Azure AD создайте новый объект accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d53f0335ed9b130be65611d049645aba6a7abe44
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439410"
---
# <a name="create-accessreview"></a>Создание accessReview

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) создайте новый [объект accessReview.](../resources/accessreview.md)

Прежде чем сделать этот запрос, [](businessflowtemplate-list.md)звонявший должен ранее получить список шаблонов бизнес-потока, чтобы иметь значение включить `businessFlowTemplateId` в запрос.

После этого запроса вызываемая должна [создать программуControl,](programcontrol-create.md)чтобы связать обзор доступа с программой.  

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | AccessReview.ReadWrite.Membership |

Вызываемая должна также иметь разрешение ProgramControl.ReadWrite.All, чтобы после создания обзора доступа вызываемая мог создать [программуControl](../resources/programcontrol.md).
Кроме того, подписанный пользователь также должен быть в роли каталога, что позволяет им создавать обзор доступа.  Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviews-root.md)

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
| Authorization | Носитель \{токен\}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [accessReview.](../resources/accessreview.md)

В следующей таблице показаны свойства, необходимые при создании accessReview.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | Имя обзора доступа.  |
| `startDateTime`           |`DateTimeOffset`                                                | DateTime, когда планируется начать проверку.  Это должна быть дата в будущем.   |
| `endDateTime`             |`DateTimeOffset`                                                | DateTime, когда проверка должна завершиться. Это должно быть по крайней мере на один день позже даты начала.   |
| `description`             |`String`                                                        | Описание, чтобы показать рецензентам. |
| `businessFlowTemplateId`  |`String`                                                        | Идентификатор шаблона бизнес-потока, полученный из [businessFlowTemplate.](../resources/businessflowtemplate.md)  |
| `reviewerType`            |`String`                                                        | Тип отношения рецензента к правам доступа к рассмотренного объекта, одного из `self` , `delegated` или `entityOwners` . | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | Объект, для которого создается обзор доступа, например членство в группе или назначения пользователей приложению. | 


Если предоставленный reviewerType имеет значение, то вызываемая должна также включать свойство с коллекцией `delegated` `reviewers` [userIdentity](../resources/useridentity.md) рецензентов.

Если приложение вызывает этот API без подписанного пользователя, вызываемая должна также включать свойство **createdBy,** значение для которого является [объектом userIdentity](../resources/useridentity.md) пользователя, который будет определен в качестве создателя отзыва.

Кроме того, вызывающее может включать параметры, чтобы создать повторяющиеся серии обзоров или изменить поведение проверки по умолчанию. В частности, чтобы создать повторяющийся обзор, вызывающий должен включить параметры обзора `accessReviewRecurrenceSettings` доступа,


## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201, Created` [объект accessReview](../resources/accessreview.md) в тексте ответа.

## <a name="example"></a>Пример

Это пример создания разового (не повторяющегося) обзора доступа, явно указывав двух пользователей в качестве рецензентов.

### <a name="request"></a>Запрос
В теле запроса поставляем JSON-представление [объекта accessReview.](../resources/accessreview.md)

<!-- {
  "blockType": "ignored",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b"
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```

### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


