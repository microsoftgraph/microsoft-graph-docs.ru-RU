---
title: Удаление объекта eventMessage
description: Удаление объекта eventMessage.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 833c2af37ae92cccea5abf0c2eefc3efbaa75c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038745"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="7562d-103">Удаление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="7562d-103">Delete eventMessage</span></span>

<span data-ttu-id="7562d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7562d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7562d-105">Удаление объекта eventMessage.</span><span class="sxs-lookup"><span data-stu-id="7562d-105">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="7562d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7562d-106">Permissions</span></span>
<span data-ttu-id="7562d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7562d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7562d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7562d-109">Permission type</span></span>      | <span data-ttu-id="7562d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7562d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7562d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7562d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7562d-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7562d-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7562d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7562d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7562d-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7562d-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7562d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7562d-115">Application</span></span> | <span data-ttu-id="7562d-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7562d-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7562d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7562d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7562d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7562d-118">Request headers</span></span>
| <span data-ttu-id="7562d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7562d-119">Name</span></span>       | <span data-ttu-id="7562d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7562d-120">Type</span></span> | <span data-ttu-id="7562d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7562d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7562d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7562d-122">Authorization</span></span>  | <span data-ttu-id="7562d-123">string</span><span class="sxs-lookup"><span data-stu-id="7562d-123">string</span></span>  | <span data-ttu-id="7562d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7562d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7562d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7562d-126">Request body</span></span>
<span data-ttu-id="7562d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7562d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7562d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7562d-128">Response</span></span>

<span data-ttu-id="7562d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7562d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7562d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7562d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7562d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7562d-132">Request</span></span>
<span data-ttu-id="7562d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7562d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7562d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7562d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="7562d-135">C#</span><span class="sxs-lookup"><span data-stu-id="7562d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7562d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7562d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7562d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7562d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7562d-138">Java</span><span class="sxs-lookup"><span data-stu-id="7562d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7562d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7562d-139">Response</span></span>
<span data-ttu-id="7562d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7562d-140">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

