---
title: Удаление personCertification
description: Удаляет объект personCertification.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6a6c1493496fdfca68c1282091ebe2092f0683be
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774077"
---
# <a name="delete-personcertification"></a><span data-ttu-id="ba828-103">Удаление personCertification</span><span class="sxs-lookup"><span data-stu-id="ba828-103">Delete personCertification</span></span>
<span data-ttu-id="ba828-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba828-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba828-105">Удаляет объект [personCertification](../resources/personcertification.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="ba828-105">Deletes a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba828-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba828-106">Permissions</span></span>

<span data-ttu-id="ba828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba828-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba828-109">Permission type</span></span>                        | <span data-ttu-id="ba828-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba828-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ba828-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba828-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba828-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba828-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ba828-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba828-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba828-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba828-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ba828-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba828-115">Application</span></span>                            | <span data-ttu-id="ba828-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba828-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="ba828-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba828-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/certifications/{id}
DELETE /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba828-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba828-118">Request headers</span></span>
|<span data-ttu-id="ba828-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ba828-119">Name</span></span>|<span data-ttu-id="ba828-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ba828-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba828-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba828-121">Authorization</span></span>|<span data-ttu-id="ba828-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba828-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba828-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba828-124">Request body</span></span>
<span data-ttu-id="ba828-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba828-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba828-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba828-126">Response</span></span>

<span data-ttu-id="ba828-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba828-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ba828-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba828-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba828-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba828-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="ba828-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba828-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personCertification"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/certifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="ba828-131">C#</span><span class="sxs-lookup"><span data-stu-id="ba828-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personcertification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba828-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba828-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personcertification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba828-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba828-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personcertification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba828-134">Java</span><span class="sxs-lookup"><span data-stu-id="ba828-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-personcertification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ba828-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba828-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


