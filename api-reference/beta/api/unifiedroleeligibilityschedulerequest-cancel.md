---
title: 'unifiedRoleEligibilityScheduleRequest: отмена'
description: Отмена единойRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c877c30ed016a83a9c1da8019a33467e232fc110
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680103"
---
# <a name="unifiedroleeligibilityschedulerequest-cancel"></a><span data-ttu-id="dda45-103">unifiedRoleEligibilityScheduleRequest: отмена</span><span class="sxs-lookup"><span data-stu-id="dda45-103">unifiedRoleEligibilityScheduleRequest: cancel</span></span>
<span data-ttu-id="dda45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dda45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dda45-105">Немедленно отмените [унифицированныйRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) и заключите автоматическое удаление отмененного запроса через 30 дней.</span><span class="sxs-lookup"><span data-stu-id="dda45-105">Immediately cancel a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="dda45-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dda45-106">Permissions</span></span>
<span data-ttu-id="dda45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dda45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dda45-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dda45-109">Permission type</span></span>|<span data-ttu-id="dda45-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dda45-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dda45-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dda45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dda45-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="dda45-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="dda45-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dda45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dda45-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dda45-114">Not supported</span></span>|
|<span data-ttu-id="dda45-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="dda45-115">Application</span></span>|<span data-ttu-id="dda45-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dda45-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="dda45-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dda45-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="dda45-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dda45-118">Request headers</span></span>
|<span data-ttu-id="dda45-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dda45-119">Name</span></span>|<span data-ttu-id="dda45-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dda45-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dda45-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dda45-121">Authorization</span></span>|<span data-ttu-id="dda45-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dda45-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dda45-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dda45-124">Request body</span></span>
<span data-ttu-id="dda45-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dda45-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dda45-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="dda45-126">Response</span></span>

<span data-ttu-id="dda45-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dda45-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dda45-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="dda45-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dda45-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="dda45-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dda45-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dda45-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="dda45-131">C#</span><span class="sxs-lookup"><span data-stu-id="dda45-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dda45-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dda45-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dda45-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dda45-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dda45-134">Java</span><span class="sxs-lookup"><span data-stu-id="dda45-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dda45-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dda45-135">Response</span></span>
<span data-ttu-id="dda45-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dda45-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

