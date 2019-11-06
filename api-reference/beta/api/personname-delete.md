---
title: Удаление personName
description: Удаление объекта personName из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0c058173371afd538ab9a5cd3da6dea8499b296d
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997256"
---
# <a name="delete-personname"></a><span data-ttu-id="26972-103">Удаление personName</span><span class="sxs-lookup"><span data-stu-id="26972-103">Delete personName</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26972-104">Удаление объекта [PersonName](../resources/personname.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="26972-104">Delete a [personName](../resources/personname.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26972-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26972-105">Permissions</span></span>

<span data-ttu-id="26972-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26972-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26972-108">Permission type</span></span>                        | <span data-ttu-id="26972-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26972-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26972-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26972-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="26972-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="26972-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="26972-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26972-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26972-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="26972-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="26972-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26972-114">Application</span></span>                            | <span data-ttu-id="26972-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26972-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="26972-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26972-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26972-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26972-117">Request headers</span></span>

| <span data-ttu-id="26972-118">Имя</span><span class="sxs-lookup"><span data-stu-id="26972-118">Name</span></span>           |<span data-ttu-id="26972-119">Описание</span><span class="sxs-lookup"><span data-stu-id="26972-119">Description</span></span>                  | 
|:---------------|:----------------------------|
| <span data-ttu-id="26972-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26972-120">Authorization</span></span>  | <span data-ttu-id="26972-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26972-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="26972-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26972-123">Content-Type</span></span>   | <span data-ttu-id="26972-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26972-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26972-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26972-126">Request body</span></span>

<span data-ttu-id="26972-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26972-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26972-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="26972-128">Response</span></span>

<span data-ttu-id="26972-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="26972-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26972-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="26972-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26972-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26972-132">Request</span></span>

<span data-ttu-id="26972-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26972-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="26972-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="26972-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personname"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/names/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="26972-135">C#</span><span class="sxs-lookup"><span data-stu-id="26972-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26972-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26972-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26972-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26972-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26972-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="26972-138">Response</span></span>

<span data-ttu-id="26972-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="26972-139">The following is an example of the response.</span></span>

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
  "description": "Delete personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
