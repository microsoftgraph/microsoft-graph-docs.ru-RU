---
title: Удаление Персонавард
description: Удаляет объект Персонавард.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ec8358fb1015e2816818b28a887a6e7a8c2f9a48
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969349"
---
# <a name="delete-personaward"></a><span data-ttu-id="37c08-103">Удаление Персонавард</span><span class="sxs-lookup"><span data-stu-id="37c08-103">Delete personAward</span></span>

<span data-ttu-id="37c08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37c08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37c08-105">Удаляет объект [персонавард](../resources/personaward.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="37c08-105">Deletes a [personAward](../resources/personaward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37c08-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37c08-106">Permissions</span></span>

<span data-ttu-id="37c08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37c08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37c08-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37c08-109">Permission type</span></span>                        | <span data-ttu-id="37c08-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37c08-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="37c08-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37c08-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37c08-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="37c08-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="37c08-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37c08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37c08-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="37c08-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="37c08-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37c08-115">Application</span></span>                            | <span data-ttu-id="37c08-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c08-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="37c08-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37c08-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/awards/{id}
DELETE /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="request-headers"></a><span data-ttu-id="37c08-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37c08-118">Request headers</span></span>
|<span data-ttu-id="37c08-119">Имя</span><span class="sxs-lookup"><span data-stu-id="37c08-119">Name</span></span>|<span data-ttu-id="37c08-120">Описание</span><span class="sxs-lookup"><span data-stu-id="37c08-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37c08-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37c08-121">Authorization</span></span>|<span data-ttu-id="37c08-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37c08-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37c08-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37c08-124">Request body</span></span>
<span data-ttu-id="37c08-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37c08-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37c08-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="37c08-126">Response</span></span>

<span data-ttu-id="37c08-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="37c08-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="37c08-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="37c08-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37c08-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="37c08-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="37c08-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c08-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personaward"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/awards/{personAwardId}
```
# <a name="c"></a>[<span data-ttu-id="37c08-131">C#</span><span class="sxs-lookup"><span data-stu-id="37c08-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c08-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c08-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c08-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c08-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="37c08-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="37c08-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


