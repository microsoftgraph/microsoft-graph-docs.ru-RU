---
title: Удаление Итемемаил
description: Удаление объекта Итемемаил из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 51978f3f57be0244f5320688466ac21dcd94dd0b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997395"
---
# <a name="delete-itememail"></a><span data-ttu-id="6c21d-103">Удаление Итемемаил</span><span class="sxs-lookup"><span data-stu-id="6c21d-103">Delete itemEmail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c21d-104">Удаление объекта [итемемаил](../resources/itememail.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="6c21d-104">Delete an [itemEmail](../resources/itememail.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c21d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c21d-105">Permissions</span></span>

<span data-ttu-id="6c21d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c21d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c21d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c21d-108">Permission type</span></span>                        | <span data-ttu-id="6c21d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c21d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c21d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c21d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c21d-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c21d-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6c21d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c21d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c21d-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c21d-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6c21d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c21d-114">Application</span></span>                            | <span data-ttu-id="6c21d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c21d-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="6c21d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c21d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/emails/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="6c21d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c21d-117">Request headers</span></span>

| <span data-ttu-id="6c21d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6c21d-118">Name</span></span>           |<span data-ttu-id="6c21d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6c21d-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="6c21d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c21d-120">Authorization</span></span>  | <span data-ttu-id="6c21d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c21d-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="6c21d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c21d-123">Request body</span></span>

<span data-ttu-id="6c21d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c21d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c21d-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c21d-125">Response</span></span>

<span data-ttu-id="6c21d-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6c21d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c21d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c21d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c21d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c21d-129">Request</span></span>

<span data-ttu-id="6c21d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c21d-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6c21d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c21d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itememail"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/emails/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6c21d-132">C#</span><span class="sxs-lookup"><span data-stu-id="6c21d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c21d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c21d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6c21d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c21d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c21d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c21d-135">Response</span></span>

<span data-ttu-id="6c21d-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6c21d-136">The following is an example of the response.</span></span>

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
  "description": "Delete itemEmail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
