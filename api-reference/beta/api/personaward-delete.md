---
title: Удаление personAward
description: Удаляет объект personAward.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 83f1c3ee61d20edd25af9b66e40b91b62551efde
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50576031"
---
# <a name="delete-personaward"></a><span data-ttu-id="b8dd2-103">Удаление personAward</span><span class="sxs-lookup"><span data-stu-id="b8dd2-103">Delete personAward</span></span>

<span data-ttu-id="b8dd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8dd2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8dd2-105">Удаляет объект [personAward](../resources/personaward.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="b8dd2-105">Deletes a [personAward](../resources/personaward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8dd2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8dd2-106">Permissions</span></span>

<span data-ttu-id="b8dd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8dd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8dd2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8dd2-109">Permission type</span></span>                        | <span data-ttu-id="b8dd2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8dd2-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b8dd2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8dd2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8dd2-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8dd2-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b8dd2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8dd2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8dd2-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8dd2-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b8dd2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8dd2-115">Application</span></span>                            | <span data-ttu-id="b8dd2-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8dd2-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b8dd2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8dd2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/awards/{id}
DELETE /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b8dd2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8dd2-118">Request headers</span></span>
|<span data-ttu-id="b8dd2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b8dd2-119">Name</span></span>|<span data-ttu-id="b8dd2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b8dd2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b8dd2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8dd2-121">Authorization</span></span>|<span data-ttu-id="b8dd2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8dd2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8dd2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8dd2-124">Request body</span></span>
<span data-ttu-id="b8dd2-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8dd2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8dd2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8dd2-126">Response</span></span>

<span data-ttu-id="b8dd2-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8dd2-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b8dd2-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b8dd2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8dd2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8dd2-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="b8dd2-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8dd2-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personaward"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/awards/{personAwardId}
```
# <a name="c"></a>[<span data-ttu-id="b8dd2-131">C#</span><span class="sxs-lookup"><span data-stu-id="b8dd2-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8dd2-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8dd2-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8dd2-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8dd2-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b8dd2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8dd2-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


