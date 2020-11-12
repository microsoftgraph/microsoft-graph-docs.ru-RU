---
title: Получение Акцессревиевсчедуледефинитион
description: Получение объекта Акцессревиевсчедуледефинитион.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6c5619222eb8a96fbf54a8f796abdc2d2bb85ec
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000991"
---
# <a name="get-accessreviewscheduledefinition"></a>Получение Акцессревиевсчедуледефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) по идентификатору. Возвращает все свойства серии проверки доступа "запланированный доступ", за исключением связанного Акцессревиевинстанцес. У каждого Акцессревиевсчедуледефинитион есть по крайней мере один экземпляр. Экземпляр представляет проверку для определенного ресурса (например, членов определенной группы), в течение одного экземпляра (например, Март 2021) повторяющейся проверки.

Чтобы получить экземпляры серии проверки доступа, используйте [акцессревиевинстанце API List](accessreviewinstance-list.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL  |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений                            | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL |

Чтобы вызвать этот API, вошедшего в систему пользователь должен также находиться в роли каталога, который позволяет им читать проверку доступа, или пользователь может быть назначен в качестве проверяющего при проверке доступа.  Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviewsv2-root.md).

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a>Заголовки запросов
Нет.

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в тексте отклика.

## <a name="examples"></a>Примеры
### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
---

### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "60860cdd-fb4d-4054-91ba-f7544443baa6",
    "displayName": "Test world",
    "createdDateTime": "2020-09-14T20:03:36.7391027Z",
    "lastModifiedDateTime": "2020-09-14T20:04:28Z",
    "status": "InProgress",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "createdBy": {
        "id": "957f1027-c0ee-460d-4444-b8828e59e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@microsoft.com"
    },
    "scope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b944440cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b9d14444f11f",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 0,
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
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-15",
                "endDate": "9999-12-31"
            }
        }
    }
}
```

## <a name="see-also"></a>См. также

- [Создание Акцессревиевсчедуледефинитион](accessreviewscheduledefinition-create.md)
- [Список Акцессревиевсчедуледефинитион](accessreviewscheduledefinition-list.md)
- [Список Акцессревиевинстанце](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
