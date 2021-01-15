---
title: Список задач для дел
description: Получите ресурсы todoTask из свойства навигации задач указанного todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 35e680b4189cf74b22b6f1500c7fe48882c5fd9b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873278"
---
# <a name="list-tasks"></a><span data-ttu-id="2374c-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="2374c-103">List tasks</span></span>
<span data-ttu-id="2374c-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="2374c-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="2374c-105">Получите ресурсы **todoTask** из свойства навигации **задач** указанного [todoTaskList.](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="2374c-105">Get the **todoTask** resources from the **tasks** navigation property of a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2374c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2374c-106">Permissions</span></span>
<span data-ttu-id="2374c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2374c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2374c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2374c-109">Permission type</span></span>|<span data-ttu-id="2374c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2374c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2374c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2374c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2374c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2374c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2374c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2374c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2374c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2374c-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2374c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2374c-115">Application</span></span>|<span data-ttu-id="2374c-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2374c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="2374c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2374c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2374c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2374c-118">Optional query parameters</span></span>
<span data-ttu-id="2374c-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2374c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2374c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2374c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2374c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2374c-121">Request headers</span></span>
|<span data-ttu-id="2374c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2374c-122">Name</span></span>|<span data-ttu-id="2374c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2374c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2374c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2374c-124">Authorization</span></span>|<span data-ttu-id="2374c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2374c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2374c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2374c-127">Request body</span></span>
<span data-ttu-id="2374c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2374c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2374c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2374c-129">Response</span></span>

<span data-ttu-id="2374c-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [todoTask](../resources/todotask.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2374c-130">If successful, this method returns a `200 OK` response code and a collection of [todoTask](../resources/todotask.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2374c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="2374c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2374c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2374c-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2374c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2374c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["35e2-35e2-721a-e235-1a72e2351a7"],
  "name": "get_todotask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/35e2-35e2-721a-e235-1a72e2351a7/tasks
```
# <a name="c"></a>[<span data-ttu-id="2374c-134">C#</span><span class="sxs-lookup"><span data-stu-id="2374c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2374c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2374c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2374c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2374c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2374c-137">Java</span><span class="sxs-lookup"><span data-stu-id="2374c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2374c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2374c-138">Response</span></span>
<span data-ttu-id="2374c-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2374c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.todoTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "@odata.etag":"W/\"xzyPKP0BiUGgld+lMKXwbQAAgdhkVw==\"",
         "importance":"low",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"Linked entity new task 1",
         "createdDateTime":"2020-07-08T11:15:19.9359889Z",
         "lastModifiedDateTime":"2020-07-08T11:15:20.0614375Z",
         "id":"AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtMDACLTAwCgBGAAAD",
         "body":{
            "content":"",
            "contentType":"text"
         },
         "linkedResources@odata.context":"https://graph.microsoft.com/beta/$metadata#users('todoservicetest2412201901%40outlook.com')/todo/lists('35e2-35e2-721a-e235-1a72e2351a7')/tasks('AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtMDACLTAwCgBGAAAD')/linkedResources",
         "linkedResources":[
            {
               "applicationName":"Partner App Name",
               "displayName":"Partner App Name",
               "externalId":"teset1243434",
               "id":"30911960-7321-4cba-9ba0-cdb68e2984c7"
            }
         ]
      }
   ]
}
```



