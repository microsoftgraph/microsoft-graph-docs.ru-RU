---
title: Удаление объекта contactFolder
description: Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 587941fd8463971c593caa045b17759b10758d00
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996327"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="689a4-103">Удаление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="689a4-103">Delete contactFolder</span></span>

<span data-ttu-id="689a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="689a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="689a4-105">Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="689a4-105">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="689a4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="689a4-106">Permissions</span></span>
<span data-ttu-id="689a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="689a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="689a4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="689a4-109">Permission type</span></span>      | <span data-ttu-id="689a4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="689a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="689a4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="689a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="689a4-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="689a4-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="689a4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="689a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="689a4-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="689a4-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="689a4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="689a4-115">Application</span></span> | <span data-ttu-id="689a4-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="689a4-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="689a4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="689a4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="689a4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="689a4-118">Request headers</span></span>
| <span data-ttu-id="689a4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="689a4-119">Name</span></span>       | <span data-ttu-id="689a4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="689a4-120">Type</span></span> | <span data-ttu-id="689a4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="689a4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="689a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="689a4-122">Authorization</span></span>  | <span data-ttu-id="689a4-123">string</span><span class="sxs-lookup"><span data-stu-id="689a4-123">string</span></span>  | <span data-ttu-id="689a4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="689a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="689a4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="689a4-126">Request body</span></span>
<span data-ttu-id="689a4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="689a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="689a4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="689a4-128">Response</span></span>

<span data-ttu-id="689a4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="689a4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="689a4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="689a4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="689a4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="689a4-132">Request</span></span>
<span data-ttu-id="689a4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="689a4-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="689a4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="689a4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="689a4-135">C#</span><span class="sxs-lookup"><span data-stu-id="689a4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="689a4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="689a4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="689a4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="689a4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="689a4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="689a4-138">Response</span></span>
<span data-ttu-id="689a4-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="689a4-139">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


