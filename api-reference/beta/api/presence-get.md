---
title: Получить присутствие
description: Получите сведения о присутствии пользователя.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 80a5bd421d3c8ab5497f0b52a52fb77135e11648
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796712"
---
# <a name="get-presence"></a><span data-ttu-id="4124e-103">Получить присутствие</span><span class="sxs-lookup"><span data-stu-id="4124e-103">Get presence</span></span>

<span data-ttu-id="4124e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4124e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4124e-105">Получите сведения о [присутствии](../resources/presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="4124e-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="4124e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4124e-106">Permissions</span></span>
<span data-ttu-id="4124e-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="4124e-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="4124e-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4124e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4124e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4124e-109">Permission type</span></span> | <span data-ttu-id="4124e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4124e-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="4124e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4124e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4124e-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="4124e-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="4124e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4124e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4124e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4124e-114">Not Supported.</span></span>                        |
| <span data-ttu-id="4124e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4124e-115">Application</span></span>                            | <span data-ttu-id="4124e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4124e-116">Not Supported.</span></span>                        |

## <a name="http-requests"></a><span data-ttu-id="4124e-117">HTTP-запросы</span><span class="sxs-lookup"><span data-stu-id="4124e-117">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="4124e-118">Заглавные запросы</span><span class="sxs-lookup"><span data-stu-id="4124e-118">Request Headers</span></span>
| <span data-ttu-id="4124e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4124e-119">Name</span></span>          | <span data-ttu-id="4124e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4124e-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4124e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4124e-121">Authorization</span></span> | <span data-ttu-id="4124e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4124e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4124e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4124e-124">Request body</span></span>

<span data-ttu-id="4124e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4124e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4124e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4124e-126">Response</span></span>
<span data-ttu-id="4124e-127">В случае успеха этот метод возвращает код отклика и объект `200 OK` [присутствия](../resources/presence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4124e-127">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4124e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="4124e-128">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="4124e-129">Пример 1. Получите сведения о присутствии</span><span class="sxs-lookup"><span data-stu-id="4124e-129">Example 1: Get your own presence information</span></span>

<span data-ttu-id="4124e-130">В следующем примере показано, как получить собственные сведения о присутствии.</span><span class="sxs-lookup"><span data-stu-id="4124e-130">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="4124e-131">Для этой операции требуется разрешение Presence.Read.</span><span class="sxs-lookup"><span data-stu-id="4124e-131">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4124e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4124e-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4124e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4124e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="c"></a>[<span data-ttu-id="4124e-134">C#</span><span class="sxs-lookup"><span data-stu-id="4124e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4124e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4124e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4124e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4124e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4124e-137">Java</span><span class="sxs-lookup"><span data-stu-id="4124e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-your-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4124e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4124e-138">Response</span></span>

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
  "activity": "Available",
  "outOfOfficeSettings": {
    "message": null,
    "isOutOfOffice": false
  }
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="4124e-139">Пример 2. Получите сведения о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="4124e-139">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="4124e-140">В следующем примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4124e-140">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="4124e-141">Для этой операции требуется разрешение Presence.Read.All.</span><span class="sxs-lookup"><span data-stu-id="4124e-141">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4124e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4124e-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4124e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4124e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="4124e-144">C#</span><span class="sxs-lookup"><span data-stu-id="4124e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4124e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4124e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4124e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4124e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4124e-147">Java</span><span class="sxs-lookup"><span data-stu-id="4124e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4124e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="4124e-148">Response</span></span>

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
  "activity": "Presenting",
  "outOfOfficeSettings": {
    "message": null,
    "isOutOfOffice": false
  }
}
```

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="4124e-149">Пример 3. Получите сведения о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="4124e-149">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="4124e-150">В следующем примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4124e-150">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="4124e-151">Для этой операции требуется разрешение Presence.Read.All.</span><span class="sxs-lookup"><span data-stu-id="4124e-151">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4124e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="4124e-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4124e-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="4124e-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="4124e-154">C#</span><span class="sxs-lookup"><span data-stu-id="4124e-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4124e-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4124e-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4124e-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4124e-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4124e-157">Java</span><span class="sxs-lookup"><span data-stu-id="4124e-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4124e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4124e-158">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
  "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
  "availability": "Away",
  "activity": "BeRightBack",
  "outOfOfficeSettings": {
    "message": null,
    "isOutOfOffice": false
  }
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


