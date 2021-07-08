---
title: Список unifiedRoleAssignmentScheduleInstances
description: Получите список объектов unifiedRoleAssignmentScheduleInstance и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 382c5a7ff8b75da06f1d75b06a2bb382137c275d
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334390"
---
# <a name="list-unifiedroleassignmentscheduleinstances"></a><span data-ttu-id="4ed4e-103">Список unifiedRoleAssignmentScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="4ed4e-103">List unifiedRoleAssignmentScheduleInstances</span></span>
<span data-ttu-id="4ed4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ed4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ed4e-105">Получите список объектов [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="4ed4e-105">Get a list of the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ed4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ed4e-106">Permissions</span></span>
<span data-ttu-id="4ed4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ed4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ed4e-109">Permission type</span></span>|<span data-ttu-id="4ed4e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ed4e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ed4e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ed4e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ed4e-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="4ed4e-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="4ed4e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ed4e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ed4e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4ed4e-114">Not supported</span></span>|
|<span data-ttu-id="4ed4e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4ed4e-115">Application</span></span>|<span data-ttu-id="4ed4e-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="4ed4e-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ed4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ed4e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ed4e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ed4e-118">Optional query parameters</span></span>
<span data-ttu-id="4ed4e-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="4ed4e-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4ed4e-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4ed4e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ed4e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ed4e-121">Request headers</span></span>
|<span data-ttu-id="4ed4e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4ed4e-122">Name</span></span>|<span data-ttu-id="4ed4e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4ed4e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ed4e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ed4e-124">Authorization</span></span>|<span data-ttu-id="4ed4e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ed4e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ed4e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ed4e-127">Request body</span></span>
<span data-ttu-id="4ed4e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ed4e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ed4e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ed4e-129">Response</span></span>

<span data-ttu-id="4ed4e-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4ed4e-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ed4e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4ed4e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ed4e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ed4e-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4ed4e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ed4e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances
```
# <a name="c"></a>[<span data-ttu-id="4ed4e-134">C#</span><span class="sxs-lookup"><span data-stu-id="4ed4e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ed4e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ed4e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ed4e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ed4e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ed4e-137">Java</span><span class="sxs-lookup"><span data-stu-id="4ed4e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4ed4e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ed4e-138">Response</span></span>
<span data-ttu-id="4ed4e-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4ed4e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "principalId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "roleDefinitionId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "directoryScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "appScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "assignmentType": "eligible",
      "memberType": "direct",
      "roleAssignmentOriginId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "roleAssignmentScheduleId": "eb18c026-c026-eb18-26c0-18eb26c018eb"
    }
  ]
}
```

