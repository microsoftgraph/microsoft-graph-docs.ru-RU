---
title: Get unifiedRoleEligibilitySchedule
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleEligibilitySchedule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 749d8df40fbc5aa92af9f4b33fe8502863139d0d
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334523"
---
# <a name="get-unifiedroleeligibilityschedule"></a>Get unifiedRoleEligibilitySchedule
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilitySchedule.](../resources/unifiedroleeligibilityschedule.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules/{unifiedRoleEligibilitySchedulesId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules/5cfd7709-7709-5cfd-0977-fd5c0977fd5c
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleeligibilityschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleeligibilityschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleeligibilityschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleeligibilityschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilitySchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "createdUsing": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "createdDateTime": "2020-09-09T21:35:27.91Z",
    "modifiedDateTime": "2020-09-09T21:35:27.91Z",
    "status": "Provisioned",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "memberType": "direct"
  }
}
```

