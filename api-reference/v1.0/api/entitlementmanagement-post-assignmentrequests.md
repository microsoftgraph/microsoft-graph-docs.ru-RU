---
title: Создание accessPackageAssignmentRequest
description: Создание нового accessPackageAssignmentRequest.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 827020fd3da1c4b52dd95f67bb0550fbfcb9253a
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607899"
---
# <a name="create-accesspackageassignmentrequest"></a>Создание accessPackageAssignmentRequest

Пространство имен: microsoft.graph


В [Azure AD Entitlement Management](../resources/entitlementmanagement-overview.md) создайте новый [объект accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .  Эта операция используется для назначения пользователя пакету доступа или удаления назначения пакета доступа.


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/assignmentRequests
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .

Для администратора, запрашиваемого для создания назначения для пользователя, значение свойства **requestType** `AdminAdd`—  и `targetId` свойство назначения содержит назначенного пользователя, свойство **assignmentPolicyId**, определяющий accessPackageAssignmentPolicy, и **свойство accessPackageId**, определяющие [accessPackpackage](../resources/accesspackage.md).

Для администратора, запрашиваемого для удаления назначения, значение свойства **requestType** `AdminRemove`составляет , а свойство назначения содержит  свойство **id**, определяющий [удаляется accessPackageAssignment](../resources/accesspackageassignment.md).

Чтобы пользователь, не вступив в администратор, попросил создать свое собственное назначение для первого назначения или возобновления назначения, значение свойства **requestType** составляет `UserAdd`. Свойство **назначения** содержит объект с `targetId` пользователем `id` . Свойство **assignmentPolicyId** определяет accessPackageAssignmentPolicy. Свойство **accessPackageId** определяет [accessPackage](../resources/accesspackage.md). Пользователь, делая запрос, должен уже существовать в каталоге.

Чтобы пользователь, не вступив в администратор, запрашивал расширение своих назначений, значение свойства **requestType** составляет `UserExtend`. Свойство **назначения** содержит свойство `targetId` с `id` пользователями. Свойство **assignmentPolicyId** определяет accessPackageAssignmentPolicy. Свойство **accessPackageId** определяет [accessPackage](../resources/accesspackage.md). Пользователь, делая запрос, должен уже существовать в каталоге.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа из 200 серий и новый объект [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.

Если это запрос `AdminAdd` , то впоследствии создается [accessPackageAssignment](../resources/accesspackageassignment.md) и, при необходимости, [accessPackageSubject](../resources/accesspackagesubject.md) . Вы можете найти тех, кто использует параметры запроса при перечислении [accessPackageAssignments](entitlementmanagement-list-assignments.md).

## <a name="examples"></a>Примеры

### <a name="example-1-admin-requests-a-direct-assignment-for-a-user-already-in-the-directory"></a>Пример 1. Администратор запрашивает прямое назначение для пользователя уже в каталоге
#### <a name="request"></a>Запрос

Ниже приводится пример запроса на прямое назначение, в котором администратор запрашивает создание назначения для пользователя. Так как [accessPackageSubject](../resources/accesspackagesubject.md) может еще не существовать, значение **targetID** — это объектный ID назначенного пользователя, значение **accessPackageId** — это желаемый пакет доступа для этого пользователя, а значение **assignmentPolicyId** — это политика прямого назначения в этом пакете доступа.


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "assignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```

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
  "requestStatus": "Accepted"
}
```

### <a name="example-2-remove-an-assignment"></a>Пример 2. Удаление назначения

Чтобы удалить назначения, создайте новый объект accessPackageAssignmentRequest со следующими настройками:

+ Значение свойства **requestType** , установленного для `AdminRemove`.
+ В свойство назначения включите объект с идентификатором объекта accessPackageAssignment для удаления.

#### <a name="request"></a>Запрос

В следующем примере показано, как удалить назначение.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests
Content-type: application/json

{
    "requestType": "AdminRemove",
    "assignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#accessPackageAssignmentRequests/$entity",

    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted"
}
```

