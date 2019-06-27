---
title: Получение группы маршрутизации звука
description: Получение свойств и связей объекта Аудиораутингграуп.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 43279f67b88e5e4c08c2c1cd83648786585b538d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258291"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="e4999-103">Получение группы маршрутизации звука</span><span class="sxs-lookup"><span data-stu-id="e4999-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4999-104">Получение свойств и связей объекта [аудиораутингграуп](../resources/audioroutinggroup.md) .</span><span class="sxs-lookup"><span data-stu-id="e4999-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4999-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4999-105">Permissions</span></span>
<span data-ttu-id="e4999-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4999-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4999-108">Permission type</span></span>                        | <span data-ttu-id="e4999-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4999-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e4999-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4999-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4999-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e4999-111">Not Supported</span></span>                               |
| <span data-ttu-id="e4999-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4999-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4999-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e4999-113">Not Supported</span></span>                               |
| <span data-ttu-id="e4999-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4999-114">Application</span></span>                            | <span data-ttu-id="e4999-115">Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="e4999-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4999-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4999-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4999-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4999-117">Optional query parameters</span></span>
<span data-ttu-id="e4999-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e4999-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4999-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4999-119">Request headers</span></span>
| <span data-ttu-id="e4999-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e4999-120">Name</span></span>          | <span data-ttu-id="e4999-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e4999-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e4999-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4999-122">Authorization</span></span> | <span data-ttu-id="e4999-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4999-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4999-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4999-125">Request body</span></span>
<span data-ttu-id="e4999-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4999-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4999-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4999-127">Response</span></span>
<span data-ttu-id="e4999-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [аудиораутингграуп](../resources/audioroutinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4999-128">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4999-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e4999-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e4999-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4999-130">Request</span></span>
<span data-ttu-id="e4999-131">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4999-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="e4999-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4999-132">Response</span></span>

> <span data-ttu-id="e4999-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4999-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e4999-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e4999-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e4999-136">C#</span><span class="sxs-lookup"><span data-stu-id="e4999-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4999-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="e4999-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e4999-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e4999-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-audioRoutingGroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/audioroutinggroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/audioroutinggroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
