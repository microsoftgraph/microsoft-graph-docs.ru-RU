---
title: Удаление профиля
description: Удаление профиля.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5acbffb4f272b5c5c8b760dd7a032608189d78ad
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998060"
---
# <a name="delete-profile"></a><span data-ttu-id="e147e-103">Удаление профиля</span><span class="sxs-lookup"><span data-stu-id="e147e-103">Delete profile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e147e-104">Удаление объекта [Profile](../resources/profile.md) из учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="e147e-104">Delete [profile](../resources/profile.md) object from a user's account.</span></span>

## <a name="permissions"></a><span data-ttu-id="e147e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e147e-105">Permissions</span></span>

<span data-ttu-id="e147e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e147e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e147e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e147e-108">Permission type</span></span>                        | <span data-ttu-id="e147e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e147e-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e147e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e147e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e147e-111">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e147e-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e147e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e147e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e147e-113">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e147e-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e147e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e147e-114">Application</span></span>                            | <span data-ttu-id="e147e-115">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e147e-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e147e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e147e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile
```

## <a name="request-headers"></a><span data-ttu-id="e147e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e147e-117">Request headers</span></span>

| <span data-ttu-id="e147e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e147e-118">Name</span></span>           |<span data-ttu-id="e147e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e147e-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e147e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e147e-120">Authorization</span></span>  | <span data-ttu-id="e147e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e147e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e147e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e147e-123">Content-Type</span></span>   | <span data-ttu-id="e147e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e147e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e147e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e147e-126">Request body</span></span>

<span data-ttu-id="e147e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e147e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e147e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e147e-128">Response</span></span>

<span data-ttu-id="e147e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e147e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e147e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e147e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e147e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e147e-132">Request</span></span>

<span data-ttu-id="e147e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e147e-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e147e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e147e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_profile"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e147e-135">C#</span><span class="sxs-lookup"><span data-stu-id="e147e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e147e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e147e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e147e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e147e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e147e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e147e-138">Response</span></span>

<span data-ttu-id="e147e-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e147e-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete profile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
