---
title: Удаление outlookTask
description: Удаление указанной задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 23893cdf745ad20ede30298f9febd06e2b23a886
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456217"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="7afa0-103">Удаление outlookTask</span><span class="sxs-lookup"><span data-stu-id="7afa0-103">Delete outlookTask</span></span>

<span data-ttu-id="7afa0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7afa0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7afa0-105">Удаление указанной задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="7afa0-105">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="7afa0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7afa0-106">Permissions</span></span>

<span data-ttu-id="7afa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7afa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7afa0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7afa0-109">Permission type</span></span>      | <span data-ttu-id="7afa0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7afa0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7afa0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7afa0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7afa0-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7afa0-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7afa0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7afa0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7afa0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7afa0-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="7afa0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7afa0-115">Application</span></span> | <span data-ttu-id="7afa0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7afa0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7afa0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7afa0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7afa0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7afa0-118">Request headers</span></span>

| <span data-ttu-id="7afa0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7afa0-119">Name</span></span>       | <span data-ttu-id="7afa0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7afa0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7afa0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7afa0-121">Authorization</span></span>  | <span data-ttu-id="7afa0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7afa0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7afa0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7afa0-124">Request body</span></span>

<span data-ttu-id="7afa0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7afa0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7afa0-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="7afa0-126">Response</span></span>

<span data-ttu-id="7afa0-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7afa0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7afa0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7afa0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7afa0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7afa0-130">Request</span></span>

<span data-ttu-id="7afa0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7afa0-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7afa0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7afa0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```
# <a name="c"></a>[<span data-ttu-id="7afa0-133">C#</span><span class="sxs-lookup"><span data-stu-id="7afa0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7afa0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7afa0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7afa0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7afa0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7afa0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7afa0-136">Response</span></span>

<span data-ttu-id="7afa0-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7afa0-137">Here is an example of the response.</span></span>
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
