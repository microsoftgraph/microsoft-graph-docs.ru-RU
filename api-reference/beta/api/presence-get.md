---
title: Получение сведений о присутствии
description: Получение сведений о присутствии пользователя.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: f993c68b9858523a621f23bc182f6f6113c50366
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863352"
---
# <a name="get-presence"></a><span data-ttu-id="5bbef-103">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="5bbef-103">Get presence</span></span>

<span data-ttu-id="5bbef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bbef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bbef-105">Получение сведений о [присутствии](../resources/presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bbef-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bbef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bbef-106">Permissions</span></span>
<span data-ttu-id="5bbef-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="5bbef-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="5bbef-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bbef-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bbef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bbef-109">Permission type</span></span> | <span data-ttu-id="5bbef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bbef-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="5bbef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bbef-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bbef-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bbef-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="5bbef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bbef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bbef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bbef-114">Not Supported.</span></span>                        |
| <span data-ttu-id="5bbef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bbef-115">Application</span></span>                            | <span data-ttu-id="5bbef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bbef-116">Not Supported.</span></span>                        |

## <a name="http-requests"></a><span data-ttu-id="5bbef-117">HTTP-запросы</span><span class="sxs-lookup"><span data-stu-id="5bbef-117">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="5bbef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bbef-118">Request Headers</span></span>
| <span data-ttu-id="5bbef-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5bbef-119">Name</span></span>          | <span data-ttu-id="5bbef-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5bbef-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5bbef-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bbef-121">Authorization</span></span> | <span data-ttu-id="5bbef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bbef-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5bbef-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bbef-124">Request body</span></span>

<span data-ttu-id="5bbef-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bbef-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bbef-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbef-126">Response</span></span>
<span data-ttu-id="5bbef-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [присутствия](../resources/presence.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5bbef-127">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5bbef-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5bbef-128">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="5bbef-129">Пример 1: получение собственных сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="5bbef-129">Example 1: Get your own presence information</span></span>

<span data-ttu-id="5bbef-130">В приведенном ниже примере показано, как получить сведения о присутствии.</span><span class="sxs-lookup"><span data-stu-id="5bbef-130">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="5bbef-131">Для выполнения этой операции требуется разрешение на присутствие. чтение.</span><span class="sxs-lookup"><span data-stu-id="5bbef-131">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="5bbef-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bbef-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5bbef-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bbef-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="c"></a>[<span data-ttu-id="5bbef-134">C#</span><span class="sxs-lookup"><span data-stu-id="5bbef-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bbef-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bbef-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bbef-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bbef-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bbef-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbef-137">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="5bbef-138">Пример 2: получение сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="5bbef-138">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="5bbef-139">В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bbef-139">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="5bbef-140">Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="5bbef-140">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="5bbef-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bbef-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5bbef-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bbef-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="5bbef-143">C#</span><span class="sxs-lookup"><span data-stu-id="5bbef-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bbef-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bbef-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bbef-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bbef-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bbef-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbef-146">Response</span></span>

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

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="5bbef-147">Пример 3: получение сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="5bbef-147">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="5bbef-148">В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bbef-148">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="5bbef-149">Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="5bbef-149">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="5bbef-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bbef-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5bbef-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bbef-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="5bbef-152">C#</span><span class="sxs-lookup"><span data-stu-id="5bbef-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bbef-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bbef-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bbef-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bbef-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bbef-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bbef-155">Response</span></span>

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
