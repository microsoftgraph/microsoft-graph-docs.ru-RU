---
title: Удаление itemPatent
description: Удаляет объект itemPatent.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4c819a4ca1bb50a572fbbe593a7ec951714cf4cc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776279"
---
# <a name="delete-itempatent"></a><span data-ttu-id="e6e0a-103">Удаление itemPatent</span><span class="sxs-lookup"><span data-stu-id="e6e0a-103">Delete itemPatent</span></span>

<span data-ttu-id="e6e0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6e0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6e0a-105">Удаляет объект [itemPatent.](../resources/itempatent.md)</span><span class="sxs-lookup"><span data-stu-id="e6e0a-105">Deletes an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6e0a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6e0a-106">Permissions</span></span>

<span data-ttu-id="e6e0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6e0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6e0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6e0a-109">Permission type</span></span>                        | <span data-ttu-id="e6e0a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6e0a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e6e0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6e0a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6e0a-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6e0a-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e6e0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6e0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6e0a-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6e0a-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e6e0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6e0a-115">Application</span></span>                            | <span data-ttu-id="e6e0a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6e0a-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e6e0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6e0a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/patents/{id}
DELETE /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e6e0a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6e0a-118">Request headers</span></span>
|<span data-ttu-id="e6e0a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e6e0a-119">Name</span></span>|<span data-ttu-id="e6e0a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e6e0a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e6e0a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6e0a-121">Authorization</span></span>|<span data-ttu-id="e6e0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6e0a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6e0a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6e0a-124">Request body</span></span>
<span data-ttu-id="e6e0a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6e0a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6e0a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6e0a-126">Response</span></span>

<span data-ttu-id="e6e0a-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6e0a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e6e0a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e6e0a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6e0a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6e0a-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="e6e0a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6e0a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itempatent"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="e6e0a-131">C#</span><span class="sxs-lookup"><span data-stu-id="e6e0a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itempatent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6e0a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6e0a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itempatent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6e0a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6e0a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itempatent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6e0a-134">Java</span><span class="sxs-lookup"><span data-stu-id="e6e0a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itempatent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e6e0a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6e0a-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


