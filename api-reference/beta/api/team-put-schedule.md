---
title: Создание или замена расписания
description: Создание или замена объекта **расписания** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d6cc676638dcdbf8c6fca462726df6479f06dd52
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270751"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="f074e-103">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="f074e-103">Create or replace schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f074e-104">Создание или замена объекта [расписания](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="f074e-104">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="f074e-105">Процесс создания расписания соответствует [одной рекомендации API для долгосрочных операций, выполняемых на основе ресурсов (РЕЛО)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="f074e-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="f074e-106">Когда клиенты используют метод PUT, если расписание подготовлено, операция заменяет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="f074e-106">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="f074e-107">Во время подготовки расписания клиенты могут использовать [метод Get](schedule-get.md) для получения расписания и просмотра `provisionStatus` свойства для текущего состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="f074e-107">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="f074e-108">Если не удалось выполнить подготовку, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.</span><span class="sxs-lookup"><span data-stu-id="f074e-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="f074e-109">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="f074e-109">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="f074e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f074e-110">Permissions</span></span>

<span data-ttu-id="f074e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f074e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f074e-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f074e-113">Permission type</span></span>      | <span data-ttu-id="f074e-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f074e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f074e-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f074e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f074e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f074e-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f074e-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f074e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f074e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f074e-118">Not supported.</span></span>    |
|<span data-ttu-id="f074e-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f074e-119">Application</span></span> | <span data-ttu-id="f074e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f074e-120">Not supported.</span></span> |

> <span data-ttu-id="f074e-121">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f074e-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f074e-122">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="f074e-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f074e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f074e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="f074e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f074e-124">Request headers</span></span>

| <span data-ttu-id="f074e-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f074e-125">Header</span></span>       | <span data-ttu-id="f074e-126">Значение</span><span class="sxs-lookup"><span data-stu-id="f074e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f074e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f074e-127">Authorization</span></span>  | <span data-ttu-id="f074e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f074e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f074e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f074e-130">Content-Type</span></span>  | <span data-ttu-id="f074e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f074e-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f074e-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f074e-132">Request body</span></span>

<span data-ttu-id="f074e-133">В тексте запроса добавьте представление объекта [расписания](../resources/schedule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f074e-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f074e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f074e-134">Response</span></span>

<span data-ttu-id="f074e-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Schedule](../resources/schedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f074e-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f074e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f074e-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f074e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f074e-137">Request</span></span>

<span data-ttu-id="f074e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f074e-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```

#### <a name="response"></a><span data-ttu-id="f074e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f074e-139">Response</span></span>

<span data-ttu-id="f074e-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f074e-140">The following is an example of the response.</span></span> 

><span data-ttu-id="f074e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f074e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f074e-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f074e-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f074e-144">C#</span><span class="sxs-lookup"><span data-stu-id="f074e-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/team-put-schedule-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f074e-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="f074e-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/team-put-schedule-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f074e-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f074e-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/team-put-schedule-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-put-schedule.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/team-put-schedule.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/team-put-schedule.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
