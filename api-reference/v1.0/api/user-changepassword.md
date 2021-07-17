---
title: 'пользователь: changePassword'
description: Обновление собственного пароля.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2adf91adb5eab959dc981f0532c4017e838852ab
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441713"
---
# <a name="user-changepassword"></a><span data-ttu-id="7ea37-103">пользователь: changePassword</span><span class="sxs-lookup"><span data-stu-id="7ea37-103">user: changePassword</span></span>

<span data-ttu-id="7ea37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ea37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ea37-105">Внося пользователю возможность обновить пароль.</span><span class="sxs-lookup"><span data-stu-id="7ea37-105">Enable the user to update their password.</span></span> <span data-ttu-id="7ea37-106">Любой пользователь может обновить пароль, не относясь к роли администратора.</span><span class="sxs-lookup"><span data-stu-id="7ea37-106">Any user can update their password without belonging to any administrator role.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ea37-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ea37-107">Permissions</span></span>
<span data-ttu-id="7ea37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ea37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ea37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ea37-110">Permission type</span></span>      | <span data-ttu-id="7ea37-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ea37-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ea37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ea37-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ea37-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ea37-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ea37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ea37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ea37-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ea37-115">Not supported.</span></span>    |
|<span data-ttu-id="7ea37-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ea37-116">Application</span></span> | <span data-ttu-id="7ea37-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ea37-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ea37-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ea37-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/changePassword
```
## <a name="request-headers"></a><span data-ttu-id="7ea37-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ea37-119">Request headers</span></span>
| <span data-ttu-id="7ea37-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ea37-120">Header</span></span>       | <span data-ttu-id="7ea37-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7ea37-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ea37-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ea37-122">Authorization</span></span>  | <span data-ttu-id="7ea37-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ea37-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ea37-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7ea37-125">Content-type</span></span>  | <span data-ttu-id="7ea37-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ea37-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ea37-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ea37-128">Request body</span></span>
<span data-ttu-id="7ea37-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7ea37-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7ea37-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="7ea37-130">Parameter</span></span>    | <span data-ttu-id="7ea37-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ea37-131">Type</span></span>   |<span data-ttu-id="7ea37-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ea37-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ea37-133">currentPassword</span><span class="sxs-lookup"><span data-stu-id="7ea37-133">currentPassword</span></span> | <span data-ttu-id="7ea37-134">String</span><span class="sxs-lookup"><span data-stu-id="7ea37-134">String</span></span> | <span data-ttu-id="7ea37-135">Текущий пароль.</span><span class="sxs-lookup"><span data-stu-id="7ea37-135">Your current password.</span></span>|
| <span data-ttu-id="7ea37-136">newPassword</span><span class="sxs-lookup"><span data-stu-id="7ea37-136">newPassword</span></span> | <span data-ttu-id="7ea37-137">String</span><span class="sxs-lookup"><span data-stu-id="7ea37-137">String</span></span> | <span data-ttu-id="7ea37-138">Новый пароль.</span><span class="sxs-lookup"><span data-stu-id="7ea37-138">Your new password.</span></span>|

## <a name="response"></a><span data-ttu-id="7ea37-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ea37-139">Response</span></span>

<span data-ttu-id="7ea37-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7ea37-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7ea37-141">Пример</span><span class="sxs-lookup"><span data-stu-id="7ea37-141">Example</span></span>
<span data-ttu-id="7ea37-142">В следующем примере показан запрос на обновление собственного пароля.</span><span class="sxs-lookup"><span data-stu-id="7ea37-142">The following example shows a request to update your own password.</span></span>

### <a name="request"></a><span data-ttu-id="7ea37-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ea37-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7ea37-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ea37-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_changepassword"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/changePassword
Content-type: application/json

{
    "currentPassword": "xWwvJ]6NMw+bWH-d",
    "newPassword": "0eM85N54wFxWwvJ]"
}
```
# <a name="c"></a>[<span data-ttu-id="7ea37-145">C#</span><span class="sxs-lookup"><span data-stu-id="7ea37-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-changepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ea37-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ea37-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-changepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ea37-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ea37-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-changepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ea37-148">Java</span><span class="sxs-lookup"><span data-stu-id="7ea37-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-changepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7ea37-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ea37-149">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="7ea37-150">См. также</span><span class="sxs-lookup"><span data-stu-id="7ea37-150">See also</span></span>
+ [<span data-ttu-id="7ea37-151">Обновление passwordProfile пользователя для сброса пароля</span><span class="sxs-lookup"><span data-stu-id="7ea37-151">Update the passwordProfile of a user to reset their password</span></span>](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)

<!-- uuid: a7c9a0de-8324-4f80-8d88-2e6d5838f3be
2021-06-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: changePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


