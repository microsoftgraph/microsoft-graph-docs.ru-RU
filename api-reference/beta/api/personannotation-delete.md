---
title: Удаление Персонаннотатион
description: Удаляет объект Персонаннотатион.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5f9bf692b7e386ca47042ee763fa0d9e57f86fea
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809742"
---
# <a name="delete-personannotation"></a><span data-ttu-id="62ba7-103">Удаление Персонаннотатион</span><span class="sxs-lookup"><span data-stu-id="62ba7-103">Delete personAnnotation</span></span>
<span data-ttu-id="62ba7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62ba7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62ba7-105">Удаляет объект [персонаннотатион](../resources/personannotation.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="62ba7-105">Deletes a [personAnnotation](../resources/personannotation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="62ba7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62ba7-106">Permissions</span></span>

<span data-ttu-id="62ba7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62ba7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62ba7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62ba7-109">Permission type</span></span>                        | <span data-ttu-id="62ba7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62ba7-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="62ba7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62ba7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62ba7-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="62ba7-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="62ba7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62ba7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62ba7-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="62ba7-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="62ba7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="62ba7-115">Application</span></span>                            | <span data-ttu-id="62ba7-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="62ba7-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="62ba7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62ba7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/notes/{id}
DELETE /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="62ba7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62ba7-118">Request headers</span></span>
|<span data-ttu-id="62ba7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="62ba7-119">Name</span></span>|<span data-ttu-id="62ba7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="62ba7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="62ba7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62ba7-121">Authorization</span></span>|<span data-ttu-id="62ba7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62ba7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62ba7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62ba7-124">Request body</span></span>
<span data-ttu-id="62ba7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62ba7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62ba7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="62ba7-126">Response</span></span>

<span data-ttu-id="62ba7-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="62ba7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="62ba7-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="62ba7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62ba7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="62ba7-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="62ba7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="62ba7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personannotation"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/notes/{id}
```
# <a name="c"></a>[<span data-ttu-id="62ba7-131">C#</span><span class="sxs-lookup"><span data-stu-id="62ba7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62ba7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62ba7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62ba7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62ba7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="62ba7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="62ba7-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
