---
title: Перечисление списков
description: Получите список объектов todoTaskList и их свойств.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c4735dff24dbccb8fbb7106a819b0b36bb132d01
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953840"
---
# <a name="list-lists"></a><span data-ttu-id="0b0cf-103">Перечисление списков</span><span class="sxs-lookup"><span data-stu-id="0b0cf-103">List lists</span></span>
<span data-ttu-id="0b0cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b0cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b0cf-105">Получите список объектов [todoTaskList](../resources/todotasklist.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="0b0cf-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b0cf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b0cf-106">Permissions</span></span>
<span data-ttu-id="0b0cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b0cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b0cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b0cf-109">Permission type</span></span>|<span data-ttu-id="0b0cf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b0cf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b0cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b0cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b0cf-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b0cf-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0b0cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b0cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b0cf-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b0cf-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0b0cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b0cf-115">Application</span></span>|<span data-ttu-id="0b0cf-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0b0cf-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b0cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b0cf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b0cf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b0cf-118">Optional query parameters</span></span>
<span data-ttu-id="0b0cf-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0b0cf-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0b0cf-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0b0cf-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b0cf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b0cf-121">Request headers</span></span>
|<span data-ttu-id="0b0cf-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0b0cf-122">Name</span></span>|<span data-ttu-id="0b0cf-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0b0cf-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b0cf-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b0cf-124">Authorization</span></span>|<span data-ttu-id="0b0cf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b0cf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b0cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b0cf-127">Request body</span></span>
<span data-ttu-id="0b0cf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b0cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b0cf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b0cf-129">Response</span></span>

<span data-ttu-id="0b0cf-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [todoTaskList](../resources/todotasklist.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0b0cf-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b0cf-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b0cf-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b0cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b0cf-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0b0cf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b0cf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_todotasklist_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```
# <a name="c"></a>[<span data-ttu-id="0b0cf-134">C#</span><span class="sxs-lookup"><span data-stu-id="0b0cf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b0cf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b0cf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b0cf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b0cf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b0cf-137">Java</span><span class="sxs-lookup"><span data-stu-id="0b0cf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0b0cf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b0cf-138">Response</span></span>
<span data-ttu-id="0b0cf-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b0cf-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.todoTaskList)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.todoTaskList",
      "id": "AAMkADIyAAAAABrJAAA=",
      "displayName": "Tasks",
      "isOwner": true,
      "isShared": false,
      "wellknownListName": "defaultList"
    },
        {
      "@odata.type": "#microsoft.graph.todoTaskList",
      "id": "AAMkADIyAAAEFTTrJAAA=",
      "displayName": "Monthly Tasks",
      "isOwner":true,
      "isShared": false,
      "wellknownListName": "none"
    }
  ]
}
```



