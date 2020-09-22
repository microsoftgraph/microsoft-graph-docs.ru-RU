---
title: Удаление Тодотасклист
description: Удаляет объект Тодотасклист.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fed835f834b7bd65816613c2d37666294db6be62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058528"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="fc9e3-103">Удаление Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="fc9e3-103">Delete todoTaskList</span></span>
<span data-ttu-id="fc9e3-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="fc9e3-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="fc9e3-105">Удаляет объект [тодотасклист](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="fc9e3-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc9e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc9e3-106">Permissions</span></span>
<span data-ttu-id="fc9e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc9e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc9e3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc9e3-109">Permission type</span></span>|<span data-ttu-id="fc9e3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc9e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc9e3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc9e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc9e3-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fc9e3-112">Tasks.Read</span></span>|
|<span data-ttu-id="fc9e3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc9e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc9e3-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fc9e3-114">Tasks.Read</span></span>|
|<span data-ttu-id="fc9e3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc9e3-115">Application</span></span>|<span data-ttu-id="fc9e3-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fc9e3-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc9e3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc9e3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="fc9e3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc9e3-118">Request headers</span></span>
|<span data-ttu-id="fc9e3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fc9e3-119">Name</span></span>|<span data-ttu-id="fc9e3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fc9e3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fc9e3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc9e3-121">Authorization</span></span>|<span data-ttu-id="fc9e3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc9e3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc9e3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc9e3-124">Request body</span></span>
<span data-ttu-id="fc9e3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc9e3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc9e3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc9e3-126">Response</span></span>

<span data-ttu-id="fc9e3-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fc9e3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fc9e3-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="fc9e3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc9e3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc9e3-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fc9e3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc9e3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="fc9e3-131">C#</span><span class="sxs-lookup"><span data-stu-id="fc9e3-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc9e3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc9e3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc9e3-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc9e3-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fc9e3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc9e3-134">Response</span></span>
<span data-ttu-id="fc9e3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc9e3-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



