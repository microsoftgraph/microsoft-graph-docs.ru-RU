---
title: Удаление outlookTask
description: Удаление указанной задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 76aab2a7598ad380c5b1841428a5b0740c07d662
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988708"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="d18e5-103">Удаление outlookTask</span><span class="sxs-lookup"><span data-stu-id="d18e5-103">Delete outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d18e5-104">Удаление указанной задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="d18e5-104">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="d18e5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d18e5-105">Permissions</span></span>

<span data-ttu-id="d18e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d18e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d18e5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d18e5-108">Permission type</span></span>      | <span data-ttu-id="d18e5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d18e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d18e5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d18e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d18e5-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d18e5-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d18e5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d18e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d18e5-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d18e5-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d18e5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d18e5-114">Application</span></span> | <span data-ttu-id="d18e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d18e5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d18e5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d18e5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d18e5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d18e5-117">Request headers</span></span>

| <span data-ttu-id="d18e5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d18e5-118">Name</span></span>       | <span data-ttu-id="d18e5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d18e5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d18e5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d18e5-120">Authorization</span></span>  | <span data-ttu-id="d18e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d18e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d18e5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d18e5-123">Request body</span></span>

<span data-ttu-id="d18e5-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d18e5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d18e5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d18e5-125">Response</span></span>

<span data-ttu-id="d18e5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d18e5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d18e5-128">Пример</span><span class="sxs-lookup"><span data-stu-id="d18e5-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="d18e5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d18e5-129">Request</span></span>

<span data-ttu-id="d18e5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d18e5-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d18e5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d18e5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d18e5-132">C#</span><span class="sxs-lookup"><span data-stu-id="d18e5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d18e5-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d18e5-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d18e5-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d18e5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d18e5-135">Java</span><span class="sxs-lookup"><span data-stu-id="d18e5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d18e5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d18e5-136">Response</span></span>

<span data-ttu-id="d18e5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d18e5-137">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
