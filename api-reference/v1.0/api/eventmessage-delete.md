---
title: Удаление объекта eventMessage
description: Удаление объекта eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fb8cac269055e1e4b4c05daf6d8e1983139b239b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015026"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="db2eb-103">Удаление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="db2eb-103">Delete eventMessage</span></span>

<span data-ttu-id="db2eb-104">Удаление объекта eventMessage.</span><span class="sxs-lookup"><span data-stu-id="db2eb-104">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="db2eb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db2eb-105">Permissions</span></span>
<span data-ttu-id="db2eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db2eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db2eb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db2eb-108">Permission type</span></span>      | <span data-ttu-id="db2eb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db2eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db2eb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db2eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db2eb-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db2eb-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="db2eb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db2eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db2eb-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db2eb-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="db2eb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db2eb-114">Application</span></span> | <span data-ttu-id="db2eb-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db2eb-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="db2eb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db2eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="db2eb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db2eb-117">Request headers</span></span>
| <span data-ttu-id="db2eb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="db2eb-118">Name</span></span>       | <span data-ttu-id="db2eb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="db2eb-119">Type</span></span> | <span data-ttu-id="db2eb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="db2eb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db2eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db2eb-121">Authorization</span></span>  | <span data-ttu-id="db2eb-122">string</span><span class="sxs-lookup"><span data-stu-id="db2eb-122">string</span></span>  | <span data-ttu-id="db2eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db2eb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db2eb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="db2eb-125">Request body</span></span>
<span data-ttu-id="db2eb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db2eb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db2eb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="db2eb-127">Response</span></span>

<span data-ttu-id="db2eb-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="db2eb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db2eb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="db2eb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db2eb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="db2eb-131">Request</span></span>
<span data-ttu-id="db2eb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db2eb-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db2eb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db2eb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db2eb-134">C#</span><span class="sxs-lookup"><span data-stu-id="db2eb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db2eb-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="db2eb-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db2eb-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="db2eb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db2eb-137">Java</span><span class="sxs-lookup"><span data-stu-id="db2eb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db2eb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="db2eb-138">Response</span></span>
<span data-ttu-id="db2eb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db2eb-139">Here is an example of the response.</span></span> 
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
