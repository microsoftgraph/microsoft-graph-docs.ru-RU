---
title: Удаление Персонанниверсари
description: Удаление объекта Персонанниверсари из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: abbfc0fdabad6dcd43ce49a906b59573d3f585da
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807706"
---
# <a name="delete-personanniversary"></a><span data-ttu-id="93c57-103">Удаление Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="93c57-103">Delete personAnniversary</span></span>

<span data-ttu-id="93c57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93c57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93c57-105">Удаление объекта [персонанниверсари](../resources/personanniversary.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="93c57-105">Delete a [personAnniversary](../resources/personanniversary.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93c57-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93c57-106">Permissions</span></span>

<span data-ttu-id="93c57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93c57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93c57-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93c57-109">Permission type</span></span>                        | <span data-ttu-id="93c57-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93c57-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="93c57-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93c57-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="93c57-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="93c57-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="93c57-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93c57-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93c57-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="93c57-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="93c57-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93c57-115">Application</span></span>                            | <span data-ttu-id="93c57-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93c57-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="93c57-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93c57-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/anniversaries/{id}
DELETE /users/{id | userPrincipalName}/profile/anniversaries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93c57-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93c57-118">Request headers</span></span>

| <span data-ttu-id="93c57-119">Имя</span><span class="sxs-lookup"><span data-stu-id="93c57-119">Name</span></span>           |<span data-ttu-id="93c57-120">Описание</span><span class="sxs-lookup"><span data-stu-id="93c57-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="93c57-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93c57-121">Authorization</span></span>  | <span data-ttu-id="93c57-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93c57-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="93c57-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93c57-124">Request body</span></span>

<span data-ttu-id="93c57-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93c57-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93c57-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="93c57-126">Response</span></span>

<span data-ttu-id="93c57-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="93c57-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93c57-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="93c57-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93c57-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="93c57-130">Request</span></span>

<span data-ttu-id="93c57-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93c57-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93c57-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="93c57-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personanniversary"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
```
# <a name="c"></a>[<span data-ttu-id="93c57-133">C#</span><span class="sxs-lookup"><span data-stu-id="93c57-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93c57-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93c57-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93c57-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93c57-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="93c57-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="93c57-136">Response</span></span>

<span data-ttu-id="93c57-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="93c57-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
