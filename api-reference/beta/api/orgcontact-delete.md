---
title: Удаление orgContact
description: Удаление orgContact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87394067841bb5606630db8022509d3aa9723cfc
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657275"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="78dca-103">Удаление orgContact</span><span class="sxs-lookup"><span data-stu-id="78dca-103">Delete orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78dca-104">Удаление orgContact.</span><span class="sxs-lookup"><span data-stu-id="78dca-104">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="78dca-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78dca-105">Permissions</span></span>
<span data-ttu-id="78dca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78dca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78dca-108">Permission type</span></span>      | <span data-ttu-id="78dca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78dca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78dca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78dca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78dca-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="78dca-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="78dca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78dca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78dca-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78dca-113">Not supported.</span></span>    |
|<span data-ttu-id="78dca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78dca-114">Application</span></span> | <span data-ttu-id="78dca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78dca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78dca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78dca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="78dca-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78dca-117">Request headers</span></span>
| <span data-ttu-id="78dca-118">Имя</span><span class="sxs-lookup"><span data-stu-id="78dca-118">Name</span></span>       | <span data-ttu-id="78dca-119">Тип</span><span class="sxs-lookup"><span data-stu-id="78dca-119">Type</span></span> | <span data-ttu-id="78dca-120">Описание</span><span class="sxs-lookup"><span data-stu-id="78dca-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78dca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="78dca-121">Authorization</span></span>  | <span data-ttu-id="78dca-122">string</span><span class="sxs-lookup"><span data-stu-id="78dca-122">string</span></span>  | <span data-ttu-id="78dca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78dca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78dca-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="78dca-125">Request body</span></span>
<span data-ttu-id="78dca-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78dca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78dca-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="78dca-127">Response</span></span>

<span data-ttu-id="78dca-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="78dca-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78dca-130">Пример</span><span class="sxs-lookup"><span data-stu-id="78dca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78dca-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="78dca-131">Request</span></span>
<span data-ttu-id="78dca-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78dca-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="78dca-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="78dca-133">Response</span></span>
<span data-ttu-id="78dca-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="78dca-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="78dca-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="78dca-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="78dca-136">C#</span><span class="sxs-lookup"><span data-stu-id="78dca-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_orgcontact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78dca-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="78dca-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_orgcontact-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/orgcontact-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
