---
title: Увольнение riskyUser
description: Отклонять риск объекта riskyUser.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 47b749e1ac5d782d96210b493ed1451db19184c7
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761488"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="584f7-103">riskyUser: увольнение</span><span class="sxs-lookup"><span data-stu-id="584f7-103">riskyUser: dismiss</span></span>

<span data-ttu-id="584f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="584f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="584f7-105">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="584f7-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="584f7-106">Отклонять риск одного или более [объектов riskyUser.](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="584f7-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="584f7-107">Это действие задает целевому пользователю уровень риска ни к одному.</span><span class="sxs-lookup"><span data-stu-id="584f7-107">This action sets the targeted user's risk level to none.</span></span> <span data-ttu-id="584f7-108">Максимальное количество пользователей, отклоняться при одном вызове, — 60.</span><span class="sxs-lookup"><span data-stu-id="584f7-108">The maximum count of users to dismiss in one call is 60.</span></span>

## <a name="permissions"></a><span data-ttu-id="584f7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="584f7-109">Permissions</span></span>
<span data-ttu-id="584f7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="584f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="584f7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="584f7-112">Permission type</span></span>      | <span data-ttu-id="584f7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="584f7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="584f7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="584f7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="584f7-115">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584f7-115">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="584f7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="584f7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="584f7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="584f7-117">Not supported.</span></span>    |
|<span data-ttu-id="584f7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="584f7-118">Application</span></span> | <span data-ttu-id="584f7-119">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="584f7-119">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="584f7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="584f7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="584f7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="584f7-121">Request headers</span></span>
| <span data-ttu-id="584f7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="584f7-122">Name</span></span>      |<span data-ttu-id="584f7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="584f7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="584f7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="584f7-124">Authorization</span></span>  | <span data-ttu-id="584f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="584f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="584f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="584f7-127">Request body</span></span>
<span data-ttu-id="584f7-128">Укажите пользовательские интерфейсы, которые необходимо отклонять в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="584f7-128">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="584f7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="584f7-129">Response</span></span>

<span data-ttu-id="584f7-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="584f7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="584f7-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="584f7-132">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="584f7-133">Пример 1. Увольнение рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="584f7-133">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="584f7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="584f7-134">Request</span></span>
<span data-ttu-id="584f7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="584f7-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="584f7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="584f7-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="584f7-137">C#</span><span class="sxs-lookup"><span data-stu-id="584f7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="584f7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="584f7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="584f7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="584f7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="584f7-140">Java</span><span class="sxs-lookup"><span data-stu-id="584f7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="584f7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="584f7-141">Response</span></span>
<span data-ttu-id="584f7-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="584f7-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="584f7-143">Пример 2. Увольнение рискованного пользователя</span><span class="sxs-lookup"><span data-stu-id="584f7-143">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="584f7-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="584f7-144">Request</span></span>
<span data-ttu-id="584f7-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="584f7-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="584f7-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="584f7-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="584f7-147">C#</span><span class="sxs-lookup"><span data-stu-id="584f7-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="584f7-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="584f7-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="584f7-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="584f7-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="584f7-150">Java</span><span class="sxs-lookup"><span data-stu-id="584f7-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="584f7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="584f7-151">Response</span></span>
<span data-ttu-id="584f7-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="584f7-152">Here is an example of the response.</span></span>
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


