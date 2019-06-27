---
title: Получение объекта schedulingGroup
description: Получение свойств и связей объекта [счедулингграуп](../resources/schedulinggroup.md) по идентификатору.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0f9c09288b63f17d77708112660fd6890a9c3fa3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264885"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="bc420-103">Получение объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="bc420-103">Get schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc420-104">Получение свойств и связей объекта [счедулингграуп](../resources/schedulinggroup.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="bc420-104">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc420-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc420-105">Permissions</span></span>

<span data-ttu-id="bc420-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc420-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc420-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc420-108">Permission type</span></span>      | <span data-ttu-id="bc420-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc420-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc420-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc420-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc420-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc420-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc420-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc420-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc420-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc420-113">Not supported.</span></span>    |
|<span data-ttu-id="bc420-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc420-114">Application</span></span> | <span data-ttu-id="bc420-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc420-115">Not supported.</span></span> |

> <span data-ttu-id="bc420-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="bc420-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bc420-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="bc420-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bc420-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc420-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="bc420-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc420-119">Request headers</span></span>

| <span data-ttu-id="bc420-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc420-120">Header</span></span>       | <span data-ttu-id="bc420-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bc420-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc420-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc420-122">Authorization</span></span>  | <span data-ttu-id="bc420-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc420-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bc420-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc420-125">Content-Type</span></span>  | <span data-ttu-id="bc420-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc420-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc420-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc420-127">Request body</span></span>
<span data-ttu-id="bc420-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc420-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc420-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc420-129">Response</span></span>

<span data-ttu-id="bc420-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc420-130">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc420-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bc420-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bc420-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc420-132">Request</span></span>

<span data-ttu-id="bc420-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc420-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="bc420-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc420-134">Response</span></span>

<span data-ttu-id="bc420-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc420-135">The following is an example of the response.</span></span> 

><span data-ttu-id="bc420-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc420-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bc420-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="bc420-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bc420-139">C#</span><span class="sxs-lookup"><span data-stu-id="bc420-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-get-schedulinggroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc420-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="bc420-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-get-schedulinggroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bc420-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bc420-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/schedule-get-schedulinggroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a schedulingGroup by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedulinggroup-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schedulinggroup-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedulinggroup-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
