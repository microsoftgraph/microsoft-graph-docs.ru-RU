---
title: Создание Акцессревиев
description: В средстве проверки доступа Azure AD создайте новый объект Акцессревиев.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5247bacbbf15274f132c5d7620b806cfe99613b6
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287458"
---
# <a name="create-accessreview"></a>Создание Акцессревиев

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В средстве проверки [доступа](../resources/accessreviews-root.md) Azure AD создайте новый объект [акцессревиев](../resources/accessreview.md) .

Перед выполнением этого запроса абонент должен был [получить список шаблонов бизнес-процесса](businessflowtemplate-list.md), чтобы `businessFlowTemplateId` включить в запрос значение для включения в запрос.

После выполнения этого запроса вызывающий абонент должен [создать програмконтрол](programcontrol-create.md), чтобы связать проверку доступа с программой.  

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | AccessReview.ReadWrite.Membership |

Вызывающая сторона также должна иметь разрешение Програмконтрол. ReadWrite. ALL, чтобы после создания проверки доступа вызывающий абонент может создать [програмконтрол](../resources/programcontrol.md).
Кроме того, пользователь, вошедшего в систему, должен быть членом роли каталога, который позволяет им создавать проверку доступа.  Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviews-root.md).

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [акцессревиев](../resources/accessreview.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Акцессревиев.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | Имя проверки доступа.  |
| `startDateTime`           |`DateTimeOffset`                                                | Дата и время, когда выполняется запланированное начало проверки.  Это должна быть Дата в будущем.   |
| `endDateTime`             |`DateTimeOffset`                                                | Дата и время окончания запланированного рассмотрения. Это должен быть по крайней мере один день позже даты начала.   |
| `description`             |`String`                                                        | Описание, которое будет отображаться для рецензентов. |
| `businessFlowTemplateId`  |`String`                                                        | Идентификатор шаблона рабочего процесса, полученный из объекта [бусинессфловтемплате](../resources/businessflowtemplate.md).  |
| `reviewerType`            |`String`                                                        | Тип отношения проверяющего к правам доступа проверенного объекта, один из `self` , `delegated` или `entityOwners` . | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | Объект, для которого создается проверка доступа, например членство в группе или назначения пользователей приложению. | 


Если предоставленное значение Ревиевертипе имеет значение `delegated` , вызывающая сторона также должна содержать `reviewers` свойство с коллекцией [userIdentity](../resources/useridentity.md) рецензентов.

Если приложение вызывает этот API без вошедшего пользователя, вызывающая сторона также должна включать свойство **createdBy** , значение которого является [userIdentity](../resources/useridentity.md) пользователя, который будет идентифицирован как создатель проверки.

Кроме того, вызывающий может включать в себя параметры для создания повторяющихся рядов проверки или для изменения поведения проверки по умолчанию. В частности, чтобы создать повторяющуюся проверку, вызывающая сторона должна включать в себя `accessReviewRecurrenceSettings` Параметры проверки доступа,


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.

## <a name="example"></a>Пример

Это пример создания одноразовой (не повторяющейся) проверки доступа, явно указав двух пользователей в качестве проверяющих.

### <a name="request"></a>Запрос
В тексте запроса добавьте представление объекта [акцессревиев](../resources/accessreview.md) в формате JSON.

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
