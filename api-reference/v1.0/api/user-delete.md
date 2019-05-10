---
title: Удаление пользователя — API Microsoft Graph
description: Описан метод удаления ресурса (объекта) user из API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d275f6e99e9ff22d156d4d6725872cf160716513
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602226"
---
# <a name="delete-a-user"></a><span data-ttu-id="b9ee4-103">Удалить пользователя</span><span class="sxs-lookup"><span data-stu-id="b9ee4-103">Delete a user</span></span>

<span data-ttu-id="b9ee4-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-104">Delete user.</span></span>  

<span data-ttu-id="b9ee4-105">При удалении ресурсы user перемещаются во временный контейнер, и их можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="b9ee4-106">По истечении этого периода они удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="b9ee4-107">Дополнительные сведения см. в статье [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="b9ee4-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9ee4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9ee4-108">Permissions</span></span>

<span data-ttu-id="b9ee4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9ee4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9ee4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9ee4-111">Permission type</span></span>      | <span data-ttu-id="b9ee4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9ee4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9ee4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9ee4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b9ee4-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9ee4-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9ee4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9ee4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9ee4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-116">Not supported.</span></span>    |
|<span data-ttu-id="b9ee4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9ee4-117">Application</span></span> | <span data-ttu-id="b9ee4-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9ee4-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9ee4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9ee4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="b9ee4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9ee4-120">Request headers</span></span>

| <span data-ttu-id="b9ee4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9ee4-121">Header</span></span>       | <span data-ttu-id="b9ee4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9ee4-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b9ee4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9ee4-123">Authorization</span></span>  | <span data-ttu-id="b9ee4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9ee4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9ee4-126">Request body</span></span>

<span data-ttu-id="b9ee4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9ee4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9ee4-128">Response</span></span>

<span data-ttu-id="b9ee4-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9ee4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b9ee4-131">Example</span></span>

## <a name="request"></a><span data-ttu-id="b9ee4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9ee4-132">Request</span></span>

<span data-ttu-id="b9ee4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
### <a name="response"></a><span data-ttu-id="b9ee4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9ee4-134">Response</span></span>

<span data-ttu-id="b9ee4-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9ee4-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b9ee4-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b9ee4-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b9ee4-137">C#</span><span class="sxs-lookup"><span data-stu-id="b9ee4-137">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9ee4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9ee4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
