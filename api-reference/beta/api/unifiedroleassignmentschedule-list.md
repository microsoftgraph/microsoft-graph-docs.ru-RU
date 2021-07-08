---
title: Список unifiedRoleAssignmentSchedules
description: Получите список объектов unifiedRoleAssignmentSchedule и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 26c52cfa2d305f23783c384deb1f2cd09c289db6
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334481"
---
# <a name="list-unifiedroleassignmentschedules"></a><span data-ttu-id="6ffdc-103">Список unifiedRoleAssignmentSchedules</span><span class="sxs-lookup"><span data-stu-id="6ffdc-103">List unifiedRoleAssignmentSchedules</span></span>
<span data-ttu-id="6ffdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ffdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ffdc-105">Получите список объектов [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="6ffdc-105">Get a list of the [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ffdc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ffdc-106">Permissions</span></span>
<span data-ttu-id="6ffdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ffdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ffdc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ffdc-109">Permission type</span></span>|<span data-ttu-id="6ffdc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ffdc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ffdc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ffdc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ffdc-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6ffdc-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span></span>   |
|<span data-ttu-id="6ffdc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ffdc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ffdc-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6ffdc-114">Not supported</span></span>|
|<span data-ttu-id="6ffdc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6ffdc-115">Application</span></span>|<span data-ttu-id="6ffdc-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6ffdc-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ffdc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ffdc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ffdc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ffdc-118">Optional query parameters</span></span>
<span data-ttu-id="6ffdc-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="6ffdc-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6ffdc-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6ffdc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ffdc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ffdc-121">Request headers</span></span>
|<span data-ttu-id="6ffdc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6ffdc-122">Name</span></span>|<span data-ttu-id="6ffdc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6ffdc-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6ffdc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ffdc-124">Authorization</span></span>|<span data-ttu-id="6ffdc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ffdc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ffdc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ffdc-127">Request body</span></span>
<span data-ttu-id="6ffdc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ffdc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ffdc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffdc-129">Response</span></span>

<span data-ttu-id="6ffdc-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6ffdc-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ffdc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ffdc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ffdc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ffdc-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6ffdc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ffdc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules
```
# <a name="c"></a>[<span data-ttu-id="6ffdc-134">C#</span><span class="sxs-lookup"><span data-stu-id="6ffdc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ffdc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ffdc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ffdc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ffdc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ffdc-137">Java</span><span class="sxs-lookup"><span data-stu-id="6ffdc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6ffdc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffdc-138">Response</span></span>
<span data-ttu-id="6ffdc-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ffdc-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentSchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "createdUsing": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "createdDateTime": "2020-09-09T21:35:27.91Z",
      "modifiedDateTime": "2020-09-09T21:35:27.91Z",
      "status": "Provsioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "assignmentType": "eligible",
      "memberType": "direct"
    }
  ]
}
```

