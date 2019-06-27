---
title: Удаление orgContact
description: Удаление orgContact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eb6baa632b762a8e9e366d2054fa44e1d545d927
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266880"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="d9ceb-103">Удаление orgContact</span><span class="sxs-lookup"><span data-stu-id="d9ceb-103">Delete orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9ceb-104">Удаление orgContact.</span><span class="sxs-lookup"><span data-stu-id="d9ceb-104">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9ceb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ceb-105">Permissions</span></span>
<span data-ttu-id="d9ceb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9ceb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ceb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ceb-108">Permission type</span></span>      | <span data-ttu-id="d9ceb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9ceb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9ceb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9ceb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9ceb-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9ceb-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9ceb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9ceb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9ceb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ceb-113">Not supported.</span></span>    |
|<span data-ttu-id="d9ceb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9ceb-114">Application</span></span> | <span data-ttu-id="d9ceb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ceb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9ceb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9ceb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d9ceb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9ceb-117">Request headers</span></span>
| <span data-ttu-id="d9ceb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d9ceb-118">Name</span></span>       | <span data-ttu-id="d9ceb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d9ceb-119">Type</span></span> | <span data-ttu-id="d9ceb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ceb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9ceb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9ceb-121">Authorization</span></span>  | <span data-ttu-id="d9ceb-122">string</span><span class="sxs-lookup"><span data-stu-id="d9ceb-122">string</span></span>  | <span data-ttu-id="d9ceb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9ceb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9ceb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9ceb-125">Request body</span></span>
<span data-ttu-id="d9ceb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9ceb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9ceb-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9ceb-127">Response</span></span>

<span data-ttu-id="d9ceb-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d9ceb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9ceb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d9ceb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9ceb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9ceb-131">Request</span></span>
<span data-ttu-id="d9ceb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9ceb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="d9ceb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9ceb-133">Response</span></span>
<span data-ttu-id="d9ceb-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d9ceb-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d9ceb-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d9ceb-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d9ceb-136">C#</span><span class="sxs-lookup"><span data-stu-id="d9ceb-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_orgcontact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9ceb-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="d9ceb-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_orgcontact-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d9ceb-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d9ceb-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_orgcontact-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/orgcontact-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
