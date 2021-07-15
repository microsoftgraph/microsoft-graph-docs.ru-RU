---
title: Get unifiedRoleAssignmentSchedule
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleAssignmentSchedule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9efffbff7bab2c7bf012c6d6fc7dbc77e923688f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440257"
---
# <a name="get-unifiedroleassignmentschedule"></a><span data-ttu-id="a7c38-103">Get unifiedRoleAssignmentSchedule</span><span class="sxs-lookup"><span data-stu-id="a7c38-103">Get unifiedRoleAssignmentSchedule</span></span>
<span data-ttu-id="a7c38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7c38-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleAssignmentSchedule.](../resources/unifiedroleassignmentschedule.md)</span><span class="sxs-lookup"><span data-stu-id="a7c38-105">Read the properties and relationships of an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7c38-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7c38-106">Permissions</span></span>
<span data-ttu-id="a7c38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7c38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c38-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7c38-109">Permission type</span></span>|<span data-ttu-id="a7c38-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7c38-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7c38-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7c38-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7c38-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a7c38-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span></span>|
|<span data-ttu-id="a7c38-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7c38-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7c38-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a7c38-114">Not supported</span></span>|
|<span data-ttu-id="a7c38-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a7c38-115">Application</span></span>|<span data-ttu-id="a7c38-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a7c38-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7c38-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7c38-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/{unifiedRoleAssignmentSchedulesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7c38-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a7c38-118">Optional query parameters</span></span>
<span data-ttu-id="a7c38-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="a7c38-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a7c38-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a7c38-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7c38-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7c38-121">Request headers</span></span>
|<span data-ttu-id="a7c38-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a7c38-122">Name</span></span>|<span data-ttu-id="a7c38-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a7c38-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a7c38-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7c38-124">Authorization</span></span>|<span data-ttu-id="a7c38-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7c38-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7c38-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7c38-127">Request body</span></span>
<span data-ttu-id="a7c38-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7c38-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7c38-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7c38-129">Response</span></span>

<span data-ttu-id="a7c38-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7c38-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a7c38-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a7c38-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7c38-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7c38-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a7c38-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7c38-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413
```
# <a name="c"></a>[<span data-ttu-id="a7c38-134">C#</span><span class="sxs-lookup"><span data-stu-id="a7c38-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7c38-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7c38-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7c38-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7c38-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7c38-137">Java</span><span class="sxs-lookup"><span data-stu-id="a7c38-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a7c38-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7c38-138">Response</span></span>
<span data-ttu-id="a7c38-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a7c38-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "createdUsing": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "createdDateTime": "2020-09-09T21:35:27.91Z",
    "modifiedDateTime": "2020-09-09T21:35:27.91Z",
    "status": "Provisioned",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "assignmentType": "Eligible",
    "memberType": "direct"
  }
}
```

