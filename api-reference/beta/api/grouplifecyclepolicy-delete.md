---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 47a372872e849437c2367a1de6744c9b1b15e173
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001906"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="446ee-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="446ee-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="446ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="446ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="446ee-105">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="446ee-105">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="446ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="446ee-106">Permissions</span></span>

<span data-ttu-id="446ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="446ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="446ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="446ee-109">Permission type</span></span>      | <span data-ttu-id="446ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="446ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="446ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="446ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="446ee-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446ee-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="446ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="446ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="446ee-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="446ee-114">Not supported</span></span> |
|<span data-ttu-id="446ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="446ee-115">Application</span></span> | <span data-ttu-id="446ee-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446ee-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="446ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="446ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="446ee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="446ee-118">Request headers</span></span>

| <span data-ttu-id="446ee-119">Имя</span><span class="sxs-lookup"><span data-stu-id="446ee-119">Name</span></span> | <span data-ttu-id="446ee-120">Описание</span><span class="sxs-lookup"><span data-stu-id="446ee-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="446ee-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="446ee-121">Authorization</span></span> | <span data-ttu-id="446ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="446ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="446ee-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="446ee-124">Content-Type</span></span>  | <span data-ttu-id="446ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="446ee-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="446ee-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="446ee-126">Request body</span></span>
<span data-ttu-id="446ee-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="446ee-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="446ee-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="446ee-128">Response</span></span>

<span data-ttu-id="446ee-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="446ee-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="446ee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="446ee-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="446ee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="446ee-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="446ee-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="446ee-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="446ee-134">C#</span><span class="sxs-lookup"><span data-stu-id="446ee-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="446ee-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="446ee-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="446ee-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="446ee-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="446ee-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="446ee-137">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


