---
title: Получение accessReview
description: 'В Azure AD access дается обзор компонента, извлечение объекта accessReview.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a13776b9aa215d752797b6ba2de2f477660ed31d
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016662"
---
# <a name="get-accessreview"></a>Получение accessReview

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечение объекта [accessReview](../resources/accessreview.md) .  

Чтобы получить рецензентов проверки доступа, используйте [рецензентов accessReview список](accessreview-listreviewers.md) API. Для получения решения проверки доступа, используйте API [решения accessReview списка](accessreview-listdecisions.md) или интерфейса API [Мои accessReview решения](accessreview-listmydecisions.md) .

Если это повторяющееся проверки доступа, используйте `instances` связь для получения коллекции [accessReview](../resources/accessreview.md) ранее, текущие и будущие экземпляры проверки доступа.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа или назначен в качестве проверяющего на странице проверьте доступ. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носителя \{маркеров\}. Обязательная часть. |

## <a name="request-body"></a>Тело запроса
Нет текста запроса должен задаваться.

## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `200, OK` код ответа и объект [accessReview](../resources/accessreview.md) в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание accessReview](accessreview-create.md) |    [accessReview](../resources/accessreview.md) |  Создание нового accessReview. |
|[Список programControls](programcontrol-list.md) | [programControl](../resources/programcontrol.md) коллекции | Список programControls в клиент. |
|[Список accessReview рецензентов](accessreview-listreviewers.md) |     Коллекция [удостоверению пользователя](../resources/useridentity.md)|    Получите рецензентов accessReview. |
|[Список accessReview решения](accessreview-listdecisions.md) |     [accessReviewDecision](../resources/accessreviewdecision.md) коллекции|    Получите решения accessReview.|
|[Мои accessReview решения](accessreview-listmydecisions.md) |        [accessReviewDecision](../resources/accessreviewdecision.md) коллекции|    В качестве читателя получите Мои решения accessReview.|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
