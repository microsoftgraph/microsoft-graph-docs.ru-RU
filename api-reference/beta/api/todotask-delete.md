---
title: Delete todoTask
description: Удаляет объект todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9f0642a6a8c41f56d1fe8c8a5497d71393c1cad1
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873915"
---
# <a name="delete-todotask"></a><span data-ttu-id="026f3-103">Delete todoTask</span><span class="sxs-lookup"><span data-stu-id="026f3-103">Delete todoTask</span></span>
<span data-ttu-id="026f3-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="026f3-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="026f3-105">Удаляет объект [todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="026f3-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="026f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="026f3-106">Permissions</span></span>
<span data-ttu-id="026f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="026f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="026f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="026f3-109">Permission type</span></span>|<span data-ttu-id="026f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="026f3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="026f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="026f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="026f3-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="026f3-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="026f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="026f3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="026f3-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="026f3-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="026f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="026f3-115">Application</span></span>|<span data-ttu-id="026f3-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="026f3-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="026f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="026f3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="026f3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="026f3-118">Request headers</span></span>
|<span data-ttu-id="026f3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="026f3-119">Name</span></span>|<span data-ttu-id="026f3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="026f3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="026f3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="026f3-121">Authorization</span></span>|<span data-ttu-id="026f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="026f3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="026f3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="026f3-124">Request body</span></span>
<span data-ttu-id="026f3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="026f3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="026f3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="026f3-126">Response</span></span>

<span data-ttu-id="026f3-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="026f3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="026f3-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="026f3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="026f3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="026f3-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="026f3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="026f3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="026f3-131">C#</span><span class="sxs-lookup"><span data-stu-id="026f3-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="026f3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="026f3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="026f3-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="026f3-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="026f3-134">Java</span><span class="sxs-lookup"><span data-stu-id="026f3-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="026f3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="026f3-135">Response</span></span>
<span data-ttu-id="026f3-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="026f3-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



