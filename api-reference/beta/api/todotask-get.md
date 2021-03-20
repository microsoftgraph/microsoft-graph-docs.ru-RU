---
title: Get todoTask
description: Ознакомьтесь с свойствами и отношениями объекта todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8d188675fc35ac647ef11c2016104a52bfca87cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942131"
---
# <a name="get-todotask"></a><span data-ttu-id="988f0-103">Get todoTask</span><span class="sxs-lookup"><span data-stu-id="988f0-103">Get todoTask</span></span>
<span data-ttu-id="988f0-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="988f0-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="988f0-105">Ознакомьтесь с свойствами и отношениями [объекта todoTask.](../resources/todotask.md)</span><span class="sxs-lookup"><span data-stu-id="988f0-105">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="988f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="988f0-106">Permissions</span></span>
<span data-ttu-id="988f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="988f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="988f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="988f0-109">Permission type</span></span>|<span data-ttu-id="988f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="988f0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="988f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="988f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="988f0-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="988f0-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="988f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="988f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="988f0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="988f0-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="988f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="988f0-115">Application</span></span>|<span data-ttu-id="988f0-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="988f0-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="988f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="988f0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="988f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="988f0-118">Optional query parameters</span></span>
<span data-ttu-id="988f0-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="988f0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="988f0-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="988f0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="988f0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="988f0-121">Request headers</span></span>
|<span data-ttu-id="988f0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="988f0-122">Name</span></span>|<span data-ttu-id="988f0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="988f0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="988f0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="988f0-124">Authorization</span></span>|<span data-ttu-id="988f0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="988f0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="988f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="988f0-127">Request body</span></span>
<span data-ttu-id="988f0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="988f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="988f0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="988f0-129">Response</span></span>

<span data-ttu-id="988f0-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект todoTask](../resources/todotask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="988f0-130">If successful, this method returns a `200 OK` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="988f0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="988f0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="988f0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="988f0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="988f0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="988f0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "get_todotask_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```
# <a name="c"></a>[<span data-ttu-id="988f0-134">C#</span><span class="sxs-lookup"><span data-stu-id="988f0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="988f0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="988f0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="988f0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="988f0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="988f0-137">Java</span><span class="sxs-lookup"><span data-stu-id="988f0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotask-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="988f0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="988f0-138">Response</span></span>
<span data-ttu-id="988f0-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="988f0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tasks/$entity",
    "@odata.etag": "W/\"s8/ERWT3WEeFpBGD0bDgAA+TWq9g==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "Shop for dinner",
    "createdDateTime": "2020-07-22T10:39:03.7937971Z",
    "lastModifiedDateTime": "2020-07-22T12:02:10.8835421Z",
    "id": "721a35e2-35e2-721a-e235-1a72e2351a72",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "dueDateTime": {
        "dateTime": "2020-08-25T04:00:00.0000000",
        "timeZone": "UTC"
    }
}
```



