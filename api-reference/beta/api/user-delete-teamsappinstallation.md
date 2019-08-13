---
title: Удаление приложения для пользователя
description: Удаление приложения из личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 39855619704d263b11fdc55b9794fcaa8b07aa2c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362492"
---
# <a name="uninstall-app-for-user"></a><span data-ttu-id="c9ad8-103">Удаление приложения для пользователя</span><span class="sxs-lookup"><span data-stu-id="c9ad8-103">Uninstall app for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9ad8-104">Удаление [приложения](../resources/teamsappinstallation.md) из личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c9ad8-104">Uninstall an [app](../resources/teamsappinstallation.md) from the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9ad8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9ad8-105">Permissions</span></span>

<span data-ttu-id="c9ad8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9ad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9ad8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9ad8-108">Permission type</span></span>      | <span data-ttu-id="c9ad8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9ad8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9ad8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9ad8-110">Delegated (work or school account)</span></span> |<span data-ttu-id="c9ad8-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9ad8-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9ad8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9ad8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9ad8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9ad8-113">Not supported.</span></span>    |
|<span data-ttu-id="c9ad8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9ad8-114">Application</span></span> | <span data-ttu-id="c9ad8-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9ad8-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c9ad8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9ad8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c9ad8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9ad8-117">Request headers</span></span>

| <span data-ttu-id="c9ad8-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9ad8-118">Header</span></span>       | <span data-ttu-id="c9ad8-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c9ad8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9ad8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9ad8-120">Authorization</span></span>  | <span data-ttu-id="c9ad8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9ad8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9ad8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9ad8-123">Request body</span></span>

<span data-ttu-id="c9ad8-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9ad8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9ad8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9ad8-125">Response</span></span>

<span data-ttu-id="c9ad8-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9ad8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9ad8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c9ad8-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9ad8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9ad8-129">Request</span></span>

<span data-ttu-id="c9ad8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9ad8-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9ad8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9ad8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delete_teamsApp"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9ad8-132">C#</span><span class="sxs-lookup"><span data-stu-id="c9ad8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9ad8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9ad8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9ad8-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c9ad8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9ad8-135">Java</span><span class="sxs-lookup"><span data-stu-id="c9ad8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c9ad8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9ad8-136">Response</span></span>

<span data-ttu-id="c9ad8-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c9ad8-137">The following is an example of the response.</span></span>

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
  "description": "User delete teamsAppInstallations,
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
