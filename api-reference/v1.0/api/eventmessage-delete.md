---
title: Удаление объекта eventMessage
description: Удаление объекта eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 04f9d54ce2c525f8379953d7ca927edd7ee3ec50
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447336"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="1fe75-103">Удаление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="1fe75-103">Delete eventMessage</span></span>

<span data-ttu-id="1fe75-104">Удаление объекта eventMessage.</span><span class="sxs-lookup"><span data-stu-id="1fe75-104">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="1fe75-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fe75-105">Permissions</span></span>
<span data-ttu-id="1fe75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fe75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fe75-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fe75-108">Permission type</span></span>      | <span data-ttu-id="1fe75-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fe75-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fe75-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fe75-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1fe75-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe75-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1fe75-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fe75-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fe75-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe75-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1fe75-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fe75-114">Application</span></span> | <span data-ttu-id="1fe75-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fe75-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fe75-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fe75-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1fe75-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fe75-117">Request headers</span></span>
| <span data-ttu-id="1fe75-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1fe75-118">Name</span></span>       | <span data-ttu-id="1fe75-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1fe75-119">Type</span></span> | <span data-ttu-id="1fe75-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1fe75-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fe75-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fe75-121">Authorization</span></span>  | <span data-ttu-id="1fe75-122">string</span><span class="sxs-lookup"><span data-stu-id="1fe75-122">string</span></span>  | <span data-ttu-id="1fe75-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fe75-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fe75-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1fe75-125">Request body</span></span>
<span data-ttu-id="1fe75-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fe75-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fe75-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fe75-127">Response</span></span>

<span data-ttu-id="1fe75-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1fe75-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fe75-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1fe75-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fe75-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fe75-131">Request</span></span>
<span data-ttu-id="1fe75-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fe75-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1fe75-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fe75-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1fe75-134">C#</span><span class="sxs-lookup"><span data-stu-id="1fe75-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1fe75-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1fe75-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1fe75-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1fe75-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1fe75-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fe75-137">Response</span></span>
<span data-ttu-id="1fe75-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1fe75-138">Here is an example of the response.</span></span> 
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
