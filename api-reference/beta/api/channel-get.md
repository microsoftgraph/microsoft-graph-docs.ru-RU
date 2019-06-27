---
title: Получение канала
description: Получение свойств и связей канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: deafafd492782e2c0900469c7217113a6cd33ed8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262092"
---
# <a name="get-channel"></a><span data-ttu-id="18df6-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="18df6-103">Get channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18df6-104">Получение свойств и связей [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="18df6-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18df6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18df6-105">Permissions</span></span>
<span data-ttu-id="18df6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18df6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18df6-108">Permission type</span></span>      | <span data-ttu-id="18df6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18df6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18df6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18df6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18df6-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18df6-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="18df6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18df6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18df6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18df6-113">Not supported.</span></span>    |
|<span data-ttu-id="18df6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18df6-114">Application</span></span> | <span data-ttu-id="18df6-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18df6-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="18df6-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="18df6-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="18df6-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="18df6-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="18df6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18df6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="18df6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18df6-119">Optional query parameters</span></span>

<span data-ttu-id="18df6-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="18df6-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18df6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18df6-121">Request headers</span></span>
| <span data-ttu-id="18df6-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18df6-122">Header</span></span>       | <span data-ttu-id="18df6-123">Значение</span><span class="sxs-lookup"><span data-stu-id="18df6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18df6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18df6-124">Authorization</span></span>  | <span data-ttu-id="18df6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18df6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18df6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18df6-127">Request body</span></span>
<span data-ttu-id="18df6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18df6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18df6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="18df6-129">Response</span></span>

<span data-ttu-id="18df6-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18df6-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18df6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="18df6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18df6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="18df6-132">Request</span></span>
<span data-ttu-id="18df6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18df6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="18df6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="18df6-134">Response</span></span>
<span data-ttu-id="18df6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18df6-135">Here is an example of the response.</span></span> 

><span data-ttu-id="18df6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18df6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="18df6-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="18df6-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18df6-139">C#</span><span class="sxs-lookup"><span data-stu-id="18df6-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18df6-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="18df6-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="18df6-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="18df6-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_channel-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
