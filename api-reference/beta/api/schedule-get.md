---
title: Получение расписания
description: Получение свойств и связей объекта **расписания** .
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1c658ff9df1dab5f4a751c524dedb1f2fa8b3ac4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868865"
---
# <a name="get-schedule"></a><span data-ttu-id="0ea45-103">Получение расписания</span><span class="sxs-lookup"><span data-stu-id="0ea45-103">Get schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea45-104">Получение свойств и связей объекта [расписания](../resources/schedule.md) .</span><span class="sxs-lookup"><span data-stu-id="0ea45-104">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="0ea45-105">Процесс создания расписания соответствует [одной рекомендации API для долгосрочных операций, выполняемых на основе ресурсов (РЕЛО)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="0ea45-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="0ea45-106">Когда клиенты используют [метод PUT](team-put-schedule.md), если расписание подготовлено, операция обновляет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="0ea45-106">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="0ea45-107">Во время подготовки расписания клиенты могут использовать метод GET для получения расписания и просмотра `provisionStatus` свойства для текущего состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="0ea45-107">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="0ea45-108">Если не удалось выполнить подготовку, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.</span><span class="sxs-lookup"><span data-stu-id="0ea45-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="0ea45-109">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="0ea45-109">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea45-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea45-110">Permissions</span></span>

<span data-ttu-id="0ea45-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ea45-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea45-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea45-113">Permission type</span></span>      | <span data-ttu-id="0ea45-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ea45-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea45-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ea45-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea45-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea45-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0ea45-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ea45-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea45-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ea45-118">Not supported.</span></span>    |
|<span data-ttu-id="0ea45-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ea45-119">Application</span></span> | <span data-ttu-id="0ea45-120">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="0ea45-120">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="0ea45-121">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="0ea45-121">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="0ea45-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="0ea45-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0ea45-123">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="0ea45-123">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0ea45-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ea45-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="0ea45-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ea45-125">Request headers</span></span>

| <span data-ttu-id="0ea45-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ea45-126">Header</span></span>       | <span data-ttu-id="0ea45-127">Значение</span><span class="sxs-lookup"><span data-stu-id="0ea45-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0ea45-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ea45-128">Authorization</span></span>  | <span data-ttu-id="0ea45-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ea45-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0ea45-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ea45-131">Content-Type</span></span>  | <span data-ttu-id="0ea45-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ea45-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ea45-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ea45-134">Request body</span></span>
<span data-ttu-id="0ea45-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ea45-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea45-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ea45-136">Response</span></span>

<span data-ttu-id="0ea45-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Schedule](../resources/schedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ea45-137">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea45-138">Пример</span><span class="sxs-lookup"><span data-stu-id="0ea45-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0ea45-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ea45-139">Request</span></span>

<span data-ttu-id="0ea45-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ea45-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ea45-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea45-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ea45-142">C#</span><span class="sxs-lookup"><span data-stu-id="0ea45-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ea45-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ea45-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ea45-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ea45-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ea45-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ea45-145">Response</span></span>

<span data-ttu-id="0ea45-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ea45-146">The following is an example of the response.</span></span> 

><span data-ttu-id="0ea45-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ea45-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
