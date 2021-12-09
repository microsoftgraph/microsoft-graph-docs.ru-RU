---
title: 'educationAssignment: delta'
description: Получите список недавно созданных или обновленных назначений, не выполняя полную версию коллекции.
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1dab413675136bf7e8d33756e9701e4c537adb3e
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391173"
---
# <a name="educationassignment-delta"></a>educationAssignment: delta
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список недавно созданных или обновленных [назначений,](../resources/educationassignment.md) не выполняя полную версию коллекции.

Учитель или приложение, работая с разрешениями приложения, могут видеть все объекты **назначения** для класса. Учащиеся могут видеть **только назначения,** которые им назначены.

> **Примечание:** Этот метод не возвращает удаленные **назначения.**

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                                                         |
| Для приложений                            | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод не поддерживает `$expand` параметры `$orderby` запроса , `$search` и `$filter` OData.

Этот метод поддерживает только параметр `$top` запроса OData.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{educationClassId}/assignments/delta
GET /education/classes/{educationClassId}/members/{educationUserId}/assignments/delta
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения эта функция возвращает код ответа и `200 OK` коллекцию [educationAssignment](../resources/educationassignment.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-get-assignments-with-delta-query-support"></a>Пример 1. Получить назначения с поддержкой запроса delta

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. 

Используйте `$top` параметр, чтобы указать количество возвращаемого назначения. Параметр необязательный, но использовать его желательно, если у вас есть длинный список назначений; в противном случае вы получите все назначения в классе.

<!-- {
  "blockType": "request",
  "name": "get_assignments_delta"
}-->

```http
GET https://graph.microsoft.com/beta/education/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta?$top=2
```
---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание:** Возьмите `@odata.nextLink` ответ, чтобы сделать еще один вызов и получить следующий набор назначений.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(educationAssignment)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta?$skiptoken=U43TyYWKlRvJ6wWxZOfJvkp22nMqShRw9f-GxBtG2FDy9b1hMDaAJGdLb7n2fh1IdHoweKQs1czM4Ry1LVsNqwIFXftTcRHvgSCbcszvbJHEWDCO3QO7K7zwCM8DdXNepZOa1gqldecjIUM0NFRbGQoQ5yR6RmGnMgtko8TDMOyMH_yg1my82PTXA_t4Nj-DhMDZWvuNTd_lbLeTngc7mIJPMCR2gHN9CSKsW_kw850.UM9tUqwOu5Ln1pnxaP6KdMmfJHszGqY3EKPlQkOiyGs",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationAssignment",
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 3.1",
            "closeDateTime": "2021-11-14T07:59:00Z",
            "dueDateTime": "2021-11-14T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": "2021-11-10T23:57:16.1897643Z",
            "allowLateSubmissions": false,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:56:03.7992389Z",
            "lastModifiedDateTime": "2021-11-11T00:42:20.8999693Z",
            "allowStudentsToAddResourcesToSubmission": false,
            "status": "published",
            "notificationChannelUrl": "https://graph.microsoft.com/beta/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:e375b98b9d4f4738857fb70f23d329b7@thread.skype",
            "webUrl": null,
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "grading": null,
            "id": "3b870c07-21fe-47fb-8562-cdd6f2c281d6",
            "instructions": {
                "content": "follow up",
                "contentType": "text"
            },
            "assignTo": {
                "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
            },
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationAssignment",
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 4",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": null,
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:58:29.2670914Z",
            "lastModifiedDateTime": "2021-11-10T23:58:39.6191021Z",
            "allowStudentsToAddResourcesToSubmission": true,
            "status": "draft",
            "notificationChannelUrl": null,
            "webUrl": null,
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "grading": null,
            "id": "34ab8c17-eaae-4996-9c04-53696934e6ff",
            "instructions": {
                "content": "",
                "contentType": "text"
            },
            "assignTo": {
                "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
            },
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        }
    ]
}
```

### <a name="example-2-get-next-set-of-assignments-with-delta-query-support"></a>Пример 2. Получить следующий набор назначений с поддержкой запроса delta

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

Используйте значение `@odata.nextLink` из предыдущего вызова для этого запроса.

<!-- {
  "blockType": "request",
  "name": "get_assignments_delta"
}-->

```http
GET /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta?$skiptoken=U43TyYWKlRvJ6wWxZOfJvkp22nMqShRw9f-GxBtG2FDy9b1hMDaAJGdLb7n2fh1IdHoweKQs1czM4Ry1LVsNqwIFXftTcRHvgSCbcszvbJHEWDCO3QO7K7zwCM8DdXNepZOa1gqldecjIUM0NFRbGQoQ5yR6RmGnMgtko8TDMOyMH_yg1my82PTXA_t4Nj-DhMDZWvuNTd_lbLeTngc7mIJPMCR2gHN9CSKsW_kw850.UM9tUqwOu5Ln1pnxaP6KdMmfJHszGqY3EKPlQkOiyGs
```
---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание:** Вы должны продолжать использовать значение для последующих вызовов, пока не `@odata.nextLink` получите свойство в `@odata.deltaLink` ответе.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(educationAssignment)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxROmLjac48n-iXm5j6n5aQwlsnC-2OvL3lI0Z8M4klERNmJQjnBn7MHqwXZ6L8GlI3VPnya3E-p1bisiZX97jLvQUAopseIYhvnD6v7fiYrk.fVsHempT6X2CiBh6aN9Ex5nVJ71adKdcf-mdke8OHKs",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationAssignment",
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options 2",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": "2021-11-10T23:54:15.9533379Z",
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:51:08.8548584Z",
            "lastModifiedDateTime": "2021-11-10T23:54:17.4687411Z",
            "allowStudentsToAddResourcesToSubmission": true,
            "status": "assigned",
            "notificationChannelUrl": null,
            "webUrl": null,
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "grading": null,
            "id": "efa3b9a8-b41f-4263-adc5-738c01912153",
            "instructions": {
                "content": "",
                "contentType": "text"
            },
            "assignTo": {
                "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
            },
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "AAAAAAAA-0123-4567-89AB-1B4BB48C3119",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationAssignment",
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "Expand options in publish",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": "2021-11-10T23:48:03.9134549Z",
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:42:37.2869391Z",
            "lastModifiedDateTime": "2021-11-10T23:48:06.490359Z",
            "allowStudentsToAddResourcesToSubmission": true,
            "status": "assigned",
            "notificationChannelUrl": null,
            "webUrl": null,
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "grading": null,
            "id": "5cf13354-0156-4483-8c19-3185c6252188",
            "instructions": {
                "content": "",
                "contentType": "text"
            },
            "assignTo": {
                "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
            },
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "AAAAAAAA-0123-4567-89AB-1B4BB48C3119",
                    "displayName": null
                }
            }
        }
    ]
}
```

