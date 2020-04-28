---
title: Удаление пользователя — API Microsoft Graph
description: Описан метод удаления ресурса (объекта) user из API Microsoft Graph (REST).
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2eb2a971ebca944c11379d0250fb89786a80fa4c
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107908"
---
# <a name="delete-a-user"></a><span data-ttu-id="6e659-103">Удалить пользователя</span><span class="sxs-lookup"><span data-stu-id="6e659-103">Delete a user</span></span>

<span data-ttu-id="6e659-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e659-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e659-105">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e659-105">Delete user.</span></span>  

<span data-ttu-id="6e659-106">При удалении ресурсы user перемещаются во временный контейнер, и их можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="6e659-106">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="6e659-107">По истечении этого периода они удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="6e659-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="6e659-108">Дополнительные сведения см. в статье [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="6e659-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e659-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e659-109">Permissions</span></span>

<span data-ttu-id="6e659-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e659-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e659-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e659-112">Permission type</span></span>      | <span data-ttu-id="6e659-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e659-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e659-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e659-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6e659-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e659-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e659-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e659-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e659-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e659-117">Not supported.</span></span>    |
|<span data-ttu-id="6e659-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e659-118">Application</span></span> | <span data-ttu-id="6e659-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e659-119">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e659-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e659-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="6e659-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e659-121">Request headers</span></span>

| <span data-ttu-id="6e659-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e659-122">Header</span></span>       | <span data-ttu-id="6e659-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6e659-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="6e659-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e659-124">Authorization</span></span>  | <span data-ttu-id="6e659-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e659-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e659-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e659-127">Request body</span></span>

<span data-ttu-id="6e659-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e659-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e659-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e659-129">Response</span></span>

<span data-ttu-id="6e659-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6e659-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e659-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6e659-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e659-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e659-133">Request</span></span>

<span data-ttu-id="6e659-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e659-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e659-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e659-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
# <a name="c"></a>[<span data-ttu-id="6e659-136">C#</span><span class="sxs-lookup"><span data-stu-id="6e659-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e659-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e659-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e659-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e659-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6e659-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e659-139">Response</span></span>

<span data-ttu-id="6e659-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6e659-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
