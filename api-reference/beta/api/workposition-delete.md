---
title: Удаление Воркпоситион
description: Удаление объекта Воркпоситион из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 372c1518a7c7c6e63d0671b13175b75418003b1d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977380"
---
# <a name="delete-workposition"></a><span data-ttu-id="52f55-103">Удаление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="52f55-103">Delete workPosition</span></span>

<span data-ttu-id="52f55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52f55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52f55-105">Удаление определенного объекта [воркпоситион](../resources/workposition.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="52f55-105">Delete a specific [workPosition](../resources/workposition.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="52f55-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52f55-106">Permissions</span></span>

<span data-ttu-id="52f55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52f55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52f55-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52f55-109">Permission type</span></span>                        | <span data-ttu-id="52f55-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52f55-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52f55-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52f55-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="52f55-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="52f55-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="52f55-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52f55-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52f55-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="52f55-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="52f55-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52f55-115">Application</span></span>                            | <span data-ttu-id="52f55-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52f55-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="52f55-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52f55-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/positions/{id}
DELETE /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="52f55-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52f55-118">Request headers</span></span>

| <span data-ttu-id="52f55-119">Имя</span><span class="sxs-lookup"><span data-stu-id="52f55-119">Name</span></span>           |<span data-ttu-id="52f55-120">Описание</span><span class="sxs-lookup"><span data-stu-id="52f55-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="52f55-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52f55-121">Authorization</span></span>  | <span data-ttu-id="52f55-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52f55-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="52f55-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52f55-124">Content-Type</span></span>   | <span data-ttu-id="52f55-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52f55-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="52f55-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52f55-127">Request body</span></span>

<span data-ttu-id="52f55-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52f55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52f55-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="52f55-129">Response</span></span>

<span data-ttu-id="52f55-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="52f55-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52f55-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="52f55-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52f55-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="52f55-133">Request</span></span>

<span data-ttu-id="52f55-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52f55-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52f55-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="52f55-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workposition"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/positions/{id}
```
# <a name="c"></a>[<span data-ttu-id="52f55-136">C#</span><span class="sxs-lookup"><span data-stu-id="52f55-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52f55-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52f55-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52f55-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f55-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52f55-139">Java</span><span class="sxs-lookup"><span data-stu-id="52f55-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-workposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52f55-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="52f55-140">Response</span></span>

<span data-ttu-id="52f55-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="52f55-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


