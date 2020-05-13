---
title: Получение расписания
description: Получение свойств и связей объекта **расписания** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 705c42339dc64ff66f89ce72715d51a6753357d0
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44154250"
---
# <a name="get-schedule"></a><span data-ttu-id="5cab2-103">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="5cab2-103">Get schedule</span></span>

<span data-ttu-id="5cab2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cab2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cab2-105">Получение свойств и связей объекта [расписания](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="5cab2-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="5cab2-106">Процесс создания расписания соответствует [одной рекомендации API для долгосрочных операций, выполняемых на основе ресурсов (РЕЛО)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="5cab2-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="5cab2-107">Когда клиенты используют [метод PUT](team-put-schedule.md), если расписание подготовлено, операция обновляет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="5cab2-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="5cab2-108">Во время подготовки расписания клиенты могут использовать метод GET для получения расписания и просмотра `provisionStatus` свойства для текущего состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="5cab2-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="5cab2-109">Если не удалось выполнить подготовку, клиенты могут получить дополнительные сведения из `provisionStatusCode` Свойства.</span><span class="sxs-lookup"><span data-stu-id="5cab2-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="5cab2-110">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="5cab2-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cab2-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5cab2-111">Permissions</span></span>

<span data-ttu-id="5cab2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cab2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cab2-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cab2-114">Permission type</span></span>      | <span data-ttu-id="5cab2-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cab2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cab2-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cab2-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5cab2-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cab2-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5cab2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cab2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cab2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cab2-119">Not supported.</span></span>    |
|<span data-ttu-id="5cab2-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cab2-120">Application</span></span> | <span data-ttu-id="5cab2-121">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="5cab2-121">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="5cab2-122">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="5cab2-122">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="5cab2-123">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="5cab2-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5cab2-124">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="5cab2-124">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5cab2-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cab2-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cab2-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5cab2-126">Optional query parameters</span></span>

<span data-ttu-id="5cab2-127">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5cab2-127">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5cab2-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cab2-128">Request headers</span></span>

| <span data-ttu-id="5cab2-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cab2-129">Header</span></span>       | <span data-ttu-id="5cab2-130">Значение</span><span class="sxs-lookup"><span data-stu-id="5cab2-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5cab2-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5cab2-131">Authorization</span></span>  | <span data-ttu-id="5cab2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cab2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5cab2-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5cab2-134">Content-Type</span></span>  | <span data-ttu-id="5cab2-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5cab2-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cab2-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cab2-137">Request body</span></span>
<span data-ttu-id="5cab2-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cab2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cab2-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cab2-139">Response</span></span>

<span data-ttu-id="5cab2-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Schedule](../resources/schedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cab2-140">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cab2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5cab2-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5cab2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cab2-142">Request</span></span>

<span data-ttu-id="5cab2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cab2-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5cab2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="5cab2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```
# <a name="c"></a>[<span data-ttu-id="5cab2-145">C#</span><span class="sxs-lookup"><span data-stu-id="5cab2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5cab2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cab2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5cab2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cab2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5cab2-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cab2-148">Response</span></span>

<span data-ttu-id="5cab2-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5cab2-149">The following is an example of the response.</span></span> 

><span data-ttu-id="5cab2-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5cab2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
