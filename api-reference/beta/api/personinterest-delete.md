---
title: Удаление Персонинтерест
description: Удаление объекта Персонинтерест из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 74af9dab8e1ef5790a2aa9a53b251d0dcdf38a9c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972824"
---
# <a name="delete-personinterest"></a><span data-ttu-id="65d65-103">Удаление Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="65d65-103">Delete personInterest</span></span>

<span data-ttu-id="65d65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65d65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65d65-105">Удаляет объект [персонинтерест](../resources/personinterest.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="65d65-105">Deletes a [personInterest](../resources/personinterest.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65d65-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65d65-106">Permissions</span></span>

<span data-ttu-id="65d65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65d65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65d65-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65d65-109">Permission type</span></span>                        | <span data-ttu-id="65d65-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65d65-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="65d65-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65d65-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65d65-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="65d65-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="65d65-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65d65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65d65-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="65d65-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="65d65-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65d65-115">Application</span></span>                            | <span data-ttu-id="65d65-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d65-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="65d65-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65d65-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/interests/{id}
DELETE /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="65d65-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65d65-118">Request headers</span></span>

| <span data-ttu-id="65d65-119">Имя</span><span class="sxs-lookup"><span data-stu-id="65d65-119">Name</span></span>           |<span data-ttu-id="65d65-120">Описание</span><span class="sxs-lookup"><span data-stu-id="65d65-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="65d65-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65d65-121">Authorization</span></span>  | <span data-ttu-id="65d65-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65d65-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="65d65-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65d65-124">Request body</span></span>

<span data-ttu-id="65d65-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65d65-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65d65-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="65d65-126">Response</span></span>

<span data-ttu-id="65d65-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="65d65-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65d65-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="65d65-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65d65-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="65d65-130">Request</span></span>

<span data-ttu-id="65d65-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65d65-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65d65-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="65d65-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personinterest"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/interests/{id}
```
# <a name="c"></a>[<span data-ttu-id="65d65-133">C#</span><span class="sxs-lookup"><span data-stu-id="65d65-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65d65-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65d65-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65d65-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65d65-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65d65-136">Java</span><span class="sxs-lookup"><span data-stu-id="65d65-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-personinterest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65d65-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="65d65-137">Response</span></span>

<span data-ttu-id="65d65-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="65d65-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


