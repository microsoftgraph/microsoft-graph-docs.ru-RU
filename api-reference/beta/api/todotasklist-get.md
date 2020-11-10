---
title: Получение Тодотасклист
description: Чтение свойств и связей объекта Тодотасклист.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bbc3202f2f4e7ed4e54c1f0cc9e18351a15cf3f0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980973"
---
# <a name="get-todotasklist"></a><span data-ttu-id="2a124-103">Получение Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="2a124-103">Get todoTaskList</span></span>
<span data-ttu-id="2a124-104">Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="2a124-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="2a124-105">Чтение свойств и связей объекта [тодотасклист](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="2a124-105">Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a124-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a124-106">Permissions</span></span>
<span data-ttu-id="2a124-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a124-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a124-109">Permission type</span></span>|<span data-ttu-id="2a124-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a124-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a124-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a124-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a124-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a124-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2a124-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a124-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a124-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a124-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2a124-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a124-115">Application</span></span>|<span data-ttu-id="2a124-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a124-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a124-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a124-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a124-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a124-118">Optional query parameters</span></span>
<span data-ttu-id="2a124-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2a124-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a124-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a124-120">Request headers</span></span>
|<span data-ttu-id="2a124-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2a124-121">Name</span></span>|<span data-ttu-id="2a124-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2a124-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a124-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a124-123">Authorization</span></span>|<span data-ttu-id="2a124-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a124-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a124-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a124-126">Request body</span></span>
<span data-ttu-id="2a124-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a124-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a124-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a124-128">Response</span></span>

<span data-ttu-id="2a124-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тодотасклист](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a124-129">If successful, this method returns a `200 OK` response code and a [todoTaskList](../resources/todotasklist.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a124-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a124-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a124-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a124-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2a124-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a124-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAAABrJAAA="],
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAAABrJAAA=
```
# <a name="c"></a>[<span data-ttu-id="2a124-133">C#</span><span class="sxs-lookup"><span data-stu-id="2a124-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a124-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a124-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a124-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a124-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a124-136">Java</span><span class="sxs-lookup"><span data-stu-id="2a124-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-todotasklist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2a124-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a124-137">Response</span></span>
><span data-ttu-id="2a124-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a124-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTaskList"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.todoTaskList",
    "id": "5daae1ed-e1ed-5daa-ede1-aa5dede1aa5d",
    "displayName": "Monthly tasks",
    "isOwner": "true",
    "isShared": "false",
    "wellknownListName": "defaultList"
  }
}
```



