---
title: Удаление СкиллпрофиЦиенци
description: Удаление СкиллпрофиЦиенци.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7b77afd4c2ae083408bc565b83f143e968e1646a
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997537"
---
# <a name="delete-skillproficiency"></a><span data-ttu-id="547fa-103">Удаление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="547fa-103">Delete skillProficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="547fa-104">Удаление объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="547fa-104">Delete a [skillProficiency](../resources/skillproficiency.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="547fa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="547fa-105">Permissions</span></span>

<span data-ttu-id="547fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="547fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="547fa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="547fa-108">Permission type</span></span>                        | <span data-ttu-id="547fa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="547fa-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="547fa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="547fa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="547fa-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="547fa-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="547fa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="547fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="547fa-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="547fa-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="547fa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="547fa-114">Application</span></span>                            | <span data-ttu-id="547fa-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="547fa-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="547fa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="547fa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="547fa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="547fa-117">Request headers</span></span>

| <span data-ttu-id="547fa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="547fa-118">Name</span></span>           |<span data-ttu-id="547fa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="547fa-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="547fa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="547fa-120">Authorization</span></span>  | <span data-ttu-id="547fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="547fa-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="547fa-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="547fa-123">Content-Type</span></span>   | <span data-ttu-id="547fa-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="547fa-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="547fa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="547fa-126">Request body</span></span>

<span data-ttu-id="547fa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="547fa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="547fa-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="547fa-128">Response</span></span>

<span data-ttu-id="547fa-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="547fa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="547fa-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="547fa-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="547fa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="547fa-132">Request</span></span>

<span data-ttu-id="547fa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="547fa-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="547fa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="547fa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_skillproficiency"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/skills/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="547fa-135">C#</span><span class="sxs-lookup"><span data-stu-id="547fa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="547fa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="547fa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="547fa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="547fa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="547fa-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="547fa-138">Response</span></span>

<span data-ttu-id="547fa-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="547fa-139">The following is an example of the response.</span></span>

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
  "description": "Delete skillProficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
