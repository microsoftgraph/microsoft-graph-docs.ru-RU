---
title: Удаление СкиллпрофиЦиенци
description: Удаление СкиллпрофиЦиенци.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 20ec502730358d59c02491ff6f299cb6f4bcb9ce
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973166"
---
# <a name="delete-skillproficiency"></a><span data-ttu-id="2c4bf-103">Удаление СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="2c4bf-103">Delete skillProficiency</span></span>

<span data-ttu-id="2c4bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c4bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c4bf-105">Удаление объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c4bf-105">Delete a [skillProficiency](../resources/skillproficiency.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c4bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c4bf-106">Permissions</span></span>

<span data-ttu-id="2c4bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c4bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c4bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c4bf-109">Permission type</span></span>                        | <span data-ttu-id="2c4bf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c4bf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c4bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c4bf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c4bf-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2c4bf-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2c4bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c4bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c4bf-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2c4bf-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="2c4bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c4bf-115">Application</span></span>                            | <span data-ttu-id="2c4bf-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c4bf-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="2c4bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c4bf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/skills/{id}
DELETE /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2c4bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c4bf-118">Request headers</span></span>

| <span data-ttu-id="2c4bf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2c4bf-119">Name</span></span>           |<span data-ttu-id="2c4bf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2c4bf-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="2c4bf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c4bf-121">Authorization</span></span>  | <span data-ttu-id="2c4bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c4bf-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2c4bf-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c4bf-124">Content-Type</span></span>   | <span data-ttu-id="2c4bf-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c4bf-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2c4bf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c4bf-127">Request body</span></span>

<span data-ttu-id="2c4bf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c4bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c4bf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c4bf-129">Response</span></span>

<span data-ttu-id="2c4bf-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2c4bf-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c4bf-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2c4bf-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2c4bf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c4bf-133">Request</span></span>

<span data-ttu-id="2c4bf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c4bf-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c4bf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c4bf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_skillproficiency"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/skills/{id}
```
# <a name="c"></a>[<span data-ttu-id="2c4bf-136">C#</span><span class="sxs-lookup"><span data-stu-id="2c4bf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c4bf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c4bf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c4bf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c4bf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c4bf-139">Java</span><span class="sxs-lookup"><span data-stu-id="2c4bf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-skillproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2c4bf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c4bf-140">Response</span></span>

<span data-ttu-id="2c4bf-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2c4bf-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


