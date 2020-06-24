---
title: Отклонить Рискюсер
description: Отклонение риска для объекта Рискюсер.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 3a549ca4b50d1a0e873a905a6312e30d6bf1e838
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863518"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="27735-103">Рискюсер: отклонить</span><span class="sxs-lookup"><span data-stu-id="27735-103">riskyUser: dismiss</span></span>

<span data-ttu-id="27735-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27735-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="27735-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="27735-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="27735-106">Отклонить риск одного или нескольких объектов [рискюсер](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="27735-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="27735-107">Это действие задает для уровня риска целевого пользователя значение нет.</span><span class="sxs-lookup"><span data-stu-id="27735-107">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="27735-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27735-108">Permissions</span></span>
<span data-ttu-id="27735-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="27735-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="27735-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27735-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27735-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27735-111">Permission type</span></span>      | <span data-ttu-id="27735-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27735-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27735-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27735-113">Delegated (work or school account)</span></span> | <span data-ttu-id="27735-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27735-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="27735-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27735-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27735-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27735-116">Not supported.</span></span>    |
|<span data-ttu-id="27735-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27735-117">Application</span></span> | <span data-ttu-id="27735-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27735-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27735-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27735-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="27735-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27735-120">Request headers</span></span>
| <span data-ttu-id="27735-121">Имя</span><span class="sxs-lookup"><span data-stu-id="27735-121">Name</span></span>      |<span data-ttu-id="27735-122">Описание</span><span class="sxs-lookup"><span data-stu-id="27735-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27735-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27735-123">Authorization</span></span>  | <span data-ttu-id="27735-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="27735-124">Bearer {token}.</span></span> <span data-ttu-id="27735-125">Required.</span><span class="sxs-lookup"><span data-stu-id="27735-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27735-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27735-126">Request body</span></span>
<span data-ttu-id="27735-127">Укажите идентификаторы пользователя, которые нужно отклонить в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="27735-127">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="27735-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="27735-128">Response</span></span>

<span data-ttu-id="27735-129">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="27735-129">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="27735-130">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="27735-130">It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="27735-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="27735-131">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="27735-132">Пример 1: отклонение рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="27735-132">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="27735-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="27735-133">Request</span></span>
<span data-ttu-id="27735-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27735-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27735-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="27735-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="27735-136">C#</span><span class="sxs-lookup"><span data-stu-id="27735-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27735-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27735-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27735-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27735-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="27735-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="27735-139">Response</span></span>
<span data-ttu-id="27735-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27735-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="27735-141">Пример 2: отклонение опасного пользователя</span><span class="sxs-lookup"><span data-stu-id="27735-141">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="27735-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="27735-142">Request</span></span>
<span data-ttu-id="27735-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27735-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27735-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="27735-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="27735-145">C#</span><span class="sxs-lookup"><span data-stu-id="27735-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27735-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27735-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27735-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27735-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="27735-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="27735-148">Response</span></span>
<span data-ttu-id="27735-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27735-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
