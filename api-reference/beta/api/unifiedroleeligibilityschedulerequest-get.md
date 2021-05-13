---
title: Get unifiedRoleEligibilityScheduleRequest
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72279405e77700847b7c885e6bf77b7893377715
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475286"
---
# <a name="get-unifiedroleeligibilityschedulerequest"></a><span data-ttu-id="769c0-103">Get unifiedRoleEligibilityScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="769c0-103">Get unifiedRoleEligibilityScheduleRequest</span></span>
<span data-ttu-id="769c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="769c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="769c0-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="769c0-105">Read the properties and relationships of an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="769c0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="769c0-106">Permissions</span></span>
<span data-ttu-id="769c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="769c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="769c0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="769c0-109">Permission type</span></span>|<span data-ttu-id="769c0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="769c0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="769c0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="769c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="769c0-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="769c0-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="769c0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="769c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="769c0-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="769c0-114">Not supported</span></span>|
|<span data-ttu-id="769c0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="769c0-115">Application</span></span>|<span data-ttu-id="769c0-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="769c0-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="769c0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="769c0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="769c0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="769c0-118">Optional query parameters</span></span>
<span data-ttu-id="769c0-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="769c0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="769c0-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="769c0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="769c0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="769c0-121">Request headers</span></span>
|<span data-ttu-id="769c0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="769c0-122">Name</span></span>|<span data-ttu-id="769c0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="769c0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="769c0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="769c0-124">Authorization</span></span>|<span data-ttu-id="769c0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="769c0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="769c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="769c0-127">Request body</span></span>
<span data-ttu-id="769c0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="769c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="769c0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="769c0-129">Response</span></span>

<span data-ttu-id="769c0-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="769c0-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="769c0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="769c0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="769c0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="769c0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="769c0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="769c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```
# <a name="c"></a>[<span data-ttu-id="769c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="769c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleeligibilityschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="769c0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="769c0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleeligibilityschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="769c0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="769c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleeligibilityschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="769c0-137">Java</span><span class="sxs-lookup"><span data-stu-id="769c0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleeligibilityschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="769c0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="769c0-138">Response</span></span>
<span data-ttu-id="769c0-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="769c0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

