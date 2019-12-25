---
title: Создание или замена расписания
description: Создание или замена объекта **расписания** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fb45a560356b6f0ba536bd44ed869f0797677f35
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864959"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="9bbaa-103">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="9bbaa-103">Create or replace schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bbaa-104">Создание или замена объекта [расписания](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="9bbaa-104">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="9bbaa-105">Процесс создания расписания соответствует [одной рекомендации API для долгосрочных операций, выполняемых на основе ресурсов (РЕЛО)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="9bbaa-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="9bbaa-106">Когда клиенты используют метод PUT, если расписание подготовлено, операция заменяет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-106">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="9bbaa-107">Во время подготовки расписания клиенты могут использовать [метод Get](schedule-get.md) для получения расписания и просмотра `provisionStatus` свойства для текущего состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-107">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="9bbaa-108">Если не удалось выполнить подготовку, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="9bbaa-109">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-109">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="9bbaa-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bbaa-110">Permissions</span></span>

<span data-ttu-id="9bbaa-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bbaa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bbaa-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bbaa-113">Permission type</span></span>      | <span data-ttu-id="9bbaa-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bbaa-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bbaa-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bbaa-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9bbaa-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bbaa-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9bbaa-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bbaa-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bbaa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-118">Not supported.</span></span>    |
|<span data-ttu-id="9bbaa-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="9bbaa-119">Application</span></span> | <span data-ttu-id="9bbaa-120">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="9bbaa-120">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="9bbaa-121">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-121">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="9bbaa-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9bbaa-123">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-123">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9bbaa-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bbaa-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="9bbaa-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bbaa-125">Request headers</span></span>

| <span data-ttu-id="9bbaa-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bbaa-126">Header</span></span>       | <span data-ttu-id="9bbaa-127">Значение</span><span class="sxs-lookup"><span data-stu-id="9bbaa-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9bbaa-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9bbaa-128">Authorization</span></span>  | <span data-ttu-id="9bbaa-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9bbaa-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bbaa-131">Content-Type</span></span>  | <span data-ttu-id="9bbaa-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9bbaa-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bbaa-134">Request body</span></span>

<span data-ttu-id="9bbaa-135">В тексте запроса добавьте представление объекта [расписания](../resources/schedule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-135">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9bbaa-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bbaa-136">Response</span></span>

<span data-ttu-id="9bbaa-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Schedule](../resources/schedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-137">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bbaa-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9bbaa-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9bbaa-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bbaa-139">Request</span></span>

<span data-ttu-id="9bbaa-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9bbaa-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bbaa-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9bbaa-142">C#</span><span class="sxs-lookup"><span data-stu-id="9bbaa-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-put-schedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9bbaa-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bbaa-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-put-schedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9bbaa-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bbaa-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-put-schedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9bbaa-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bbaa-145">Response</span></span>

<span data-ttu-id="9bbaa-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-146">The following is an example of the response.</span></span> 

><span data-ttu-id="9bbaa-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "provisionStatusCode": null,
  "timeClockEnabled": true,
  "openShiftsEnabled": true,
  "swapShiftsRequestsEnabled": true,
  "offerShiftRequestsEnabled": true,
  "timeOffRequestsEnabled": true
}
```

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
  ]
}
-->
