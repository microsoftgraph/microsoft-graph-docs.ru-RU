---
title: Удаление Итемпатент
description: Удаляет объект Итемпатент.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1721797203410eab2fee7ff46970e1da36d8047f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090003"
---
# <a name="delete-itempatent"></a><span data-ttu-id="f4941-103">Удаление Итемпатент</span><span class="sxs-lookup"><span data-stu-id="f4941-103">Delete itemPatent</span></span>

<span data-ttu-id="f4941-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4941-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4941-105">Удаляет объект [итемпатент](../resources/itempatent.md) .</span><span class="sxs-lookup"><span data-stu-id="f4941-105">Deletes an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4941-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4941-106">Permissions</span></span>

<span data-ttu-id="f4941-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4941-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4941-109">Permission type</span></span>                        | <span data-ttu-id="f4941-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4941-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f4941-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4941-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4941-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f4941-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f4941-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4941-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4941-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f4941-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f4941-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4941-115">Application</span></span>                            | <span data-ttu-id="f4941-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4941-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f4941-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4941-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/patents/{id}
DELETE /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f4941-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4941-118">Request headers</span></span>
|<span data-ttu-id="f4941-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f4941-119">Name</span></span>|<span data-ttu-id="f4941-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4941-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f4941-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4941-121">Authorization</span></span>|<span data-ttu-id="f4941-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4941-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4941-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4941-124">Request body</span></span>
<span data-ttu-id="f4941-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4941-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4941-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4941-126">Response</span></span>

<span data-ttu-id="f4941-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4941-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f4941-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f4941-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4941-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4941-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="f4941-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4941-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itempatent"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="f4941-131">C#</span><span class="sxs-lookup"><span data-stu-id="f4941-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4941-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4941-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4941-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4941-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f4941-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4941-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


