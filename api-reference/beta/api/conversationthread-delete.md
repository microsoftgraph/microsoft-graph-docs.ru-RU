---
title: Удаление объекта conversationThread
description: Удаление объекта conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a89176839875d4b5ecd3edd6e4d83242d29be567
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591123"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="e3727-103">Удаление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="e3727-103">Delete conversationThread</span></span>

<span data-ttu-id="e3727-104">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="e3727-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3727-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3727-105">Permissions</span></span>
<span data-ttu-id="e3727-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3727-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3727-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3727-108">Permission type</span></span>      | <span data-ttu-id="e3727-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3727-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3727-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3727-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e3727-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3727-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3727-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3727-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3727-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3727-113">Not supported.</span></span>    |
|<span data-ttu-id="e3727-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3727-114">Application</span></span> | <span data-ttu-id="e3727-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3727-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3727-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3727-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e3727-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3727-117">Request headers</span></span>
| <span data-ttu-id="e3727-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3727-118">Header</span></span>       | <span data-ttu-id="e3727-119">Значение</span><span class="sxs-lookup"><span data-stu-id="e3727-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3727-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3727-120">Authorization</span></span>  | <span data-ttu-id="e3727-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3727-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3727-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3727-123">Request body</span></span>
<span data-ttu-id="e3727-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3727-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3727-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3727-125">Response</span></span>

<span data-ttu-id="e3727-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e3727-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3727-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e3727-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3727-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3727-129">Request</span></span>
<span data-ttu-id="e3727-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3727-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="e3727-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3727-131">Response</span></span>
<span data-ttu-id="e3727-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3727-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3727-133">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e3727-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3727-134">Языках</span><span class="sxs-lookup"><span data-stu-id="e3727-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3727-135">Язык</span><span class="sxs-lookup"><span data-stu-id="e3727-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversationthread-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversationthread-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
