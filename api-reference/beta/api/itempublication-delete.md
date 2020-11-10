---
title: Удаление Итемпубликатион
description: Удаляет объект Итемпубликатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6e63ef86de454e63f6b90f4b9bf4ea79cfeb1222
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969897"
---
# <a name="delete-itempublication"></a><span data-ttu-id="9652d-103">Удаление Итемпубликатион</span><span class="sxs-lookup"><span data-stu-id="9652d-103">Delete itemPublication</span></span>

<span data-ttu-id="9652d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9652d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9652d-105">Удаляет объект [итемпубликатион](../resources/itempublication.md) .</span><span class="sxs-lookup"><span data-stu-id="9652d-105">Deletes an [itemPublication](../resources/itempublication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9652d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9652d-106">Permissions</span></span>

<span data-ttu-id="9652d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9652d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9652d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9652d-109">Permission type</span></span>                        | <span data-ttu-id="9652d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9652d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="9652d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9652d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9652d-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9652d-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9652d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9652d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9652d-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9652d-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9652d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9652d-115">Application</span></span>                            | <span data-ttu-id="9652d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9652d-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="9652d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9652d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/publications/{id}
DELETE /users/{id | userPrincipalName}/profile/publications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9652d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9652d-118">Request headers</span></span>
|<span data-ttu-id="9652d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9652d-119">Name</span></span>|<span data-ttu-id="9652d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9652d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9652d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9652d-121">Authorization</span></span>|<span data-ttu-id="9652d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9652d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9652d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9652d-124">Request body</span></span>
<span data-ttu-id="9652d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9652d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9652d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9652d-126">Response</span></span>

<span data-ttu-id="9652d-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9652d-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9652d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="9652d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9652d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9652d-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="9652d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9652d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemPublication"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/profile/publications/{id}
```
# <a name="c"></a>[<span data-ttu-id="9652d-131">C#</span><span class="sxs-lookup"><span data-stu-id="9652d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itempublication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9652d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9652d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itempublication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9652d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9652d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itempublication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9652d-134">Java</span><span class="sxs-lookup"><span data-stu-id="9652d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itempublication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9652d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9652d-135">Response</span></span>
<span data-ttu-id="9652d-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9652d-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


