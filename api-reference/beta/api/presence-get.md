---
title: Получение сведений о присутствии
description: Получение сведений о присутствии пользователя.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 8b6b1d473357b88123af1c8840c3445ca811cbfd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043075"
---
# <a name="get-presence"></a><span data-ttu-id="575eb-103">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="575eb-103">Get presence</span></span>

<span data-ttu-id="575eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="575eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="575eb-105">Получение сведений о [присутствии](../resources/presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="575eb-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="575eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="575eb-106">Permissions</span></span>
<span data-ttu-id="575eb-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="575eb-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="575eb-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="575eb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="575eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="575eb-109">Permission type</span></span> | <span data-ttu-id="575eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="575eb-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="575eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="575eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="575eb-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="575eb-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="575eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="575eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="575eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="575eb-114">Not Supported.</span></span>                        |
| <span data-ttu-id="575eb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="575eb-115">Application</span></span>                            | <span data-ttu-id="575eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="575eb-116">Not Supported.</span></span>                        |

## <a name="http-requests"></a><span data-ttu-id="575eb-117">HTTP-запросы</span><span class="sxs-lookup"><span data-stu-id="575eb-117">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="575eb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="575eb-118">Request Headers</span></span>
| <span data-ttu-id="575eb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="575eb-119">Name</span></span>          | <span data-ttu-id="575eb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="575eb-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="575eb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="575eb-121">Authorization</span></span> | <span data-ttu-id="575eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="575eb-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="575eb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="575eb-124">Request body</span></span>

<span data-ttu-id="575eb-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="575eb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="575eb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="575eb-126">Response</span></span>
<span data-ttu-id="575eb-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [присутствия](../resources/presence.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="575eb-127">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="575eb-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="575eb-128">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="575eb-129">Пример 1: получение собственных сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="575eb-129">Example 1: Get your own presence information</span></span>

<span data-ttu-id="575eb-130">В приведенном ниже примере показано, как получить сведения о присутствии.</span><span class="sxs-lookup"><span data-stu-id="575eb-130">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="575eb-131">Для выполнения этой операции требуется разрешение на присутствие. чтение.</span><span class="sxs-lookup"><span data-stu-id="575eb-131">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="575eb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="575eb-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="575eb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="575eb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="c"></a>[<span data-ttu-id="575eb-134">C#</span><span class="sxs-lookup"><span data-stu-id="575eb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="575eb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="575eb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="575eb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="575eb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="575eb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="575eb-137">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="575eb-138">Пример 2: получение сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="575eb-138">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="575eb-139">В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="575eb-139">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="575eb-140">Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="575eb-140">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="575eb-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="575eb-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="575eb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="575eb-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="575eb-143">C#</span><span class="sxs-lookup"><span data-stu-id="575eb-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="575eb-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="575eb-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="575eb-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="575eb-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="575eb-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="575eb-146">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="575eb-147">Пример 3: получение сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="575eb-147">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="575eb-148">В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="575eb-148">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="575eb-149">Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="575eb-149">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="575eb-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="575eb-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="575eb-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="575eb-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="575eb-152">C#</span><span class="sxs-lookup"><span data-stu-id="575eb-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="575eb-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="575eb-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="575eb-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="575eb-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="575eb-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="575eb-155">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


