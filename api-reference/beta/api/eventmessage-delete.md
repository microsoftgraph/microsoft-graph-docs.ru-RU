---
title: Удаление объекта eventMessage
description: Удаление объекта eventMessage.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1aca6a297a9d2b7732fc08f7595caeba13492760
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43364497"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="920fb-103">Удаление объекта eventMessage</span><span class="sxs-lookup"><span data-stu-id="920fb-103">Delete eventMessage</span></span>

<span data-ttu-id="920fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="920fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="920fb-105">Удаление объекта eventMessage.</span><span class="sxs-lookup"><span data-stu-id="920fb-105">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="920fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="920fb-106">Permissions</span></span>
<span data-ttu-id="920fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="920fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="920fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="920fb-109">Permission type</span></span>      | <span data-ttu-id="920fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="920fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="920fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="920fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="920fb-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="920fb-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="920fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="920fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="920fb-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="920fb-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="920fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="920fb-115">Application</span></span> | <span data-ttu-id="920fb-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="920fb-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="920fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="920fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="920fb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="920fb-118">Request headers</span></span>
| <span data-ttu-id="920fb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="920fb-119">Name</span></span>       | <span data-ttu-id="920fb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="920fb-120">Type</span></span> | <span data-ttu-id="920fb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="920fb-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="920fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="920fb-122">Authorization</span></span>  | <span data-ttu-id="920fb-123">string</span><span class="sxs-lookup"><span data-stu-id="920fb-123">string</span></span>  | <span data-ttu-id="920fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="920fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="920fb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="920fb-126">Request body</span></span>
<span data-ttu-id="920fb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="920fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="920fb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="920fb-128">Response</span></span>

<span data-ttu-id="920fb-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="920fb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="920fb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="920fb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="920fb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="920fb-132">Request</span></span>
<span data-ttu-id="920fb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="920fb-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="920fb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="920fb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="920fb-135">C#</span><span class="sxs-lookup"><span data-stu-id="920fb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="920fb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="920fb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="920fb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="920fb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="920fb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="920fb-138">Response</span></span>
<span data-ttu-id="920fb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="920fb-139">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
