---
title: Создание или замена расписания
description: Создание или замена объекта **расписания** .
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b5999fd3728dafe65e1832a632ce27d314b3d8b3
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154180"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="7b6f4-103">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="7b6f4-103">Create or replace schedule</span></span>

<span data-ttu-id="7b6f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b6f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b6f4-105">Создание или замена объекта [расписания](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="7b6f4-105">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="7b6f4-106">Процесс создания расписания соответствует [одной рекомендации API для долгосрочных операций, выполняемых на основе ресурсов (РЕЛО)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="7b6f4-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="7b6f4-107">Когда клиенты используют метод PUT, если расписание подготовлено, операция заменяет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-107">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="7b6f4-108">Во время подготовки расписания клиенты могут использовать [метод Get](schedule-get.md) для получения расписания и просмотра `provisionStatus` свойства для текущего состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-108">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="7b6f4-109">Если не удалось выполнить подготовку, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="7b6f4-110">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-110">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="7b6f4-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b6f4-111">Permissions</span></span>

<span data-ttu-id="7b6f4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b6f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b6f4-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b6f4-114">Permission type</span></span>      | <span data-ttu-id="7b6f4-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b6f4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b6f4-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b6f4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7b6f4-117">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7b6f4-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b6f4-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b6f4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b6f4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-119">Not supported.</span></span>    |
|<span data-ttu-id="7b6f4-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b6f4-120">Application</span></span> | <span data-ttu-id="7b6f4-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b6f4-121">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="7b6f4-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7b6f4-123">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-123">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7b6f4-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b6f4-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="7b6f4-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b6f4-125">Request headers</span></span>

| <span data-ttu-id="7b6f4-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b6f4-126">Header</span></span>       | <span data-ttu-id="7b6f4-127">Значение</span><span class="sxs-lookup"><span data-stu-id="7b6f4-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7b6f4-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b6f4-128">Authorization</span></span>  | <span data-ttu-id="7b6f4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7b6f4-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b6f4-131">Content-Type</span></span>  | <span data-ttu-id="7b6f4-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b6f4-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b6f4-134">Request body</span></span>

<span data-ttu-id="7b6f4-135">В тексте запроса добавьте представление объекта [расписания](../resources/schedule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-135">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7b6f4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b6f4-136">Response</span></span>

<span data-ttu-id="7b6f4-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Schedule](../resources/schedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-137">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b6f4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="7b6f4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b6f4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b6f4-139">Request</span></span>

<span data-ttu-id="7b6f4-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/v1/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```
---


### <a name="response"></a><span data-ttu-id="7b6f4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b6f4-141">Response</span></span>

<span data-ttu-id="7b6f4-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-142">The following is an example of the response.</span></span> 

><span data-ttu-id="7b6f4-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b6f4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
