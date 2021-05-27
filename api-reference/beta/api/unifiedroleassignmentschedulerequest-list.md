---
title: Список unifiedRoleAssignmentScheduleRequests
description: Получите список объектов unifiedRoleAssignmentScheduleRequest и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: eb84749f882244d7aa3d85f5768a0bf487fed3b6
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680443"
---
# <a name="list-unifiedroleassignmentschedulerequests"></a><span data-ttu-id="a5fc2-103">Список unifiedRoleAssignmentScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="a5fc2-103">List unifiedRoleAssignmentScheduleRequests</span></span>

<span data-ttu-id="a5fc2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5fc2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5fc2-105">Получите список объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="a5fc2-105">Get a list of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5fc2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5fc2-106">Permissions</span></span>

<span data-ttu-id="a5fc2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5fc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5fc2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5fc2-109">Permission type</span></span>                        | <span data-ttu-id="a5fc2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5fc2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a5fc2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5fc2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5fc2-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a5fc2-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>          |
| <span data-ttu-id="a5fc2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5fc2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5fc2-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a5fc2-114">Not supported</span></span>                               |
| <span data-ttu-id="a5fc2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a5fc2-115">Application</span></span>                            | <span data-ttu-id="a5fc2-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a5fc2-116">PrivilegedAccess.Read.AzureAD</span></span>               |

## <a name="http-request"></a><span data-ttu-id="a5fc2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5fc2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5fc2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5fc2-118">Optional query parameters</span></span>

<span data-ttu-id="a5fc2-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a5fc2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a5fc2-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a5fc2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5fc2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5fc2-121">Request headers</span></span>

| <span data-ttu-id="a5fc2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a5fc2-122">Name</span></span>          | <span data-ttu-id="a5fc2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a5fc2-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a5fc2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5fc2-124">Authorization</span></span> | <span data-ttu-id="a5fc2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5fc2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5fc2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5fc2-127">Request body</span></span>

<span data-ttu-id="a5fc2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5fc2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5fc2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5fc2-129">Response</span></span>

<span data-ttu-id="a5fc2-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5fc2-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5fc2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5fc2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5fc2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5fc2-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a5fc2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5fc2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedulerequest"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests
```
# <a name="c"></a>[<span data-ttu-id="a5fc2-134">C#</span><span class="sxs-lookup"><span data-stu-id="a5fc2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5fc2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5fc2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5fc2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5fc2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5fc2-137">Java</span><span class="sxs-lookup"><span data-stu-id="a5fc2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5fc2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5fc2-138">Response</span></span>

<span data-ttu-id="a5fc2-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5fc2-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```
