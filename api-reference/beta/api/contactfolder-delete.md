---
title: Удаление объекта contactFolder
description: Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b2b34b1b5d7299fc7e002e26dc9545151dc1108
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943325"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="980cf-103">Удаление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="980cf-103">Delete contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="980cf-104">Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="980cf-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="980cf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="980cf-105">Permissions</span></span>
<span data-ttu-id="980cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="980cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="980cf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="980cf-108">Permission type</span></span>      | <span data-ttu-id="980cf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="980cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="980cf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="980cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="980cf-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="980cf-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="980cf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="980cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="980cf-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="980cf-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="980cf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="980cf-114">Application</span></span> | <span data-ttu-id="980cf-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="980cf-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="980cf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="980cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="980cf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="980cf-117">Request headers</span></span>
| <span data-ttu-id="980cf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="980cf-118">Name</span></span>       | <span data-ttu-id="980cf-119">Тип</span><span class="sxs-lookup"><span data-stu-id="980cf-119">Type</span></span> | <span data-ttu-id="980cf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="980cf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="980cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="980cf-121">Authorization</span></span>  | <span data-ttu-id="980cf-122">string</span><span class="sxs-lookup"><span data-stu-id="980cf-122">string</span></span>  | <span data-ttu-id="980cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="980cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="980cf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="980cf-125">Request body</span></span>
<span data-ttu-id="980cf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="980cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="980cf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="980cf-127">Response</span></span>

<span data-ttu-id="980cf-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="980cf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="980cf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="980cf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="980cf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="980cf-131">Request</span></span>
<span data-ttu-id="980cf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="980cf-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="980cf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="980cf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="980cf-134">C#</span><span class="sxs-lookup"><span data-stu-id="980cf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="980cf-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="980cf-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="980cf-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="980cf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="980cf-137">Java</span><span class="sxs-lookup"><span data-stu-id="980cf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="980cf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="980cf-138">Response</span></span>
<span data-ttu-id="980cf-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="980cf-139">Here is an example of the response.</span></span> 
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
