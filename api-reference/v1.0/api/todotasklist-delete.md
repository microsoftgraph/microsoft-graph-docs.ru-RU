---
title: Удаление Тодотасклист
description: Удаляет объект Тодотасклист.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4f8029417e841d2bebdf6224946342a7d9ea8797
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904976"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="678ee-103">Удаление Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="678ee-103">Delete todoTaskList</span></span>
<span data-ttu-id="678ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="678ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="678ee-105">Удаляет объект [тодотасклист](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="678ee-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="678ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="678ee-106">Permissions</span></span>
<span data-ttu-id="678ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="678ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="678ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="678ee-109">Permission type</span></span>|<span data-ttu-id="678ee-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="678ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="678ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="678ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="678ee-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="678ee-112">Tasks.Read</span></span>|
|<span data-ttu-id="678ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="678ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="678ee-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="678ee-114">Tasks.Read</span></span>|
|<span data-ttu-id="678ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="678ee-115">Application</span></span>|<span data-ttu-id="678ee-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="678ee-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="678ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="678ee-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="678ee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="678ee-118">Request headers</span></span>
|<span data-ttu-id="678ee-119">Имя</span><span class="sxs-lookup"><span data-stu-id="678ee-119">Name</span></span>|<span data-ttu-id="678ee-120">Описание</span><span class="sxs-lookup"><span data-stu-id="678ee-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="678ee-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="678ee-121">Authorization</span></span>|<span data-ttu-id="678ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="678ee-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="678ee-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="678ee-124">Request body</span></span>
<span data-ttu-id="678ee-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="678ee-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="678ee-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="678ee-126">Response</span></span>

<span data-ttu-id="678ee-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="678ee-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="678ee-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="678ee-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="678ee-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="678ee-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="678ee-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="678ee-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="678ee-131">C#</span><span class="sxs-lookup"><span data-stu-id="678ee-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="678ee-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="678ee-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="678ee-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="678ee-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="678ee-134">Java</span><span class="sxs-lookup"><span data-stu-id="678ee-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="678ee-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="678ee-135">Response</span></span>
<span data-ttu-id="678ee-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="678ee-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



