---
title: Список унифицированныхRoleEligibilityScheduleRequests
description: Получите список объектов unifiedRoleEligibilityScheduleRequest и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: eaee624680315655f7e2326338ef684043c392f8
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334663"
---
# <a name="list-unifiedroleeligibilityschedulerequests"></a><span data-ttu-id="a1012-103">Список унифицированныхRoleEligibilityScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="a1012-103">List unifiedRoleEligibilityScheduleRequests</span></span>
<span data-ttu-id="a1012-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1012-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1012-105">Получите список объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="a1012-105">Get a list of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1012-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1012-106">Permissions</span></span>
<span data-ttu-id="a1012-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1012-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1012-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1012-109">Permission type</span></span>|<span data-ttu-id="a1012-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1012-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1012-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1012-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1012-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a1012-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span> |
|<span data-ttu-id="a1012-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1012-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1012-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a1012-114">Not supported</span></span>|
|<span data-ttu-id="a1012-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a1012-115">Application</span></span>|<span data-ttu-id="a1012-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="a1012-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1012-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1012-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1012-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1012-118">Optional query parameters</span></span>
<span data-ttu-id="a1012-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a1012-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a1012-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a1012-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1012-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1012-121">Request headers</span></span>
|<span data-ttu-id="a1012-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a1012-122">Name</span></span>|<span data-ttu-id="a1012-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a1012-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a1012-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1012-124">Authorization</span></span>|<span data-ttu-id="a1012-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1012-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1012-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1012-127">Request body</span></span>
<span data-ttu-id="a1012-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1012-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1012-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1012-129">Response</span></span>

<span data-ttu-id="a1012-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a1012-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1012-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a1012-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1012-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1012-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a1012-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1012-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
```
# <a name="c"></a>[<span data-ttu-id="a1012-134">C#</span><span class="sxs-lookup"><span data-stu-id="a1012-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleeligibilityschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1012-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1012-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleeligibilityschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1012-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1012-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleeligibilityschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1012-137">Java</span><span class="sxs-lookup"><span data-stu-id="a1012-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleeligibilityschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a1012-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1012-138">Response</span></span>
<span data-ttu-id="a1012-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a1012-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "a2e242a0-42a0-a2e2-a042-e2a2a042e2a2",
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
  ]
}
```

