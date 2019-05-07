---
title: Получение канала
description: Получение свойств и связей канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a217f83cc9ab039e990af2cada53919d00b296dc
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635479"
---
# <a name="get-channel"></a><span data-ttu-id="29676-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="29676-103">Get channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29676-104">Получение свойств и связей [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="29676-104">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29676-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29676-105">Permissions</span></span>
<span data-ttu-id="29676-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29676-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29676-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29676-108">Permission type</span></span>      | <span data-ttu-id="29676-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29676-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29676-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29676-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29676-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29676-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="29676-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29676-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29676-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29676-113">Not supported.</span></span>    |
|<span data-ttu-id="29676-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29676-114">Application</span></span> | <span data-ttu-id="29676-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29676-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="29676-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="29676-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="29676-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="29676-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="29676-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29676-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="29676-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29676-119">Optional query parameters</span></span>

<span data-ttu-id="29676-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="29676-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29676-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29676-121">Request headers</span></span>
| <span data-ttu-id="29676-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29676-122">Header</span></span>       | <span data-ttu-id="29676-123">Значение</span><span class="sxs-lookup"><span data-stu-id="29676-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29676-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29676-124">Authorization</span></span>  | <span data-ttu-id="29676-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29676-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29676-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29676-127">Request body</span></span>
<span data-ttu-id="29676-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29676-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29676-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="29676-129">Response</span></span>

<span data-ttu-id="29676-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29676-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29676-131">Пример</span><span class="sxs-lookup"><span data-stu-id="29676-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29676-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="29676-132">Request</span></span>
<span data-ttu-id="29676-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29676-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="29676-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="29676-134">Response</span></span>
<span data-ttu-id="29676-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="29676-135">Here is an example of the response.</span></span> 

><span data-ttu-id="29676-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29676-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="29676-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="29676-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="29676-139">Языках</span><span class="sxs-lookup"><span data-stu-id="29676-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29676-140">Язык</span><span class="sxs-lookup"><span data-stu-id="29676-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/channel-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
