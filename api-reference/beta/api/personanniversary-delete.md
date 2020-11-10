---
title: Удаление Персонанниверсари
description: Удаление объекта Персонанниверсари из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c23e51d89023ce5cb5442cf4267d1733ceffc241
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968504"
---
# <a name="delete-personanniversary"></a><span data-ttu-id="2e5a0-103">Удаление Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="2e5a0-103">Delete personAnniversary</span></span>

<span data-ttu-id="2e5a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e5a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e5a0-105">Удаление объекта [персонанниверсари](../resources/personanniversary.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="2e5a0-105">Delete a [personAnniversary](../resources/personanniversary.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e5a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e5a0-106">Permissions</span></span>

<span data-ttu-id="2e5a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e5a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e5a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e5a0-109">Permission type</span></span>                        | <span data-ttu-id="2e5a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e5a0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e5a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e5a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e5a0-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2e5a0-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2e5a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e5a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e5a0-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2e5a0-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2e5a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e5a0-115">Application</span></span>                            | <span data-ttu-id="2e5a0-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5a0-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="2e5a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e5a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/anniversaries/{id}
DELETE /users/{id | userPrincipalName}/profile/anniversaries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e5a0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e5a0-118">Request headers</span></span>

| <span data-ttu-id="2e5a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2e5a0-119">Name</span></span>           |<span data-ttu-id="2e5a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2e5a0-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="2e5a0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e5a0-121">Authorization</span></span>  | <span data-ttu-id="2e5a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e5a0-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="2e5a0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e5a0-124">Request body</span></span>

<span data-ttu-id="2e5a0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e5a0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e5a0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e5a0-126">Response</span></span>

<span data-ttu-id="2e5a0-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2e5a0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e5a0-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e5a0-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e5a0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e5a0-130">Request</span></span>

<span data-ttu-id="2e5a0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e5a0-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e5a0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e5a0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personanniversary"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
```
# <a name="c"></a>[<span data-ttu-id="2e5a0-133">C#</span><span class="sxs-lookup"><span data-stu-id="2e5a0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e5a0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e5a0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e5a0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e5a0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e5a0-136">Java</span><span class="sxs-lookup"><span data-stu-id="2e5a0-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-personanniversary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2e5a0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e5a0-137">Response</span></span>

<span data-ttu-id="2e5a0-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e5a0-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


