---
title: Удаление Едукатионалактивити
description: Удаление объекта Едукатионалактивити из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ad9cc4f842e9d4cf4402d70d515a109279b1f92d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966684"
---
# <a name="delete-educationalactivity"></a><span data-ttu-id="3a441-103">Удаление Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="3a441-103">Delete educationalActivity</span></span>

<span data-ttu-id="3a441-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a441-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a441-105">Удаление объекта [едукатионалактивити](../resources/educationalactivity.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="3a441-105">Delete an [educationalActivity](../resources/educationalactivity.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3a441-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a441-106">Permissions</span></span>

<span data-ttu-id="3a441-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a441-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a441-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a441-109">Permission type</span></span>                        | <span data-ttu-id="3a441-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a441-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3a441-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a441-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a441-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3a441-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3a441-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a441-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a441-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3a441-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3a441-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a441-115">Application</span></span>                            | <span data-ttu-id="3a441-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a441-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3a441-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a441-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/educationalActivities/{id} 
DELETE /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3a441-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a441-118">Request headers</span></span>

| <span data-ttu-id="3a441-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3a441-119">Name</span></span>           |<span data-ttu-id="3a441-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3a441-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="3a441-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a441-121">Authorization</span></span>  | <span data-ttu-id="3a441-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a441-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="3a441-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a441-124">Request body</span></span>

<span data-ttu-id="3a441-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a441-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a441-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a441-126">Response</span></span>

<span data-ttu-id="3a441-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a441-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a441-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a441-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a441-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a441-130">Request</span></span>

<span data-ttu-id="3a441-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a441-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a441-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a441-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationalactivity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```
# <a name="c"></a>[<span data-ttu-id="3a441-133">C#</span><span class="sxs-lookup"><span data-stu-id="3a441-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a441-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a441-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a441-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a441-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a441-136">Java</span><span class="sxs-lookup"><span data-stu-id="3a441-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationalactivity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a441-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a441-137">Response</span></span>

<span data-ttu-id="3a441-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3a441-138">The following is an example of the response.</span></span>

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
  "description": "Delete educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


