---
title: Получение сведений о присутствии
description: Получение сведений о присутствии пользователя.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: cdb211e85f3e995801bb7583a8aa043cb2d6a133
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913088"
---
# <a name="get-presence"></a><span data-ttu-id="238d9-103">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="238d9-103">Get presence</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="238d9-104">Получение сведений о [присутствии](../resources/presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="238d9-104">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="238d9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="238d9-105">Permissions</span></span>
<span data-ttu-id="238d9-106">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="238d9-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="238d9-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="238d9-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="238d9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="238d9-108">Permission type</span></span> | <span data-ttu-id="238d9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="238d9-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="238d9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="238d9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="238d9-111">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="238d9-111">Presence.Read, Presence.Read.All</span></span>                         |
| <span data-ttu-id="238d9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="238d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="238d9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="238d9-113">Not Supported.</span></span>                         |
| <span data-ttu-id="238d9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="238d9-114">Application</span></span>                            | <span data-ttu-id="238d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="238d9-115">Not Supported.</span></span>                                  |

## <a name="http-requests"></a><span data-ttu-id="238d9-116">HTTP-запросы</span><span class="sxs-lookup"><span data-stu-id="238d9-116">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
```

## <a name="request-headers"></a><span data-ttu-id="238d9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="238d9-117">Request Headers</span></span>
| <span data-ttu-id="238d9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="238d9-118">Name</span></span>          | <span data-ttu-id="238d9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="238d9-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="238d9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="238d9-120">Authorization</span></span> | <span data-ttu-id="238d9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="238d9-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="238d9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="238d9-123">Request body</span></span>

<span data-ttu-id="238d9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="238d9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="238d9-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="238d9-125">Response</span></span>
<span data-ttu-id="238d9-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [присутствия](../resources/presence.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="238d9-126">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="238d9-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="238d9-127">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="238d9-128">Пример 1: получение собственных сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="238d9-128">Example 1: Get your own presence information</span></span>

<span data-ttu-id="238d9-129">В приведенном ниже примере показано, как получить сведения о присутствии.</span><span class="sxs-lookup"><span data-stu-id="238d9-129">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="238d9-130">Для выполнения этой операции требуется разрешение на присутствие. чтение.</span><span class="sxs-lookup"><span data-stu-id="238d9-130">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="238d9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="238d9-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="238d9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="238d9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="238d9-133">C#</span><span class="sxs-lookup"><span data-stu-id="238d9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="238d9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="238d9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="238d9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="238d9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="238d9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="238d9-136">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="238d9-137">Пример 2: получение сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="238d9-137">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="238d9-138">В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="238d9-138">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="238d9-139">Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="238d9-139">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="238d9-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="238d9-140">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="238d9-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="238d9-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="238d9-142">C#</span><span class="sxs-lookup"><span data-stu-id="238d9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="238d9-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="238d9-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="238d9-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="238d9-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="238d9-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="238d9-145">Response</span></span>

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
