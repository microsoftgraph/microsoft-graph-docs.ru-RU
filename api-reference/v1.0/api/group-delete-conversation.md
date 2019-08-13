---
title: Удаление беседы
description: Удаление объекта conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5996b860492f26ec0a42caa7d78d92dabdd4b2d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337533"
---
# <a name="delete-conversation"></a><span data-ttu-id="f6691-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="f6691-103">Delete conversation</span></span>
<span data-ttu-id="f6691-104">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="f6691-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6691-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6691-105">Permissions</span></span>
<span data-ttu-id="f6691-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6691-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6691-108">Permission type</span></span>      | <span data-ttu-id="f6691-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6691-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6691-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6691-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6691-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6691-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6691-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6691-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6691-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6691-113">Not supported.</span></span>    |
|<span data-ttu-id="f6691-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6691-114">Application</span></span> | <span data-ttu-id="f6691-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6691-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6691-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6691-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f6691-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6691-117">Request headers</span></span>
| <span data-ttu-id="f6691-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f6691-118">Name</span></span>       | <span data-ttu-id="f6691-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f6691-119">Type</span></span> | <span data-ttu-id="f6691-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f6691-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f6691-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6691-121">Authorization</span></span>  | <span data-ttu-id="f6691-122">string</span><span class="sxs-lookup"><span data-stu-id="f6691-122">string</span></span>  | <span data-ttu-id="f6691-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6691-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6691-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6691-125">Request body</span></span>
<span data-ttu-id="f6691-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6691-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6691-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6691-127">Response</span></span>
<span data-ttu-id="f6691-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f6691-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6691-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f6691-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f6691-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6691-131">Request</span></span>
<span data-ttu-id="f6691-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6691-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f6691-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6691-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6691-134">C#</span><span class="sxs-lookup"><span data-stu-id="f6691-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6691-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6691-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6691-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f6691-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f6691-137">Java</span><span class="sxs-lookup"><span data-stu-id="f6691-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f6691-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6691-138">Response</span></span>
<span data-ttu-id="f6691-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6691-139">The following is an example of the response.</span></span> 
><span data-ttu-id="f6691-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6691-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
