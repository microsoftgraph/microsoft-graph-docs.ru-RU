---
title: Удаление Тодотаск
description: Удаляет объект Тодотаск.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b8e890bac27be2ba29e6c241af6faeb645e55f92
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904941"
---
# <a name="delete-todotask"></a><span data-ttu-id="39dc7-103">Удаление Тодотаск</span><span class="sxs-lookup"><span data-stu-id="39dc7-103">Delete todoTask</span></span>
<span data-ttu-id="39dc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39dc7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39dc7-105">Удаляет объект [тодотаск](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="39dc7-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39dc7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39dc7-106">Permissions</span></span>
<span data-ttu-id="39dc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39dc7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39dc7-109">Permission type</span></span>|<span data-ttu-id="39dc7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39dc7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39dc7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39dc7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39dc7-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39dc7-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="39dc7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39dc7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39dc7-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39dc7-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="39dc7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39dc7-115">Application</span></span>|<span data-ttu-id="39dc7-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="39dc7-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="39dc7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39dc7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="39dc7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39dc7-118">Request headers</span></span>
|<span data-ttu-id="39dc7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="39dc7-119">Name</span></span>|<span data-ttu-id="39dc7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39dc7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="39dc7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39dc7-121">Authorization</span></span>|<span data-ttu-id="39dc7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39dc7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39dc7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39dc7-124">Request body</span></span>
<span data-ttu-id="39dc7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39dc7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39dc7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dc7-126">Response</span></span>

<span data-ttu-id="39dc7-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="39dc7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="39dc7-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="39dc7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39dc7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="39dc7-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39dc7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="39dc7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="39dc7-131">C#</span><span class="sxs-lookup"><span data-stu-id="39dc7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39dc7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39dc7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39dc7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39dc7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39dc7-134">Java</span><span class="sxs-lookup"><span data-stu-id="39dc7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="39dc7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dc7-135">Response</span></span>
<span data-ttu-id="39dc7-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="39dc7-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



