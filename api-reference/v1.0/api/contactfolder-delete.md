---
title: Удаление объекта contactFolder
description: Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4060f2c258b1ad9cf8f4e84dd24cd98ef626c6bc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277506"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="c08cf-103">Удаление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="c08cf-103">Delete contactFolder</span></span>

<span data-ttu-id="c08cf-104">Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c08cf-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c08cf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c08cf-105">Permissions</span></span>
<span data-ttu-id="c08cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c08cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c08cf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c08cf-108">Permission type</span></span>      | <span data-ttu-id="c08cf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c08cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c08cf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c08cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c08cf-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c08cf-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c08cf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c08cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c08cf-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c08cf-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c08cf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c08cf-114">Application</span></span> | <span data-ttu-id="c08cf-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c08cf-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c08cf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c08cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c08cf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c08cf-117">Request headers</span></span>
| <span data-ttu-id="c08cf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c08cf-118">Name</span></span>       | <span data-ttu-id="c08cf-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c08cf-119">Type</span></span> | <span data-ttu-id="c08cf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c08cf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c08cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c08cf-121">Authorization</span></span>  | <span data-ttu-id="c08cf-122">string</span><span class="sxs-lookup"><span data-stu-id="c08cf-122">string</span></span>  | <span data-ttu-id="c08cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c08cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c08cf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c08cf-125">Request body</span></span>
<span data-ttu-id="c08cf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c08cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c08cf-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c08cf-127">Response</span></span>

<span data-ttu-id="c08cf-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c08cf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c08cf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c08cf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c08cf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c08cf-131">Request</span></span>
<span data-ttu-id="c08cf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c08cf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="c08cf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c08cf-133">Response</span></span>
<span data-ttu-id="c08cf-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c08cf-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c08cf-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c08cf-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c08cf-136">C#</span><span class="sxs-lookup"><span data-stu-id="c08cf-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c08cf-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="c08cf-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c08cf-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c08cf-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
