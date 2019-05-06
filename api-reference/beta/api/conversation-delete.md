---
title: Удаление беседы
description: Удаление беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7fc4c8d1d3f32cce54ae99687f23e5543be50017
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591235"
---
# <a name="delete-conversation"></a><span data-ttu-id="cfaf3-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="cfaf3-103">Delete conversation</span></span>

<span data-ttu-id="cfaf3-104">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfaf3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfaf3-105">Permissions</span></span>
<span data-ttu-id="cfaf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfaf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfaf3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfaf3-108">Permission type</span></span>      | <span data-ttu-id="cfaf3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfaf3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfaf3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfaf3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfaf3-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfaf3-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cfaf3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfaf3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfaf3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-113">Not supported.</span></span>    |
|<span data-ttu-id="cfaf3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfaf3-114">Application</span></span> | <span data-ttu-id="cfaf3-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfaf3-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfaf3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfaf3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cfaf3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfaf3-117">Request headers</span></span>
| <span data-ttu-id="cfaf3-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cfaf3-118">Header</span></span>       | <span data-ttu-id="cfaf3-119">Значение</span><span class="sxs-lookup"><span data-stu-id="cfaf3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cfaf3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cfaf3-120">Authorization</span></span>  | <span data-ttu-id="cfaf3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfaf3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cfaf3-123">Request body</span></span>
<span data-ttu-id="cfaf3-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfaf3-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="cfaf3-125">Response</span></span>

<span data-ttu-id="cfaf3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfaf3-128">Пример</span><span class="sxs-lookup"><span data-stu-id="cfaf3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfaf3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfaf3-129">Request</span></span>
<span data-ttu-id="cfaf3-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="cfaf3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfaf3-131">Response</span></span>
<span data-ttu-id="cfaf3-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cfaf3-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cfaf3-133">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="cfaf3-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cfaf3-134">Языках</span><span class="sxs-lookup"><span data-stu-id="cfaf3-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfaf3-135">Язык</span><span class="sxs-lookup"><span data-stu-id="cfaf3-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversation-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
