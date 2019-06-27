---
title: Удаление канала
description: Удаление канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d1beba200c44ab74b1271a62a3c7f194a7aff279
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262211"
---
# <a name="delete-channel"></a><span data-ttu-id="fc7d3-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="fc7d3-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc7d3-104">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="fc7d3-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="fc7d3-105">**Примечание**. Существует известная проблема с разрешениями для приложений и этим API.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="fc7d3-106">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="fc7d3-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc7d3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc7d3-107">Permissions</span></span>
<span data-ttu-id="fc7d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc7d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc7d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc7d3-110">Permission type</span></span>      | <span data-ttu-id="fc7d3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc7d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc7d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc7d3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc7d3-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc7d3-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fc7d3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc7d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc7d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-115">Not supported.</span></span>    |
|<span data-ttu-id="fc7d3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc7d3-116">Application</span></span> | <span data-ttu-id="fc7d3-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc7d3-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="fc7d3-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fc7d3-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fc7d3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc7d3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fc7d3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc7d3-121">Request headers</span></span>
| <span data-ttu-id="fc7d3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc7d3-122">Header</span></span>       | <span data-ttu-id="fc7d3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fc7d3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc7d3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc7d3-124">Authorization</span></span>  | <span data-ttu-id="fc7d3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc7d3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc7d3-127">Request body</span></span>
<span data-ttu-id="fc7d3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc7d3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc7d3-129">Response</span></span>

<span data-ttu-id="fc7d3-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc7d3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fc7d3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc7d3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc7d3-133">Request</span></span>
<span data-ttu-id="fc7d3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="fc7d3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc7d3-135">Response</span></span>

<span data-ttu-id="fc7d3-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc7d3-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fc7d3-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fc7d3-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fc7d3-138">C#</span><span class="sxs-lookup"><span data-stu-id="fc7d3-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc7d3-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc7d3-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_channel-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fc7d3-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fc7d3-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_channel-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
