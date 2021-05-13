---
title: 'unifiedRoleEligibilityScheduleRequest: отмена'
description: Отмена единойRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 325eb611042cf4627cb1a02f15fad8513ba70870
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474476"
---
# <a name="unifiedroleeligibilityschedulerequest-cancel"></a><span data-ttu-id="2213b-103">unifiedRoleEligibilityScheduleRequest: отмена</span><span class="sxs-lookup"><span data-stu-id="2213b-103">unifiedRoleEligibilityScheduleRequest: cancel</span></span>
<span data-ttu-id="2213b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2213b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2213b-105">Немедленно отмените [унифицированныйRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и заключите автоматическое удаление отмененного запроса через 30 дней.</span><span class="sxs-lookup"><span data-stu-id="2213b-105">Immediately cancel a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="2213b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2213b-106">Permissions</span></span>
<span data-ttu-id="2213b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2213b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2213b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2213b-109">Permission type</span></span>|<span data-ttu-id="2213b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2213b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2213b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2213b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2213b-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2213b-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="2213b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2213b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2213b-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2213b-114">Not supported</span></span>|
|<span data-ttu-id="2213b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2213b-115">Application</span></span>|<span data-ttu-id="2213b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2213b-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="2213b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2213b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="2213b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2213b-118">Request headers</span></span>
|<span data-ttu-id="2213b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2213b-119">Name</span></span>|<span data-ttu-id="2213b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2213b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2213b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2213b-121">Authorization</span></span>|<span data-ttu-id="2213b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2213b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2213b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2213b-124">Request body</span></span>
<span data-ttu-id="2213b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2213b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2213b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2213b-126">Response</span></span>

<span data-ttu-id="2213b-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2213b-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2213b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2213b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2213b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2213b-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2213b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2213b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="2213b-131">C#</span><span class="sxs-lookup"><span data-stu-id="2213b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2213b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2213b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2213b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2213b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2213b-134">Java</span><span class="sxs-lookup"><span data-stu-id="2213b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2213b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2213b-135">Response</span></span>
<span data-ttu-id="2213b-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2213b-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

