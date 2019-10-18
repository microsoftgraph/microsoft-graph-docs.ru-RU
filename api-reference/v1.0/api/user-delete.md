---
title: Удаление пользователя — API Microsoft Graph
description: Описан метод удаления ресурса (объекта) user из API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f7ef2f0b067b4d240340172f113e4878edbb4537
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373681"
---
# <a name="delete-a-user"></a><span data-ttu-id="730a5-103">Удалить пользователя</span><span class="sxs-lookup"><span data-stu-id="730a5-103">Delete a user</span></span>

<span data-ttu-id="730a5-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="730a5-104">Delete user.</span></span>  

<span data-ttu-id="730a5-105">При удалении ресурсы user перемещаются во временный контейнер, и их можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="730a5-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="730a5-106">По истечении этого периода они удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="730a5-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="730a5-107">Дополнительные сведения см. в статье [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="730a5-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="730a5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="730a5-108">Permissions</span></span>

<span data-ttu-id="730a5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="730a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="730a5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="730a5-111">Permission type</span></span>      | <span data-ttu-id="730a5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="730a5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="730a5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="730a5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="730a5-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="730a5-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="730a5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="730a5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="730a5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="730a5-116">Not supported.</span></span>    |
|<span data-ttu-id="730a5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="730a5-117">Application</span></span> | <span data-ttu-id="730a5-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="730a5-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="730a5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="730a5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="730a5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="730a5-120">Request headers</span></span>

| <span data-ttu-id="730a5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="730a5-121">Header</span></span>       | <span data-ttu-id="730a5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="730a5-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="730a5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="730a5-123">Authorization</span></span>  | <span data-ttu-id="730a5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="730a5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="730a5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="730a5-126">Request body</span></span>

<span data-ttu-id="730a5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="730a5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="730a5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="730a5-128">Response</span></span>

<span data-ttu-id="730a5-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="730a5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="730a5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="730a5-131">Example</span></span>

## <a name="request"></a><span data-ttu-id="730a5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="730a5-132">Request</span></span>

<span data-ttu-id="730a5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="730a5-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="730a5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="730a5-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="730a5-135">C#</span><span class="sxs-lookup"><span data-stu-id="730a5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="730a5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="730a5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="730a5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="730a5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="730a5-138">Java</span><span class="sxs-lookup"><span data-stu-id="730a5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="730a5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="730a5-139">Response</span></span>

<span data-ttu-id="730a5-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="730a5-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