### <a name="example-3-get-the-created-and-modified-assignments-using-delta-token"></a>Пример 3. Получить созданные и измененные назначения с помощью маркера delta

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

Используйте значение `@odata.deltaLink` из предыдущего вызова для этого запроса.

<!-- {
  "blockType": "request",
  "name": "get_assignments_delta"
}-->

```http
GET /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxROmLjac48n-iXm5j6n5aQwlsnC-2OvL3lI0Z8M4klERNmJQjnBn7MHqwXZ6L8GlI3VPnya3E-p1bisiZX97jLvQUAopseIYhvnD6v7fiYrk.fVsHempT6X2CiBh6aN9Ex5nVJ71adKdcf-mdke8OHKs
```
---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание:** Вы должны продолжать использовать для получения вновь созданных или измененных `@odata.deltaLink` назначений с момента первоначального вызова Delta.

>Иногда ответ дельты будет очень большим, и в этом случае будет возвращено, чтобы продолжить извлечение изменений до тех пор, `@odata.nextLink` пока вы не нажметесь `@odata.deltaLink` снова.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(educationAssignment)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxROmLjac48n-iXm5j6n5aQwlsnC-2OvL3lI0Z8M4klER9TeVMFnEEWX3TRYFAJe1nNUp5s0cjvqM59nMNhcFoIhmt6RUUcXe6vlP9yy00ADA.gT8PrGKC3hZnt4oDxMAmjyX50EASWG4KNcc1E9yTRRo",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationAssignment",
            "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "displayName": "expand options 2 updated for delta",
            "closeDateTime": null,
            "dueDateTime": "2021-11-12T07:59:00Z",
            "assignDateTime": null,
            "assignedDateTime": "2021-11-10T23:54:15.9533379Z",
            "allowLateSubmissions": true,
            "resourcesFolderUrl": null,
            "createdDateTime": "2021-11-10T23:51:08.8548584Z",
            "lastModifiedDateTime": "2021-11-16T15:17:07.518655Z",
            "allowStudentsToAddResourcesToSubmission": true,
            "status": "assigned",
            "notificationChannelUrl": null,
            "webUrl": null,
            "addToCalendarAction": "none",
            "addedStudentAction": "none",
            "grading": null,
            "id": "efa3b9a8-b41f-4263-adc5-738c01912153",
            "instructions": {
                "content": "",
                "contentType": "text"
            },
            "assignTo": {
                "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
            },
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
                    "displayName": null
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d80
2021-11-18 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
