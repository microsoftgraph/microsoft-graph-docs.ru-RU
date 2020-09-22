---
title: Удаление outlookTask
description: Удаление указанной задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7b2dd31ee34a226e11a28c3b86ed144f84ea5900
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017444"
---
# <a name="delete-outlooktask-deprecated"></a><span data-ttu-id="dedaa-103">Delete outlookTask (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="dedaa-103">Delete outlookTask (deprecated)</span></span>

<span data-ttu-id="dedaa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dedaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="dedaa-105">Удаление указанной задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="dedaa-105">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="dedaa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dedaa-106">Permissions</span></span>

<span data-ttu-id="dedaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dedaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dedaa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dedaa-109">Permission type</span></span>      | <span data-ttu-id="dedaa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dedaa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dedaa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dedaa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dedaa-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dedaa-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dedaa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dedaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dedaa-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dedaa-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dedaa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dedaa-115">Application</span></span> | <span data-ttu-id="dedaa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dedaa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dedaa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dedaa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dedaa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dedaa-118">Request headers</span></span>

| <span data-ttu-id="dedaa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dedaa-119">Name</span></span>       | <span data-ttu-id="dedaa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dedaa-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dedaa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dedaa-121">Authorization</span></span>  | <span data-ttu-id="dedaa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dedaa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dedaa-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dedaa-124">Request body</span></span>

<span data-ttu-id="dedaa-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dedaa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dedaa-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="dedaa-126">Response</span></span>

<span data-ttu-id="dedaa-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dedaa-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dedaa-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dedaa-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="dedaa-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dedaa-130">Request</span></span>

<span data-ttu-id="dedaa-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dedaa-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dedaa-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dedaa-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```
# <a name="c"></a>[<span data-ttu-id="dedaa-133">C#</span><span class="sxs-lookup"><span data-stu-id="dedaa-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dedaa-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dedaa-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dedaa-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dedaa-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dedaa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dedaa-136">Response</span></span>

<span data-ttu-id="dedaa-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dedaa-137">Here is an example of the response.</span></span>
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


