---
title: Создание Акцессревиевсчедуледефинитион
description: Создание нового объекта Акцессревиевсчедуледефинитион.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9bf7cfb768134ce51e3f06b291da6726fe11a297
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000983"
---
# <a name="create-accessreviewscheduledefinition"></a>Создание Акцессревиевсчедуледефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений                            | AccessReview.ReadWrite.All |

Вошедшего в систему пользователя также должен находиться в роли каталога, позволяющей им создавать проверку доступа.  Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviewsv2-root.md).

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
|Авторизация|Bearer {токен}. Обязательный.|
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [акцессревиев](../resources/accessreview.md) в формате JSON.

В следующей таблице приведены свойства, принятые для создания Акцессревиев.

| Свойство | Тип | Описание |
|:-------------|:------------|:------------|
| displayName | Строка | Имя серии проверки доступа. Обязательный.|
| дескриптионфорадминс | строка | Контекст проверки, предоставленной администраторам. Обязательный. |
  дескриптионфорревиеверс | строка | Контекст проверки, предоставленной для рецензентов. Обязательный. |
| scope | [акцессревиевскопе](../resources/accessreviewscope.md) | Определяет область пользователей, проверенных в группе. Обратитесь к разделу  [акцессревиевскопе](../resources/accessreviewscheduledefinition.md). Обязательный.| 
| инстанцеенумератионскопе | [акцессревиевскопе](../resources/accessreviewscope.md) | В случае проверки всех групп это определяет область, в которой будут проверяться группы. Обратитесь к разделу [акцессревиевскопе](../resources/accessreviewscheduledefinition.md). | 
| settings | [акцессревиевсчедулесеттингс](../resources/accessreviewschedulesettings.md)| Параметры ряда проверки доступа. Здесь определяется повторение. Обратитесь к разделу [акцессревиевсчедулесеттингс](../resources/accessreviewscheduledefinition.md). |
| обсужден | Коллекция [акцессревиевревиеверскопе](../resources/accessreviewreviewerscope.md) | Определяет, кто является рецензентом. Если ничего не указано, проверка является самостоятельным обзором (пользователи, Просмотрели проверку собственного доступа). Обратитесь к разделу [акцессревиевревиеверскопе](../resources/accessreviewscheduledefinition.md). |


## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201, Created` код отклика и объект [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в тексте отклика.

## <a name="examples"></a>Примеры

Это пример создания серии проверки доступа с определенным пользователем, чей идентификатор объекта пользователя — 7eae4444-D425-48b2-adf2-3c777f6256f3, в качестве проверяющего. В ходе проверки просматриваются все члены определенной группы, чей объект Group ID имеет значение b7a059cb-038a-4802-8fc9-b9d1ed0c4444. Он повторяется еженедельно.

### <a name="request"></a>Запрос
В тексте запроса добавьте представление объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в формате JSON.

<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
  "displayName": "Test create",
  "descriptionForAdmins": "New scheduled access review",
  "descriptionForReviewers": "If you have any questions, contact jerry@contoso.com",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0c4444/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/7eae4444-d425-48b2-adf2-3c777f6256f3",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-08T12:02:30.667Z"
      }
    }
  }
}
```

### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "29f2d16e-9ca6-4052-bbfe-802c48944448",
    "displayName": "Test create",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
    "status": "NotStarted",
    "descriptionForAdmins": "Test create",
    "descriptionForReviewers": "Test create",
    "instanceEnumerationScope": null,
    "createdBy": {
        "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@microsoft.com"
    },
    "scope": {
        "query": "/groups/b74444cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "/users/7eae986b-d425-48b2-adf2-3c777f4444f3",
            "queryType": "MicrosoftGraph",
            "queryRoot": "decisions"
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 1,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "noEnd",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-08",
                "endDate": null
            }
        },
        "applyActions": []
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
