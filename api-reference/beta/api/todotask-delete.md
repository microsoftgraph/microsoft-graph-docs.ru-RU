---
title: Удаление Тодотаск
description: Удаляет объект Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9e9391ccbd03f20d1b83fd7d015c9878b88c7e76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010467"
---
# <a name="delete-todotask"></a><span data-ttu-id="8a16a-103">Удаление Тодотаск</span><span class="sxs-lookup"><span data-stu-id="8a16a-103">Delete todoTask</span></span>
<span data-ttu-id="8a16a-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="8a16a-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="8a16a-105">Удаляет объект [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="8a16a-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a16a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a16a-106">Permissions</span></span>
<span data-ttu-id="8a16a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a16a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a16a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a16a-109">Permission type</span></span>|<span data-ttu-id="8a16a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a16a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a16a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a16a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8a16a-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a16a-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8a16a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a16a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a16a-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a16a-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="8a16a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a16a-115">Application</span></span>|<span data-ttu-id="8a16a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8a16a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a16a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a16a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="8a16a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a16a-118">Request headers</span></span>
|<span data-ttu-id="8a16a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8a16a-119">Name</span></span>|<span data-ttu-id="8a16a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8a16a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a16a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a16a-121">Authorization</span></span>|<span data-ttu-id="8a16a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a16a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a16a-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a16a-124">Request body</span></span>
<span data-ttu-id="8a16a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a16a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a16a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a16a-126">Response</span></span>

<span data-ttu-id="8a16a-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8a16a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8a16a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8a16a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8a16a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a16a-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8a16a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a16a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="8a16a-131">C#</span><span class="sxs-lookup"><span data-stu-id="8a16a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a16a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a16a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a16a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a16a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8a16a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a16a-134">Response</span></span>
<span data-ttu-id="8a16a-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8a16a-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



