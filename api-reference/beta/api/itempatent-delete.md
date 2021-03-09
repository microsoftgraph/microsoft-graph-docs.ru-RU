---
title: Удаление itemPatent
description: Удаляет объект itemPatent.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6a5045c4c9c2cd95bee5534b86e99c2d4fba5202
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577438"
---
# <a name="delete-itempatent"></a><span data-ttu-id="74871-103">Удаление itemPatent</span><span class="sxs-lookup"><span data-stu-id="74871-103">Delete itemPatent</span></span>

<span data-ttu-id="74871-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74871-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74871-105">Удаляет объект [itemPatent.](../resources/itempatent.md)</span><span class="sxs-lookup"><span data-stu-id="74871-105">Deletes an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74871-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74871-106">Permissions</span></span>

<span data-ttu-id="74871-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74871-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74871-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74871-109">Permission type</span></span>                        | <span data-ttu-id="74871-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74871-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="74871-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74871-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="74871-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74871-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="74871-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74871-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74871-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74871-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="74871-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74871-115">Application</span></span>                            | <span data-ttu-id="74871-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74871-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="74871-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74871-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/patents/{id}
DELETE /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="74871-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74871-118">Request headers</span></span>
|<span data-ttu-id="74871-119">Имя</span><span class="sxs-lookup"><span data-stu-id="74871-119">Name</span></span>|<span data-ttu-id="74871-120">Описание</span><span class="sxs-lookup"><span data-stu-id="74871-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="74871-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74871-121">Authorization</span></span>|<span data-ttu-id="74871-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74871-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74871-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74871-124">Request body</span></span>
<span data-ttu-id="74871-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74871-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74871-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="74871-126">Response</span></span>

<span data-ttu-id="74871-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="74871-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="74871-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="74871-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74871-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="74871-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="74871-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="74871-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itempatent"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="74871-131">C#</span><span class="sxs-lookup"><span data-stu-id="74871-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74871-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74871-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74871-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74871-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="74871-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="74871-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


