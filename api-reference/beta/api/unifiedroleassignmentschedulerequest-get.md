---
title: Get unifiedRoleAssignmentScheduleRequest
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e7b33eea1551bcf0d5bd661cc4f097e8f0e01a82
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334411"
---
# <a name="get-unifiedroleassignmentschedulerequest"></a><span data-ttu-id="45834-103">Get unifiedRoleAssignmentScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="45834-103">Get unifiedRoleAssignmentScheduleRequest</span></span>
<span data-ttu-id="45834-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45834-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45834-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="45834-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45834-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45834-106">Permissions</span></span>
<span data-ttu-id="45834-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45834-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45834-109">Permission type</span></span>|<span data-ttu-id="45834-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45834-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45834-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45834-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45834-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="45834-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="45834-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45834-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45834-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="45834-114">Not supported</span></span>|
|<span data-ttu-id="45834-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="45834-115">Application</span></span>|<span data-ttu-id="45834-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="45834-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="45834-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45834-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45834-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45834-118">Optional query parameters</span></span>
<span data-ttu-id="45834-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="45834-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="45834-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="45834-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="45834-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45834-121">Request headers</span></span>
|<span data-ttu-id="45834-122">Имя</span><span class="sxs-lookup"><span data-stu-id="45834-122">Name</span></span>|<span data-ttu-id="45834-123">Описание</span><span class="sxs-lookup"><span data-stu-id="45834-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="45834-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45834-124">Authorization</span></span>|<span data-ttu-id="45834-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45834-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45834-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45834-127">Request body</span></span>
<span data-ttu-id="45834-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45834-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45834-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="45834-129">Response</span></span>

<span data-ttu-id="45834-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="45834-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45834-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="45834-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45834-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="45834-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="45834-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="45834-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```
# <a name="c"></a>[<span data-ttu-id="45834-134">C#</span><span class="sxs-lookup"><span data-stu-id="45834-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45834-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45834-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45834-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45834-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45834-137">Java</span><span class="sxs-lookup"><span data-stu-id="45834-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="45834-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="45834-138">Response</span></span>
<span data-ttu-id="45834-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="45834-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
    "action": "String",
    "principalId": "String",
    "roleDefinitionId": "String",
    "directoryScopeId": "String",
    "appScopeId": "String",
    "isValidationOnly": "Boolean",
    "targetScheduleId": "String",
    "justification": "String",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "ticketInfo": {
      "@odata.type": "microsoft.graph.ticketInfo"
    }
  }
}
```

