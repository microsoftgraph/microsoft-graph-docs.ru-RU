---
title: Создание accessPackageAssignmentRequest
description: Создание нового accessPackageAssignmentRequest.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 269045dd629974bfde3b060082657d28a6a36d75
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322666"
---
# <a name="create-accesspackageassignmentrequest"></a>Создание accessPackageAssignmentRequest

Пространство имен: microsoft.graph


В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)создайте новый объект [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Application                            | EntitlementManagement.ReadWrite.All |

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
| Authorization | Носитель \{токен\}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

Для администратора, запрашиваемого для удаления назначения, значение свойства **requestType** составляет , а свойство назначения содержит свойство `AdminRemove` **id,** определяющий [удаляется accessPackageAssignment.](../resources/accesspackageassignment.md) 

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа из 200 серий и новый объект [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-remove-an-assignment"></a>Пример 1. Удаление назначения

Чтобы удалить назначения, создайте новый объект accessPackageAssignmentRequest со следующими настройками:

+ Значение свойства **requestType,** установленного для `AdminRemove` .
+ В свойство назначения включите объект с идентификатором объекта accessPackageAssignment для удаления.

#### <a name="request"></a>Запрос

В следующем примере показано, как удалить назначение.

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

