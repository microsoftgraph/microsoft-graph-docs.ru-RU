---
title: Удаление беседы
description: Удаление объекта conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 03b5c098dc0b41c8f753da7ccf115067f97fd879
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859010"
---
# <a name="delete-conversation"></a><span data-ttu-id="abce4-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="abce4-103">Delete conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abce4-104">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="abce4-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="abce4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abce4-105">Permissions</span></span>
<span data-ttu-id="abce4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abce4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abce4-108">Permission type</span></span>      | <span data-ttu-id="abce4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abce4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abce4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abce4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abce4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abce4-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="abce4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abce4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abce4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abce4-113">Not supported.</span></span>    |
|<span data-ttu-id="abce4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abce4-114">Application</span></span> | <span data-ttu-id="abce4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abce4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abce4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abce4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="abce4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abce4-117">Request headers</span></span>
| <span data-ttu-id="abce4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="abce4-118">Name</span></span>       | <span data-ttu-id="abce4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="abce4-119">Type</span></span> | <span data-ttu-id="abce4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="abce4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="abce4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="abce4-121">Authorization</span></span>  | <span data-ttu-id="abce4-122">string</span><span class="sxs-lookup"><span data-stu-id="abce4-122">string</span></span>  | <span data-ttu-id="abce4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abce4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="abce4-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="abce4-125">Request body</span></span>
<span data-ttu-id="abce4-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abce4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abce4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="abce4-127">Response</span></span>
<span data-ttu-id="abce4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="abce4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abce4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="abce4-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="abce4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="abce4-131">Request</span></span>
<span data-ttu-id="abce4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abce4-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="abce4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="abce4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="abce4-134">C#</span><span class="sxs-lookup"><span data-stu-id="abce4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="abce4-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="abce4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="abce4-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="abce4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="abce4-137">Java</span><span class="sxs-lookup"><span data-stu-id="abce4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="abce4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="abce4-138">Response</span></span>
<span data-ttu-id="abce4-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="abce4-139">The following is an example of the response.</span></span> 
><span data-ttu-id="abce4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abce4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
