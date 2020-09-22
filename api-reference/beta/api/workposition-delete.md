---
title: Удаление Воркпоситион
description: Удаление объекта Воркпоситион из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d11a4f12e4b0837ab6a18c56eb4547872ba8563f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092955"
---
# <a name="delete-workposition"></a><span data-ttu-id="0e42b-103">Удаление Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="0e42b-103">Delete workPosition</span></span>

<span data-ttu-id="0e42b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e42b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e42b-105">Удаление определенного объекта [воркпоситион](../resources/workposition.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e42b-105">Delete a specific [workPosition](../resources/workposition.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e42b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e42b-106">Permissions</span></span>

<span data-ttu-id="0e42b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e42b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e42b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e42b-109">Permission type</span></span>                        | <span data-ttu-id="0e42b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e42b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e42b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e42b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e42b-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0e42b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0e42b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e42b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e42b-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0e42b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0e42b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e42b-115">Application</span></span>                            | <span data-ttu-id="0e42b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e42b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0e42b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e42b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/positions/{id}
DELETE /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e42b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e42b-118">Request headers</span></span>

| <span data-ttu-id="0e42b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0e42b-119">Name</span></span>           |<span data-ttu-id="0e42b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0e42b-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0e42b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e42b-121">Authorization</span></span>  | <span data-ttu-id="0e42b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e42b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0e42b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e42b-124">Content-Type</span></span>   | <span data-ttu-id="0e42b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e42b-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0e42b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e42b-127">Request body</span></span>

<span data-ttu-id="0e42b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e42b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e42b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e42b-129">Response</span></span>

<span data-ttu-id="0e42b-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0e42b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e42b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="0e42b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e42b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e42b-133">Request</span></span>

<span data-ttu-id="0e42b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e42b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e42b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e42b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workposition"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/positions/{id}
```
# <a name="c"></a>[<span data-ttu-id="0e42b-136">C#</span><span class="sxs-lookup"><span data-stu-id="0e42b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e42b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e42b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e42b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e42b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e42b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e42b-139">Response</span></span>

<span data-ttu-id="0e42b-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0e42b-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


