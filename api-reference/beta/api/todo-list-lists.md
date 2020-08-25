---
title: Перечисление списков
description: Получение списка объектов Тодотасклист и их свойств.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 97ce611af4441027146d2ccd5d951beacd9d20d6
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873274"
---
# <a name="list-lists"></a><span data-ttu-id="b1269-103">Перечисление списков</span><span class="sxs-lookup"><span data-stu-id="b1269-103">List lists</span></span>
<span data-ttu-id="b1269-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1269-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1269-105">Получение списка объектов [тодотасклист](../resources/todotasklist.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="b1269-105">Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1269-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1269-106">Permissions</span></span>
<span data-ttu-id="b1269-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1269-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1269-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1269-109">Permission type</span></span>|<span data-ttu-id="b1269-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1269-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1269-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1269-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1269-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1269-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b1269-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1269-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1269-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1269-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="b1269-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1269-115">Application</span></span>|<span data-ttu-id="b1269-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b1269-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1269-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1269-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists
GET /users/{id|userPrincipalName}/todo/lists
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1269-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1269-118">Optional query parameters</span></span>
<span data-ttu-id="b1269-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b1269-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b1269-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b1269-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1269-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1269-121">Request headers</span></span>
|<span data-ttu-id="b1269-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b1269-122">Name</span></span>|<span data-ttu-id="b1269-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b1269-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b1269-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1269-124">Authorization</span></span>|<span data-ttu-id="b1269-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1269-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1269-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1269-127">Request body</span></span>
<span data-ttu-id="b1269-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1269-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1269-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1269-129">Response</span></span>

<span data-ttu-id="b1269-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тодотасклист](../resources/todotasklist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1269-130">If successful, this method returns a `200 OK` response code and a collection of [todoTaskList](../resources/todotasklist.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1269-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b1269-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1269-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1269-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b1269-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1269-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_todotasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists
```
# <a name="c"></a>[<span data-ttu-id="b1269-134">C#</span><span class="sxs-lookup"><span data-stu-id="b1269-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1269-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1269-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1269-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1269-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b1269-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1269-137">Response</span></span>
<span data-ttu-id="b1269-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b1269-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

