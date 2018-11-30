---
title: Список accessReview решения
description: В Azure AD access дается обзор компонента, извлечение решения accessReview объекта.
ms.openlocfilehash: d8cf89706f053dfee6e98cdf23d2539874ac6997
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076019"
---
# <a name="list-accessreview-decisions"></a>Список accessReview решения

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечения решения [accessReview](../resources/accessreview.md) объекта.

Обратите внимание, что повторяющиеся проверки доступа, не будут иметь `decisions` отношения.  Вместо этого необходимо перейти вызывающего `instance` отношения, чтобы найти `accessReview` объект для текущей или последние экземпляр проверки доступа.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носителя \{маркеров\}. Обязательный атрибут. |

## <a name="request-body"></a>Текст запроса
Нет текста запроса должен задаваться.

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [accessReviewDecision](../resources/accessreviewdecision.md) в теле ответа.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
|[Мои accessReview решения](accessreview-listmydecisions.md) |        [accessReviewDecision](../resources/accessreviewdecision.md) коллекции|    В качестве читателя получите Мои решения accessReview.|
|[Отправлять напоминание accessReview](accessreview-sendreminder.md) |       Отсутствуют.   |   Отправьте напоминание, чтобы проверяющие accessReview. |
|[Остановка accessReview](accessreview-stop.md) |        Отсутствуют.   |   Остановите accessReview. |
|[Сброс accessReview решения](accessreview-reset.md) |        Отсутствуют.   |   Сброс решения, принимаемые при accessReview в хода выполнения.|
|[Применение accessReview решения](accessreview-apply.md) |        Отсутствуют.   |   Применение решения из завершенных accessReview.|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
