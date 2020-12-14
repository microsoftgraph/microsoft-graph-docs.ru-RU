---
title: Получить присутствие
description: Получите сведения о присутствии пользователя.
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 591c388418ddb60fad1d78a04de79cb65a884630
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663970"
---
# <a name="get-presence"></a><span data-ttu-id="ac334-103">Получить присутствие</span><span class="sxs-lookup"><span data-stu-id="ac334-103">Get presence</span></span>

<span data-ttu-id="ac334-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac334-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac334-105">Получите сведения о [присутствии](../resources/presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac334-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac334-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac334-106">Permissions</span></span>
<span data-ttu-id="ac334-107">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="ac334-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="ac334-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac334-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac334-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac334-109">Permission type</span></span> | <span data-ttu-id="ac334-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac334-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="ac334-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac334-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac334-112">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac334-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="ac334-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac334-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac334-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac334-114">Not Supported.</span></span>                        |
| <span data-ttu-id="ac334-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ac334-115">Application</span></span>                            | <span data-ttu-id="ac334-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac334-116">Not Supported.</span></span>                        |

> <span data-ttu-id="ac334-117">**Примечание.** Максимальная скорость запросов для этого API составляет 1500 запросов API в течение 30 секунд для каждого приложения на клиента.</span><span class="sxs-lookup"><span data-stu-id="ac334-117">**Note:** The maximum request rate for this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-requests"></a><span data-ttu-id="ac334-118">HTTP-запросы</span><span class="sxs-lookup"><span data-stu-id="ac334-118">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="ac334-119">Заглавные запросы</span><span class="sxs-lookup"><span data-stu-id="ac334-119">Request Headers</span></span>
| <span data-ttu-id="ac334-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ac334-120">Name</span></span>          | <span data-ttu-id="ac334-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ac334-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ac334-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac334-122">Authorization</span></span> | <span data-ttu-id="ac334-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac334-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ac334-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac334-125">Request body</span></span>

<span data-ttu-id="ac334-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac334-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac334-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac334-127">Response</span></span>
<span data-ttu-id="ac334-128">В случае успеха этот метод возвращает код отклика и объект `200 OK` [присутствия](../resources/presence.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac334-128">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac334-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac334-129">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="ac334-130">Пример 1. Получите сведения о присутствии</span><span class="sxs-lookup"><span data-stu-id="ac334-130">Example 1: Get your own presence information</span></span>

<span data-ttu-id="ac334-131">В следующем примере показано, как получить собственные сведения о присутствии.</span><span class="sxs-lookup"><span data-stu-id="ac334-131">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="ac334-132">Для этой операции требуется разрешение Presence.Read.</span><span class="sxs-lookup"><span data-stu-id="ac334-132">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="ac334-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac334-133">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="ac334-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac334-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```
# <a name="c"></a>[<span data-ttu-id="ac334-135">C#</span><span class="sxs-lookup"><span data-stu-id="ac334-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac334-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac334-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac334-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac334-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac334-138">Java</span><span class="sxs-lookup"><span data-stu-id="ac334-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-your-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="ac334-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac334-139">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="ac334-140">Пример 2. Просмотр сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="ac334-140">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="ac334-141">В следующем примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac334-141">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="ac334-142">Для этой операции требуется разрешение Presence.Read.All.</span><span class="sxs-lookup"><span data-stu-id="ac334-142">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="ac334-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac334-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ac334-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac334-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="ac334-145">C#</span><span class="sxs-lookup"><span data-stu-id="ac334-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac334-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac334-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac334-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac334-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac334-148">Java</span><span class="sxs-lookup"><span data-stu-id="ac334-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="ac334-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac334-149">Response</span></span>

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

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="ac334-150">Пример 3. Просмотр сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="ac334-150">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="ac334-151">В следующем примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac334-151">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="ac334-152">Для этой операции требуется разрешение Presence.Read.All.</span><span class="sxs-lookup"><span data-stu-id="ac334-152">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="ac334-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac334-153">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```

---


#### <a name="response"></a><span data-ttu-id="ac334-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac334-154">Response</span></span>

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


