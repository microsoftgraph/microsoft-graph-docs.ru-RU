---
title: 'unifiedRoleAssignmentScheduleRequest: отмена'
description: Отмена единой системыRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: db696f4a7841557f743d2cea807f273b5d538230
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680453"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a><span data-ttu-id="8c319-103">unifiedRoleAssignmentScheduleRequest: отмена</span><span class="sxs-lookup"><span data-stu-id="8c319-103">unifiedRoleAssignmentScheduleRequest: cancel</span></span>
<span data-ttu-id="8c319-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c319-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c319-105">Немедленно [отмените унифицированныйRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и задайте системе автоматическое удаление отмененного запроса через 30 дней.</span><span class="sxs-lookup"><span data-stu-id="8c319-105">Immediately cancel a [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c319-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c319-106">Permissions</span></span>
<span data-ttu-id="8c319-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c319-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c319-109">Permission type</span></span>|<span data-ttu-id="8c319-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c319-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c319-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c319-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c319-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="8c319-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="8c319-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c319-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c319-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8c319-114">Not supported</span></span>|
|<span data-ttu-id="8c319-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c319-115">Application</span></span>|<span data-ttu-id="8c319-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8c319-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c319-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c319-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="8c319-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c319-118">Request headers</span></span>
|<span data-ttu-id="8c319-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8c319-119">Name</span></span>|<span data-ttu-id="8c319-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8c319-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c319-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c319-121">Authorization</span></span>|<span data-ttu-id="8c319-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c319-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c319-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c319-124">Request body</span></span>
<span data-ttu-id="8c319-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c319-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c319-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c319-126">Response</span></span>

<span data-ttu-id="8c319-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8c319-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8c319-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c319-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c319-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c319-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c319-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c319-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="8c319-131">C#</span><span class="sxs-lookup"><span data-stu-id="8c319-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleassignmentschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c319-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c319-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleassignmentschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c319-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c319-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleassignmentschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c319-134">Java</span><span class="sxs-lookup"><span data-stu-id="8c319-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleassignmentschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8c319-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c319-135">Response</span></span>
<span data-ttu-id="8c319-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c319-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

