---
title: Удаление personAnnotation
description: Удаляет объект personAnnotation.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 16993d5919c0d588710ac2835cc2bd0f4f46a1a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774217"
---
# <a name="delete-personannotation"></a><span data-ttu-id="3c849-103">Удаление personAnnotation</span><span class="sxs-lookup"><span data-stu-id="3c849-103">Delete personAnnotation</span></span>
<span data-ttu-id="3c849-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c849-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c849-105">Удаляет объект [personAnnotation](../resources/personannotation.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="3c849-105">Deletes a [personAnnotation](../resources/personannotation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c849-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c849-106">Permissions</span></span>

<span data-ttu-id="3c849-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c849-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c849-109">Permission type</span></span>                        | <span data-ttu-id="3c849-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c849-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="3c849-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c849-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c849-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c849-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="3c849-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c849-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c849-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c849-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="3c849-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3c849-115">Application</span></span>                            | <span data-ttu-id="3c849-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c849-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="3c849-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c849-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/notes/{id}
DELETE /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3c849-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c849-118">Request headers</span></span>
|<span data-ttu-id="3c849-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3c849-119">Name</span></span>|<span data-ttu-id="3c849-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3c849-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c849-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c849-121">Authorization</span></span>|<span data-ttu-id="3c849-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c849-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c849-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c849-124">Request body</span></span>
<span data-ttu-id="3c849-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c849-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c849-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c849-126">Response</span></span>

<span data-ttu-id="3c849-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3c849-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3c849-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3c849-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c849-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c849-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="3c849-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c849-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personannotation"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/notes/{id}
```
# <a name="c"></a>[<span data-ttu-id="3c849-131">C#</span><span class="sxs-lookup"><span data-stu-id="3c849-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personannotation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c849-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c849-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personannotation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c849-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c849-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personannotation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c849-134">Java</span><span class="sxs-lookup"><span data-stu-id="3c849-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-personannotation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3c849-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c849-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


