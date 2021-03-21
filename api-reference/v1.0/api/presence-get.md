---
title: Получить присутствие
description: Получите сведения о присутствии пользователя.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: ccd05e056f4d751184dd2b5fbb9605377a9a64a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959698"
---
# <a name="get-presence"></a><span data-ttu-id="54bc8-103">Получить присутствие</span><span class="sxs-lookup"><span data-stu-id="54bc8-103">Get presence</span></span>

<span data-ttu-id="54bc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54bc8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54bc8-105">Получите сведения о [присутствии](../resources/presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="54bc8-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="54bc8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54bc8-106">Permissions</span></span>
<span data-ttu-id="54bc8-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="54bc8-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="54bc8-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54bc8-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54bc8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54bc8-109">Permission type</span></span> | <span data-ttu-id="54bc8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54bc8-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="54bc8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54bc8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54bc8-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="54bc8-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="54bc8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54bc8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54bc8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54bc8-114">Not Supported.</span></span>                        |
| <span data-ttu-id="54bc8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54bc8-115">Application</span></span>                            | <span data-ttu-id="54bc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54bc8-116">Not Supported.</span></span>                        |

> <span data-ttu-id="54bc8-117">**Примечание:** Максимальная скорость запроса для этого API — 1500 запросов API в течение 30 секунд на каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="54bc8-117">**Note:** The maximum request rate for this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-requests"></a><span data-ttu-id="54bc8-118">HTTP-запросы</span><span class="sxs-lookup"><span data-stu-id="54bc8-118">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="54bc8-119">Запрашивать заглавные</span><span class="sxs-lookup"><span data-stu-id="54bc8-119">Request Headers</span></span>
| <span data-ttu-id="54bc8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="54bc8-120">Name</span></span>          | <span data-ttu-id="54bc8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="54bc8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="54bc8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54bc8-122">Authorization</span></span> | <span data-ttu-id="54bc8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54bc8-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="54bc8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54bc8-125">Request body</span></span>

<span data-ttu-id="54bc8-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54bc8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54bc8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="54bc8-127">Response</span></span>
<span data-ttu-id="54bc8-128">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [присутствия](../resources/presence.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="54bc8-128">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54bc8-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="54bc8-129">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="54bc8-130">Пример 1. Получить сведения о собственном присутствии</span><span class="sxs-lookup"><span data-stu-id="54bc8-130">Example 1: Get your own presence information</span></span>

<span data-ttu-id="54bc8-131">В следующем примере показано, как получить собственные сведения о присутствии.</span><span class="sxs-lookup"><span data-stu-id="54bc8-131">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="54bc8-132">Для этой операции требуется разрешение Presence.Read.</span><span class="sxs-lookup"><span data-stu-id="54bc8-132">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="54bc8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="54bc8-133">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="54bc8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="54bc8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```
# <a name="c"></a>[<span data-ttu-id="54bc8-135">C#</span><span class="sxs-lookup"><span data-stu-id="54bc8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54bc8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54bc8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54bc8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54bc8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54bc8-138">Java</span><span class="sxs-lookup"><span data-stu-id="54bc8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-your-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="54bc8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="54bc8-139">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="54bc8-140">Пример 2. Получить сведения о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="54bc8-140">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="54bc8-141">В следующем примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="54bc8-141">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="54bc8-142">Для этой операции требуется разрешение Presence.Read.All.</span><span class="sxs-lookup"><span data-stu-id="54bc8-142">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="54bc8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="54bc8-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="54bc8-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="54bc8-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="54bc8-145">C#</span><span class="sxs-lookup"><span data-stu-id="54bc8-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54bc8-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54bc8-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54bc8-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54bc8-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54bc8-148">Java</span><span class="sxs-lookup"><span data-stu-id="54bc8-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="54bc8-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="54bc8-149">Response</span></span>

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

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="54bc8-150">Пример 3. Получить сведения о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="54bc8-150">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="54bc8-151">В следующем примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="54bc8-151">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="54bc8-152">Для этой операции требуется разрешение Presence.Read.All.</span><span class="sxs-lookup"><span data-stu-id="54bc8-152">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="54bc8-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="54bc8-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="54bc8-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="54bc8-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="54bc8-155">C#</span><span class="sxs-lookup"><span data-stu-id="54bc8-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54bc8-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54bc8-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54bc8-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54bc8-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54bc8-158">Java</span><span class="sxs-lookup"><span data-stu-id="54bc8-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="54bc8-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="54bc8-159">Response</span></span>

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


