---
title: Удаление беседы
description: Удаление беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0b856648d50b5536c4c3fe42d6c3c18f31d0a635
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436624"
---
# <a name="delete-conversation"></a><span data-ttu-id="ea1dc-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="ea1dc-103">Delete conversation</span></span>

<span data-ttu-id="ea1dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea1dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea1dc-105">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="ea1dc-105">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea1dc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea1dc-106">Permissions</span></span>
<span data-ttu-id="ea1dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea1dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea1dc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea1dc-109">Permission type</span></span>      | <span data-ttu-id="ea1dc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea1dc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea1dc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea1dc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea1dc-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea1dc-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea1dc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea1dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea1dc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea1dc-114">Not supported.</span></span>    |
|<span data-ttu-id="ea1dc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea1dc-115">Application</span></span> | <span data-ttu-id="ea1dc-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea1dc-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea1dc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea1dc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ea1dc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea1dc-118">Request headers</span></span>
| <span data-ttu-id="ea1dc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea1dc-119">Header</span></span>       | <span data-ttu-id="ea1dc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ea1dc-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ea1dc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea1dc-121">Authorization</span></span>  | <span data-ttu-id="ea1dc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea1dc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea1dc-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea1dc-124">Request body</span></span>
<span data-ttu-id="ea1dc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea1dc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea1dc-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea1dc-126">Response</span></span>

<span data-ttu-id="ea1dc-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ea1dc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea1dc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ea1dc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea1dc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea1dc-130">Request</span></span>
<span data-ttu-id="ea1dc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea1dc-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea1dc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea1dc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="ea1dc-133">C#</span><span class="sxs-lookup"><span data-stu-id="ea1dc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea1dc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea1dc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea1dc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea1dc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ea1dc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea1dc-136">Response</span></span>
<span data-ttu-id="ea1dc-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea1dc-137">Here is an example of the response.</span></span> 
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
