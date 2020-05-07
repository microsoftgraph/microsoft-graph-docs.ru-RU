---
title: Получение расписания
description: Получение свойств и связей объекта **расписания** .
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fe5f2d72d43398893b366e4aa2632700df6649c6
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155175"
---
# <a name="get-schedule"></a><span data-ttu-id="f433f-103">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="f433f-103">Get schedule</span></span>

<span data-ttu-id="f433f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f433f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f433f-105">Получение свойств и связей объекта [расписания](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="f433f-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="f433f-106">Процесс создания расписания соответствует [одной рекомендации API для долгосрочных операций, выполняемых на основе ресурсов (РЕЛО)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="f433f-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="f433f-107">Когда клиенты используют [метод PUT](team-put-schedule.md), если расписание подготовлено, операция обновляет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="f433f-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="f433f-108">Во время подготовки расписания клиенты могут использовать метод GET для получения расписания и просмотра `provisionStatus` свойства для текущего состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="f433f-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="f433f-109">Если не удалось выполнить подготовку, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.</span><span class="sxs-lookup"><span data-stu-id="f433f-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="f433f-110">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="f433f-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="f433f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f433f-111">Permissions</span></span>

<span data-ttu-id="f433f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f433f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f433f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f433f-114">Permission type</span></span>      | <span data-ttu-id="f433f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f433f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f433f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f433f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f433f-117">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f433f-117">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f433f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f433f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f433f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f433f-119">Not supported.</span></span>    |<span data-ttu-id="f433f-120">s</span><span class="sxs-lookup"><span data-stu-id="f433f-120">s</span></span>
|<span data-ttu-id="f433f-121">Application</span><span class="sxs-lookup"><span data-stu-id="f433f-121">Application</span></span> | <span data-ttu-id="f433f-122">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f433f-122">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="f433f-123">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f433f-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f433f-124">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="f433f-124">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f433f-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f433f-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f433f-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f433f-126">Optional query parameters</span></span>

<span data-ttu-id="f433f-127">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f433f-127">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f433f-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f433f-128">Request headers</span></span>

| <span data-ttu-id="f433f-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f433f-129">Header</span></span>       | <span data-ttu-id="f433f-130">Значение</span><span class="sxs-lookup"><span data-stu-id="f433f-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f433f-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f433f-131">Authorization</span></span>  | <span data-ttu-id="f433f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f433f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f433f-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f433f-134">Content-Type</span></span>  | <span data-ttu-id="f433f-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f433f-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f433f-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f433f-137">Request body</span></span>
<span data-ttu-id="f433f-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f433f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f433f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f433f-139">Response</span></span>

<span data-ttu-id="f433f-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Schedule](../resources/schedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f433f-140">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f433f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f433f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f433f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f433f-142">Request</span></span>

<span data-ttu-id="f433f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f433f-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule
```
---


### <a name="response"></a><span data-ttu-id="f433f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f433f-144">Response</span></span>

<span data-ttu-id="f433f-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f433f-145">The following is an example of the response.</span></span> 

><span data-ttu-id="f433f-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f433f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
