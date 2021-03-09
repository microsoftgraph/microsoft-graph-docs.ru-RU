---
title: Удаление itemAddress
description: Удаляет объект itemAddress.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ede930a2f76c09ea0b469a6b449b92275abbac28
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578712"
---
# <a name="delete-itemaddress"></a><span data-ttu-id="34fcc-103">Удаление itemAddress</span><span class="sxs-lookup"><span data-stu-id="34fcc-103">Delete itemAddress</span></span>
<span data-ttu-id="34fcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34fcc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34fcc-105">Удаляет объект [itemAddress.](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="34fcc-105">Deletes an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="34fcc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34fcc-106">Permissions</span></span>

<span data-ttu-id="34fcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34fcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34fcc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34fcc-109">Permission type</span></span>                        | <span data-ttu-id="34fcc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34fcc-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="34fcc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34fcc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="34fcc-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34fcc-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="34fcc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34fcc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34fcc-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34fcc-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="34fcc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34fcc-115">Application</span></span>                            | <span data-ttu-id="34fcc-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34fcc-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="34fcc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34fcc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/addresses/{id}
DELETE /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="request-headers"></a><span data-ttu-id="34fcc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34fcc-118">Request headers</span></span>
|<span data-ttu-id="34fcc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="34fcc-119">Name</span></span>|<span data-ttu-id="34fcc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="34fcc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="34fcc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34fcc-121">Authorization</span></span>|<span data-ttu-id="34fcc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34fcc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34fcc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34fcc-124">Request body</span></span>
<span data-ttu-id="34fcc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34fcc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34fcc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="34fcc-126">Response</span></span>

<span data-ttu-id="34fcc-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="34fcc-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="34fcc-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="34fcc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="34fcc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="34fcc-129">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="34fcc-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="34fcc-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemaddress"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/addresses/{id}
```
# <a name="c"></a>[<span data-ttu-id="34fcc-131">C#</span><span class="sxs-lookup"><span data-stu-id="34fcc-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34fcc-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34fcc-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34fcc-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34fcc-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="34fcc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="34fcc-134">Response</span></span>
<span data-ttu-id="34fcc-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="34fcc-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


