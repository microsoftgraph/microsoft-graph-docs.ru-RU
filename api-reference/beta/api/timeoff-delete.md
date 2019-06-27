---
title: Удаление Тимеофф
description: Удаление экземпляра Тимеофф по расписанию.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ee20d51fe5cf2c3cc01db23e65398deba2263e68
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270590"
---
# <a name="delete-timeoff"></a><span data-ttu-id="7c0d9-103">Удаление Тимеофф</span><span class="sxs-lookup"><span data-stu-id="7c0d9-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c0d9-104">Удаление экземпляра [тимеофф](../resources/timeoff.md) по расписанию [](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="7c0d9-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c0d9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c0d9-105">Permissions</span></span>

<span data-ttu-id="7c0d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c0d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c0d9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c0d9-108">Permission type</span></span>      | <span data-ttu-id="7c0d9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c0d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c0d9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c0d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c0d9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c0d9-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7c0d9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c0d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c0d9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-113">Not supported.</span></span>    |
|<span data-ttu-id="7c0d9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c0d9-114">Application</span></span> | <span data-ttu-id="7c0d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-115">Not supported.</span></span> |

> <span data-ttu-id="7c0d9-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7c0d9-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7c0d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c0d9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="7c0d9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c0d9-119">Request headers</span></span>

| <span data-ttu-id="7c0d9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c0d9-120">Header</span></span>       | <span data-ttu-id="7c0d9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c0d9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c0d9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c0d9-122">Authorization</span></span>  | <span data-ttu-id="7c0d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7c0d9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c0d9-125">Content-Type</span></span>  | <span data-ttu-id="7c0d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c0d9-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c0d9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c0d9-127">Request body</span></span>
<span data-ttu-id="7c0d9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c0d9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c0d9-129">Response</span></span>

<span data-ttu-id="7c0d9-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c0d9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7c0d9-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c0d9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c0d9-133">Request</span></span>

<span data-ttu-id="7c0d9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```

#### <a name="response"></a><span data-ttu-id="7c0d9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c0d9-135">Response</span></span>

<span data-ttu-id="7c0d9-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-136">The following is an example of the response.</span></span> 

><span data-ttu-id="7c0d9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c0d9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7c0d9-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="7c0d9-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7c0d9-140">C#</span><span class="sxs-lookup"><span data-stu-id="7c0d9-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoff-delete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c0d9-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c0d9-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoff-delete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7c0d9-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7c0d9-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/timeoff-delete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoff-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
