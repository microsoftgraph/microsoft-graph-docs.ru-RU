---
title: Удаление outlookTask
description: Удаление указанной задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 42dbfd011b9bc0bd50ef91049767c27016f0d9b9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951571"
---
# <a name="delete-outlooktask-deprecated"></a><span data-ttu-id="f2f8b-103">Delete outlookTask (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="f2f8b-103">Delete outlookTask (deprecated)</span></span>

<span data-ttu-id="f2f8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="f2f8b-105">Удаление указанной задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2f8b-105">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2f8b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2f8b-106">Permissions</span></span>

<span data-ttu-id="f2f8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2f8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2f8b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2f8b-109">Permission type</span></span>      | <span data-ttu-id="f2f8b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2f8b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2f8b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2f8b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2f8b-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2f8b-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f2f8b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2f8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2f8b-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2f8b-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f2f8b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2f8b-115">Application</span></span> | <span data-ttu-id="f2f8b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2f8b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2f8b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2f8b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f2f8b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2f8b-118">Request headers</span></span>

| <span data-ttu-id="f2f8b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f2f8b-119">Name</span></span>       | <span data-ttu-id="f2f8b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f8b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f2f8b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2f8b-121">Authorization</span></span>  | <span data-ttu-id="f2f8b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2f8b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2f8b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2f8b-124">Request body</span></span>

<span data-ttu-id="f2f8b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2f8b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2f8b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2f8b-126">Response</span></span>

<span data-ttu-id="f2f8b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f2f8b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2f8b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f2f8b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2f8b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2f8b-130">Request</span></span>

<span data-ttu-id="f2f8b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2f8b-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2f8b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2f8b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```
# <a name="c"></a>[<span data-ttu-id="f2f8b-133">C#</span><span class="sxs-lookup"><span data-stu-id="f2f8b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2f8b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2f8b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2f8b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2f8b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2f8b-136">Java</span><span class="sxs-lookup"><span data-stu-id="f2f8b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlooktask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2f8b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2f8b-137">Response</span></span>

<span data-ttu-id="f2f8b-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2f8b-138">Here is an example of the response.</span></span>
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


