---
title: Мои accessReview решения
description: В компоненте обзоры доступа Azure AD извлечение решения объект accessReview для вызывающего пользователя в виде редактор.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 037b916bca45c74d1918b45e4e9e21b685bd8ae0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941501"
---
# <a name="list-my-accessreview-decisions"></a>Мои accessReview решения

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечение решения объект [accessReview](../resources/accessreview.md) для вызывающего пользователя в виде редактор.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  Выполнен вход пользователей необходимо также могут читать этот анализ конкретного клиента. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | строка | Носителя \{маркеров\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Нет текста запроса должен задаваться.

## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [accessReviewDecision](../resources/accessreviewdecision.md) в теле ответа, для которого вызывающего пользователя — это назначенный редактор.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение accessReview](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  Получите обзор доступа. |
|[Список accessReview решения](accessreview-listdecisions.md) |     [accessReviewDecision](../resources/accessreviewdecision.md) коллекции|    Получите все решения accessReview.|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
