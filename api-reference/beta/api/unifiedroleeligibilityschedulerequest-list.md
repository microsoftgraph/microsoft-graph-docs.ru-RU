---
title: Список унифицированныхRoleEligibilityScheduleRequests
description: Получите список объектов unifiedRoleEligibilityScheduleRequest и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b9564d4ee163a3d53e9233e0d7b690cb2337326f
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680128"
---
# <a name="list-unifiedroleeligibilityschedulerequests"></a><span data-ttu-id="e68ed-103">Список унифицированныхRoleEligibilityScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="e68ed-103">List unifiedRoleEligibilityScheduleRequests</span></span>
<span data-ttu-id="e68ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e68ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e68ed-105">Получите список объектов [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="e68ed-105">Get a list of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e68ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e68ed-106">Permissions</span></span>
<span data-ttu-id="e68ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e68ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e68ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e68ed-109">Permission type</span></span>|<span data-ttu-id="e68ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e68ed-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e68ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e68ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e68ed-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e68ed-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="e68ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e68ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e68ed-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e68ed-114">Not supported</span></span>|
|<span data-ttu-id="e68ed-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e68ed-115">Application</span></span>|<span data-ttu-id="e68ed-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e68ed-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="e68ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e68ed-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e68ed-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e68ed-118">Optional query parameters</span></span>
<span data-ttu-id="e68ed-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e68ed-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e68ed-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e68ed-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e68ed-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e68ed-121">Request headers</span></span>
|<span data-ttu-id="e68ed-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e68ed-122">Name</span></span>|<span data-ttu-id="e68ed-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e68ed-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e68ed-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e68ed-124">Authorization</span></span>|<span data-ttu-id="e68ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e68ed-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e68ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e68ed-127">Request body</span></span>
<span data-ttu-id="e68ed-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e68ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e68ed-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e68ed-129">Response</span></span>

<span data-ttu-id="e68ed-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e68ed-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e68ed-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e68ed-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e68ed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e68ed-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e68ed-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e68ed-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
```
# <a name="c"></a>[<span data-ttu-id="e68ed-134">C#</span><span class="sxs-lookup"><span data-stu-id="e68ed-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleeligibilityschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e68ed-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e68ed-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleeligibilityschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e68ed-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e68ed-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleeligibilityschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e68ed-137">Java</span><span class="sxs-lookup"><span data-stu-id="e68ed-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleeligibilityschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e68ed-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e68ed-138">Response</span></span>
<span data-ttu-id="e68ed-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e68ed-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

