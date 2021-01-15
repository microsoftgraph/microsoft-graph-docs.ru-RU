---
title: Delete todoTaskList
description: Удаляет объект todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7881513af6f97f96f212854d9e994de19e234dc6
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874265"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="88b4d-103">Delete todoTaskList</span><span class="sxs-lookup"><span data-stu-id="88b4d-103">Delete todoTaskList</span></span>
<span data-ttu-id="88b4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88b4d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88b4d-105">Удаляет объект [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="88b4d-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="88b4d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88b4d-106">Permissions</span></span>
<span data-ttu-id="88b4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88b4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88b4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88b4d-109">Permission type</span></span>|<span data-ttu-id="88b4d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88b4d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88b4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88b4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88b4d-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="88b4d-112">Tasks.Read</span></span>|
|<span data-ttu-id="88b4d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88b4d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88b4d-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="88b4d-114">Tasks.Read</span></span>|
|<span data-ttu-id="88b4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88b4d-115">Application</span></span>|<span data-ttu-id="88b4d-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="88b4d-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="88b4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88b4d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="88b4d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88b4d-118">Request headers</span></span>
|<span data-ttu-id="88b4d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="88b4d-119">Name</span></span>|<span data-ttu-id="88b4d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="88b4d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88b4d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88b4d-121">Authorization</span></span>|<span data-ttu-id="88b4d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88b4d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88b4d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88b4d-124">Request body</span></span>
<span data-ttu-id="88b4d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88b4d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88b4d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="88b4d-126">Response</span></span>

<span data-ttu-id="88b4d-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88b4d-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="88b4d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="88b4d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88b4d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="88b4d-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88b4d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="88b4d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="88b4d-131">C#</span><span class="sxs-lookup"><span data-stu-id="88b4d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88b4d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88b4d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88b4d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88b4d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88b4d-134">Java</span><span class="sxs-lookup"><span data-stu-id="88b4d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="88b4d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="88b4d-135">Response</span></span>
<span data-ttu-id="88b4d-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="88b4d-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



