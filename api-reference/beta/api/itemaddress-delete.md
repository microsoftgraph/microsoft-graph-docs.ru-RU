---
title: Удаление itemAddress
description: Удаляет объект itemAddress.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1469633fd4cff278914bc4aa6cb6a757fd20c36f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774718"
---
# <a name="delete-itemaddress"></a><span data-ttu-id="e346b-103">Удаление itemAddress</span><span class="sxs-lookup"><span data-stu-id="e346b-103">Delete itemAddress</span></span>
<span data-ttu-id="e346b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e346b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e346b-105">Удаляет объект [itemAddress.](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="e346b-105">Deletes an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e346b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e346b-106">Permissions</span></span>

<span data-ttu-id="e346b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e346b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e346b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e346b-109">Permission type</span></span>                        | <span data-ttu-id="e346b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e346b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e346b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e346b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e346b-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e346b-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e346b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e346b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e346b-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e346b-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e346b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e346b-115">Application</span></span>                            | <span data-ttu-id="e346b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e346b-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e346b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e346b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/addresses/{id}
DELETE /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e346b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e346b-118">Request headers</span></span>
|<span data-ttu-id="e346b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e346b-119">Name</span></span>|<span data-ttu-id="e346b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e346b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e346b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e346b-121">Authorization</span></span>|<span data-ttu-id="e346b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e346b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e346b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e346b-124">Request body</span></span>
<span data-ttu-id="e346b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e346b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e346b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e346b-126">Response</span></span>

<span data-ttu-id="e346b-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e346b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e346b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e346b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e346b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e346b-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="e346b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e346b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemaddress"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/addresses/{id}
```
# <a name="c"></a>[<span data-ttu-id="e346b-131">C#</span><span class="sxs-lookup"><span data-stu-id="e346b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itemaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e346b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e346b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itemaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e346b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e346b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itemaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e346b-134">Java</span><span class="sxs-lookup"><span data-stu-id="e346b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itemaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e346b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e346b-135">Response</span></span>
<span data-ttu-id="e346b-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e346b-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


