---
title: 'unifiedRoleAssignmentScheduleRequest: отмена'
description: Отмена единой системыRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9a74d0b9d341074c3ad68eb1fdad7c77b2baa43
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334376"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a><span data-ttu-id="72038-103">unifiedRoleAssignmentScheduleRequest: отмена</span><span class="sxs-lookup"><span data-stu-id="72038-103">unifiedRoleAssignmentScheduleRequest: cancel</span></span>
<span data-ttu-id="72038-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72038-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72038-105">Немедленно [отмените унифицированныйRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и задайте системе автоматическое удаление отмененного запроса через 30 дней.</span><span class="sxs-lookup"><span data-stu-id="72038-105">Immediately cancel a [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="72038-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72038-106">Permissions</span></span>
<span data-ttu-id="72038-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72038-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72038-109">Permission type</span></span>|<span data-ttu-id="72038-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72038-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72038-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72038-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72038-112">RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="72038-112">RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="72038-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72038-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72038-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="72038-114">Not supported</span></span>|
|<span data-ttu-id="72038-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="72038-115">Application</span></span>|<span data-ttu-id="72038-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="72038-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="72038-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72038-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="72038-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72038-118">Request headers</span></span>
|<span data-ttu-id="72038-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72038-119">Name</span></span>|<span data-ttu-id="72038-120">Описание</span><span class="sxs-lookup"><span data-stu-id="72038-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="72038-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72038-121">Authorization</span></span>|<span data-ttu-id="72038-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72038-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72038-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72038-124">Request body</span></span>
<span data-ttu-id="72038-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72038-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72038-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="72038-126">Response</span></span>

<span data-ttu-id="72038-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="72038-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="72038-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="72038-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72038-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="72038-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="72038-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="72038-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="72038-131">C#</span><span class="sxs-lookup"><span data-stu-id="72038-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleassignmentschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72038-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72038-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleassignmentschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72038-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72038-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleassignmentschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72038-134">Java</span><span class="sxs-lookup"><span data-stu-id="72038-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleassignmentschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="72038-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="72038-135">Response</span></span>
<span data-ttu-id="72038-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72038-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

