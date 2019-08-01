---
title: Удаление цепочки беседы
description: Удаление объекта thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 347143e8cea8ad221de505e901131374f84622ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006656"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="c6524-103">Удаление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="c6524-103">Delete conversation thread</span></span>
<span data-ttu-id="c6524-104">Удаление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="c6524-104">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6524-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6524-105">Permissions</span></span>
<span data-ttu-id="c6524-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6524-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6524-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6524-108">Permission type</span></span>      | <span data-ttu-id="c6524-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6524-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6524-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6524-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c6524-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6524-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c6524-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6524-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6524-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6524-113">Not supported.</span></span>    |
|<span data-ttu-id="c6524-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6524-114">Application</span></span> | <span data-ttu-id="c6524-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6524-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6524-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6524-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c6524-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6524-117">Request headers</span></span>
| <span data-ttu-id="c6524-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c6524-118">Name</span></span>       | <span data-ttu-id="c6524-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c6524-119">Type</span></span> | <span data-ttu-id="c6524-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c6524-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6524-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6524-121">Authorization</span></span>  | <span data-ttu-id="c6524-122">string</span><span class="sxs-lookup"><span data-stu-id="c6524-122">string</span></span>  | <span data-ttu-id="c6524-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6524-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6524-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6524-125">Request body</span></span>
<span data-ttu-id="c6524-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6524-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6524-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6524-127">Response</span></span>
<span data-ttu-id="c6524-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c6524-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6524-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c6524-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c6524-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6524-131">Request</span></span>
<span data-ttu-id="c6524-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6524-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c6524-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6524-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c6524-134">C#</span><span class="sxs-lookup"><span data-stu-id="c6524-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6524-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6524-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c6524-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c6524-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c6524-137">Java</span><span class="sxs-lookup"><span data-stu-id="c6524-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c6524-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6524-138">Response</span></span>
<span data-ttu-id="c6524-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c6524-139">The following is an example of the response.</span></span> 
><span data-ttu-id="c6524-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6524-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
