---
title: 'educationSubmission: reassign'
description: Повторное отправку студенту с отзывами для рассмотрения.
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 80bd60236a68c06e5abca5fd4bef90fc28ef3211
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777391"
---
# <a name="educationsubmission-reassign"></a>educationSubmission: reassign

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Повторное отправку [студенту](../resources/educationsubmission.md) с отзывами для рассмотрения.

Выполнить это действие могут только преподаватели. 

Включай заготок при вызове этого метода; в противном случае повторно назначенная отправка будет рассматриваться как `Prefer: include-unknown-enum-members` возвращенная отправка. Это означает, что состояние будет соединяться с состоянием, а свойства `reassigned` `returned` **reassignedDateTime** и **reassignedBy** будут соединяться с **returnedDateTime** и **returnedBy** соответственно.

Если `Prefer: include-unknown-enum-members` заготавка предоставлена, повторно назначенное представление сохраняет `reassigned` состояние. Подробные сведения см. в разделе Примеры.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite   |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | Не поддерживается. | 

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Prefer  | `include-unknown-enum-members`. Необязательное свойство.  |

## <a name="request-body"></a>Текст запроса
Не поставляем тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `200 OK` объект [educationSubmission](../resources/educationsubmission.md) в тексте ответа.

## <a name="examples"></a>Примеры
### <a name="example-1-request-without-optional-prefer-header"></a>Пример 1. Запрос без необязательного загона Prefer

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "educationsubmission_reassign"
}-->

```http
POST /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/7192332b-e904-4891-81e2-356242ab1858/submissions/02bb5de1-7205-2a25-fe33-f99cf53de1c4/reassign
```

#### <a name="response"></a>Отклик
Ниже приводится пример ответа, когда не предоставляется в загона запроса и отправка не `Prefer: include-unknown-enum-members` была возвращена ранее.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationSubmission",
    "@odata.type": "#microsoft.graph.educationSubmission",
    "status": "returned",
    "submittedDateTime": "2021-09-07T14:54:46.1606962Z",
    "unsubmittedDateTime": "2021-09-07T14:41:18.9512645Z",
    "returnedDateTime": "2021-09-07T21:38:40.5254847Z",
    "reassignedDateTime": "2021-09-07T21:38:40.5254847Z",
    "resourcesFolderUrl": null,
    "id": "02bb5de1-7205-2a25-fe33-f99cf53de1c4",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "80cefd93-8d88-40e2-b5d3-67898383e226"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    },
    "reassignedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    }
}
```

### <a name="example-2-request-with-prefer-header"></a>Пример 2. Запрос с помощью загона Prefer
В следующем примере показано, как вызвать этот метод.

#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "educationsubmission_prefer_reassign"
}-->

```http
POST /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/7192332b-e904-4891-81e2-356242ab1858/submissions/02bb5de1-7205-2a25-fe33-f99cf53de1c4/reassign
Prefer: include-unknown-enum-members
```

#### <a name="response"></a>Отклик
Ниже приводится пример ответа, когда в заглавной части запроса предоставляется ответ, и отправка не `Prefer: include-unknown-enum-members` была возвращена ранее.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationSubmission",
    "@odata.type": "#microsoft.graph.educationSubmission",
    "status": "reassigned",
    "submittedDateTime": "2021-09-07T21:44:41.8377109Z",
    "unsubmittedDateTime": "2021-09-07T14:41:18.9512645Z",
    "returnedDateTime": null,
    "reassignedDateTime": "2021-09-07T21:45:42.9027726Z",
    "resourcesFolderUrl": null,
    "id": "02bb5de1-7205-2a25-fe33-f99cf53de1c4",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "80cefd93-8d88-40e2-b5d3-67898383e226"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "reassignedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    }
}
```

## <a name="see-also"></a>См. также

* [Состояния, переходы и ограничения для назначений и представлений](/graph/assignments-submissions-states-transition)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: reassign",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


