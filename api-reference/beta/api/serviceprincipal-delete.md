---
title: Удаление servicePrincipal
description: Удаление servicePrincipal.
localization_priority: Normal
ms.openlocfilehash: e3da02688355fa68545691072bc13d32f7402486
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269036"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="25bfc-103">Удаление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="25bfc-103">Delete servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25bfc-104">Удаление servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="25bfc-104">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="25bfc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25bfc-105">Permissions</span></span>
<span data-ttu-id="25bfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25bfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25bfc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25bfc-108">Permission type</span></span>      | <span data-ttu-id="25bfc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25bfc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25bfc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25bfc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25bfc-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="25bfc-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="25bfc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25bfc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25bfc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25bfc-113">Not supported.</span></span>    |
|<span data-ttu-id="25bfc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25bfc-114">Application</span></span> | <span data-ttu-id="25bfc-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25bfc-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25bfc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25bfc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="25bfc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25bfc-117">Request headers</span></span>
| <span data-ttu-id="25bfc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="25bfc-118">Name</span></span>       | <span data-ttu-id="25bfc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="25bfc-119">Type</span></span> | <span data-ttu-id="25bfc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="25bfc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25bfc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25bfc-121">Authorization</span></span>  | <span data-ttu-id="25bfc-122">string</span><span class="sxs-lookup"><span data-stu-id="25bfc-122">string</span></span>  | <span data-ttu-id="25bfc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25bfc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25bfc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25bfc-125">Request body</span></span>
<span data-ttu-id="25bfc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25bfc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25bfc-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="25bfc-127">Response</span></span>

<span data-ttu-id="25bfc-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="25bfc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25bfc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="25bfc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25bfc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="25bfc-131">Request</span></span>
<span data-ttu-id="25bfc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25bfc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="25bfc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="25bfc-133">Response</span></span>
<span data-ttu-id="25bfc-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25bfc-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="25bfc-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="25bfc-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="25bfc-136">C#</span><span class="sxs-lookup"><span data-stu-id="25bfc-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_serviceprincipal-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="25bfc-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="25bfc-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_serviceprincipal-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="25bfc-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="25bfc-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_serviceprincipal-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/serviceprincipal-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
