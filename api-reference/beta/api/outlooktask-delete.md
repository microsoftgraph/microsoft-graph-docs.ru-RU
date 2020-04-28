---
title: Удаление outlookTask
description: Удаление указанной задачи Outlook в почтовом ящике пользователя.
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 62eb192165968e2f5abc7d0589fb872f9dd911f6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413832"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="8bb96-103">Удаление outlookTask</span><span class="sxs-lookup"><span data-stu-id="8bb96-103">Delete outlookTask</span></span>

<span data-ttu-id="8bb96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bb96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb96-105">Удаление указанной задачи Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="8bb96-105">Delete the specified Outlook task in the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb96-106">Permissions</span></span>

<span data-ttu-id="8bb96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb96-109">Permission type</span></span>      | <span data-ttu-id="8bb96-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bb96-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bb96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bb96-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8bb96-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bb96-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8bb96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bb96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb96-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bb96-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8bb96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bb96-115">Application</span></span> | <span data-ttu-id="8bb96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb96-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bb96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bb96-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bb96-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bb96-118">Request headers</span></span>

| <span data-ttu-id="8bb96-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8bb96-119">Name</span></span>       | <span data-ttu-id="8bb96-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb96-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8bb96-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bb96-121">Authorization</span></span>  | <span data-ttu-id="8bb96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bb96-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bb96-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8bb96-124">Request body</span></span>

<span data-ttu-id="8bb96-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bb96-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bb96-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="8bb96-126">Response</span></span>

<span data-ttu-id="8bb96-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8bb96-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bb96-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8bb96-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bb96-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bb96-130">Request</span></span>

<span data-ttu-id="8bb96-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bb96-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bb96-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb96-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=
```
# <a name="c"></a>[<span data-ttu-id="8bb96-133">C#</span><span class="sxs-lookup"><span data-stu-id="8bb96-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bb96-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb96-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bb96-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bb96-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8bb96-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb96-136">Response</span></span>

<span data-ttu-id="8bb96-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8bb96-137">Here is an example of the response.</span></span>
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
