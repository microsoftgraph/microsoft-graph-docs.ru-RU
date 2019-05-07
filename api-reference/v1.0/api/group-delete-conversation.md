---
title: Удаление беседы
description: Удаление объекта conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 03a33f834083766c081fc99a696bcb2cf4c1c651
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614868"
---
# <a name="delete-conversation"></a><span data-ttu-id="69c07-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="69c07-103">Delete conversation</span></span>
<span data-ttu-id="69c07-104">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="69c07-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="69c07-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69c07-105">Permissions</span></span>
<span data-ttu-id="69c07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69c07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69c07-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69c07-108">Permission type</span></span>      | <span data-ttu-id="69c07-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69c07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69c07-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69c07-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69c07-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c07-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69c07-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69c07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69c07-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69c07-113">Not supported.</span></span>    |
|<span data-ttu-id="69c07-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69c07-114">Application</span></span> | <span data-ttu-id="69c07-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69c07-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69c07-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69c07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="69c07-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69c07-117">Request headers</span></span>
| <span data-ttu-id="69c07-118">Имя</span><span class="sxs-lookup"><span data-stu-id="69c07-118">Name</span></span>       | <span data-ttu-id="69c07-119">Тип</span><span class="sxs-lookup"><span data-stu-id="69c07-119">Type</span></span> | <span data-ttu-id="69c07-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69c07-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69c07-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69c07-121">Authorization</span></span>  | <span data-ttu-id="69c07-122">string</span><span class="sxs-lookup"><span data-stu-id="69c07-122">string</span></span>  | <span data-ttu-id="69c07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69c07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69c07-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69c07-125">Request body</span></span>
<span data-ttu-id="69c07-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69c07-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69c07-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="69c07-127">Response</span></span>
<span data-ttu-id="69c07-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="69c07-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69c07-130">Пример</span><span class="sxs-lookup"><span data-stu-id="69c07-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="69c07-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="69c07-131">Request</span></span>
<span data-ttu-id="69c07-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69c07-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="69c07-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="69c07-133">Response</span></span>
<span data-ttu-id="69c07-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="69c07-134">The following is an example of the response.</span></span> 
><span data-ttu-id="69c07-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69c07-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="69c07-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="69c07-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="69c07-138">Языках</span><span class="sxs-lookup"><span data-stu-id="69c07-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_group_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69c07-139">Язык</span><span class="sxs-lookup"><span data-stu-id="69c07-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_group_conversation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete-conversation.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-conversation.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
