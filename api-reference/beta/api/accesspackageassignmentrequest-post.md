---
title: Создание accessPackageAssignmentRequest
description: Создание нового accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d455bde8192cfd37713d32f10e5bb8d8b908cec0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868877"
---
# <a name="create-accesspackageassignmentrequest"></a>Создание accessPackageAssignmentRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)создайте новый объект [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)  Эта операция используется для назначения пользователя пакету доступа или удаления назначения пакета доступа.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

Для администратора, запрашиваемого для создания назначения для пользователя, значение свойства **requestType** составляет , а свойство `AdminAdd` **accessPackageAssignment** содержит назначенного пользователя, свойство `targetId` **assignmentPolicyId,** определяющий [accessPackageAssignmentPolicy,](../resources/accesspackageassignmentpolicy.md)и **свойство accessPackageId,** определяющий [accessPackageage.](../resources/accesspackage.md)

Для администратора, запрашиваемого для удаления назначения, значение свойства **requestType** составляет , а свойство accessPackageAssignment содержит свойство id, определяющий удаляемую `AdminRemove`  [accessPackageAssignment.](../resources/accesspackageassignment.md) 

Чтобы пользователь, не вступив в администратор, попросил создать свое собственное назначение для первого назначения или возобновления назначения, значение свойства **requestType** составляет `UserAdd` . Свойство **accessPackageAssignment** содержит свойство `targetId` с `id` пользователями. Свойство **assignmentPolicyId** определяет [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md) Свойство **accessPackageId** определяет [accessPackage.](../resources/accesspackage.md) Пользователь, делая запрос, должен уже существовать в каталоге.

Чтобы пользователь, не вступив в администратор, запрашивал расширение своих назначений, значение свойства **requestType** `UserExtend` составляет . Свойство **accessPackageAssignment** содержит свойство `targetId` с `id` пользователями. Свойство **assignmentPolicyId** определяет [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md) Свойство **accessPackageId** определяет [accessPackage.](../resources/accesspackage.md) Пользователь, делая запрос, должен уже существовать в каталоге.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа из 200 серий и новый объект [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.  

Если это запрос, то впоследствии создается `AdminAdd` [accessPackageAssignment](../resources/accesspackageassignment.md) и, при необходимости, [accessPackageSubject.](../resources/accesspackagesubject.md) Вы можете найти тех, кто использует параметры запроса при [перечислении accessPackageAssignments](accesspackageassignment-list.md).

## <a name="examples"></a>Примеры
### <a name="example-1-admin-requests-a-direct-assignment-for-a-user"></a>Пример 1. Администратор запрашивает прямое назначение для пользователя
#### <a name="request"></a>Запрос

Ниже приводится пример запроса на прямое назначение, в котором администратор запрашивает создание назначения для пользователя. Так как [accessPackageSubject](../resources/accesspackagesubject.md) может еще не существовать, значение **targetID** — это объектный ID назначенного пользователя, значение **accessPackageId** — это желаемый пакет доступа для этого пользователя, а значение **assignmentPolicyId** — это политика прямого назначения в этом пакете доступа.
 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_1"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

### <a name="example-2-user-requests-a-package-and-answers-questions-for-approval"></a>Пример 2. Пользователь запрашивает пакет и отвечает на вопросы для утверждения
#### <a name="request"></a>Запрос

Ниже приводится пример запроса, в котором запросчик предоставил ответы на вопросы, чтобы помочь ему принять решение.
 



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_2"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "UserAdd",
    "accessPackageAssignment": {
        "targetId": "46184453-e63b-4f20-86c2-c557ed5d5df9",
        "assignmentPolicyId": "2264bf65-76ba-417b-a27d-54d291f0cbc8",
        "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA"
        }
    }]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e382d02-4454-436b-b700-59c7dd77f466",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF",
            "isRequired": false,
            "text": {
                "defaultText": "what state are you from?",
                "localizedTexts": [{
                    "text": "¿De qué estado eres?",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
            "choices": [{
                "actualValue": "AZ",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Arizona",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "CA",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "California",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "OH",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Ohio",
                        "languageCode": "es"
                    }]
                }
            }],
            "allowsMultipleSelection": false
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA",
            "isRequired": false,
            "text": {
                "defaultText": "Who is your manager?",
                "localizedTexts": [{
                    "text": "por qué necesita acceso a este paquete",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": false
        }
    }]
}
```
### <a name="example-3-request-a-package-and-provide-a-justification"></a>Пример 3. Запрос пакета и обоснование
#### <a name="request"></a>Запрос

В следующем примере показано, как запросить пакет доступа и предоставить обоснование для утвержденного.
 


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "UserAdd",
    "accessPackageAssignment": {
        "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    "justification":"Need access to New Hire access package"
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "813bbc6b-31f5-4cdf-8fed-1ba4284a1e3f",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": "Requested for the new task.",
    "answers": [],
    "schedule": {
        "startDateTime": null,
        "recurrence": null,
        "expiration": {
            "endDateTime": null,
            "duration": null,
            "type": null
        }
    }
}
```

### <a name="example-4-remove-an-assignment"></a>Пример 4. Удаление назначения

Чтобы удалить назначения, создайте новый объект accessPackageAssignmentRequest со следующими настройками:

+ Значение свойства **requestType,** установленного для `AdminRemove` .
+ В свойство accessPackageAssignment включите список с идентификатором объектов accessPackageAssignment для удаления.

#### <a name="request"></a>Запрос

В следующем примере показано, как удалить назначение.


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "AdminRemove",
    "accessPackageAssignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
    }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",

    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


