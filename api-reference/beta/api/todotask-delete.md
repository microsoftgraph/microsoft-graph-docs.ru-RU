---
title: Удаление Тодотаск
description: Удаляет объект Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5cb89bc7e21ca777f36ca846e186f741b7b5667
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873360"
---
# <a name="delete-todotask"></a><span data-ttu-id="12d96-103">Удаление Тодотаск</span><span class="sxs-lookup"><span data-stu-id="12d96-103">Delete todoTask</span></span>
<span data-ttu-id="12d96-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="12d96-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="12d96-105">Удаляет объект [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="12d96-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="12d96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12d96-106">Permissions</span></span>
<span data-ttu-id="12d96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12d96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12d96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12d96-109">Permission type</span></span>|<span data-ttu-id="12d96-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12d96-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12d96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12d96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12d96-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12d96-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="12d96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12d96-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12d96-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12d96-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="12d96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12d96-115">Application</span></span>|<span data-ttu-id="12d96-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12d96-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="12d96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12d96-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="12d96-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12d96-118">Request headers</span></span>
|<span data-ttu-id="12d96-119">Имя</span><span class="sxs-lookup"><span data-stu-id="12d96-119">Name</span></span>|<span data-ttu-id="12d96-120">Описание</span><span class="sxs-lookup"><span data-stu-id="12d96-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="12d96-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12d96-121">Authorization</span></span>|<span data-ttu-id="12d96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12d96-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12d96-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12d96-124">Request body</span></span>
<span data-ttu-id="12d96-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12d96-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12d96-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="12d96-126">Response</span></span>

<span data-ttu-id="12d96-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="12d96-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="12d96-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="12d96-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12d96-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="12d96-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="12d96-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="12d96-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="12d96-131">C#</span><span class="sxs-lookup"><span data-stu-id="12d96-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12d96-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12d96-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12d96-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12d96-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="12d96-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="12d96-134">Response</span></span>
<span data-ttu-id="12d96-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="12d96-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

