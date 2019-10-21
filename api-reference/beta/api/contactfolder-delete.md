---
title: Удаление объекта contactFolder
description: Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: af89a4d009dd1ab3110b72ac515700a2b1d1efb8
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2019
ms.locfileid: "36418000"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="47f30-103">Удаление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="47f30-103">Delete contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47f30-104">Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="47f30-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="47f30-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47f30-105">Permissions</span></span>
<span data-ttu-id="47f30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47f30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47f30-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47f30-108">Permission type</span></span>      | <span data-ttu-id="47f30-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47f30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47f30-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47f30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47f30-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47f30-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="47f30-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47f30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47f30-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47f30-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="47f30-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47f30-114">Application</span></span> | <span data-ttu-id="47f30-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47f30-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="47f30-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47f30-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="47f30-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47f30-117">Request headers</span></span>
| <span data-ttu-id="47f30-118">Имя</span><span class="sxs-lookup"><span data-stu-id="47f30-118">Name</span></span>       | <span data-ttu-id="47f30-119">Тип</span><span class="sxs-lookup"><span data-stu-id="47f30-119">Type</span></span> | <span data-ttu-id="47f30-120">Описание</span><span class="sxs-lookup"><span data-stu-id="47f30-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47f30-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47f30-121">Authorization</span></span>  | <span data-ttu-id="47f30-122">string</span><span class="sxs-lookup"><span data-stu-id="47f30-122">string</span></span>  | <span data-ttu-id="47f30-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47f30-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47f30-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47f30-125">Request body</span></span>
<span data-ttu-id="47f30-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47f30-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47f30-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="47f30-127">Response</span></span>

<span data-ttu-id="47f30-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47f30-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f30-130">Пример</span><span class="sxs-lookup"><span data-stu-id="47f30-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47f30-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="47f30-131">Request</span></span>
<span data-ttu-id="47f30-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47f30-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="47f30-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="47f30-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="47f30-134">C#</span><span class="sxs-lookup"><span data-stu-id="47f30-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47f30-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47f30-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="47f30-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47f30-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="47f30-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f30-137">Response</span></span>
<span data-ttu-id="47f30-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47f30-138">Here is an example of the response.</span></span> 
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
