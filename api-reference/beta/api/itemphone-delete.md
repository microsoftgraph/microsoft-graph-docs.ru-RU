---
title: Удаление itemPhone
description: Удаление объекта itemPhone из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 27aba7aa6a93918991f890bebdaad5ae7a2c69aa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776300"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="fd406-103">Удаление элементаPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="fd406-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="fd406-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd406-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd406-105">Удаление [объекта itemPhone](../resources/itemphone.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="fd406-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd406-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd406-106">Permissions</span></span>

<span data-ttu-id="fd406-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd406-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd406-109">Permission type</span></span>                        | <span data-ttu-id="fd406-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd406-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fd406-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd406-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd406-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd406-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fd406-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd406-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd406-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd406-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fd406-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd406-115">Application</span></span>                            | <span data-ttu-id="fd406-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd406-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="fd406-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd406-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/phones/{itemPhoneId}
DELETE /users/{userId}/profile/phones/{itemPhoneId}
```

## <a name="request-headers"></a><span data-ttu-id="fd406-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd406-118">Request headers</span></span>

|<span data-ttu-id="fd406-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fd406-119">Name</span></span>|<span data-ttu-id="fd406-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fd406-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fd406-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd406-121">Authorization</span></span>|<span data-ttu-id="fd406-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd406-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd406-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd406-124">Request body</span></span>

<span data-ttu-id="fd406-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd406-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd406-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd406-126">Response</span></span>

<span data-ttu-id="fd406-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fd406-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fd406-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="fd406-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd406-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd406-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fd406-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd406-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/users/{userId}/profile/phones/{itemPhoneId}
```
# <a name="c"></a>[<span data-ttu-id="fd406-131">C#</span><span class="sxs-lookup"><span data-stu-id="fd406-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd406-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd406-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd406-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd406-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd406-134">Java</span><span class="sxs-lookup"><span data-stu-id="fd406-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itemphone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fd406-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd406-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


