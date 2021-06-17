---
title: Создание или замена расписания
description: Создание или замена объекта **расписания.**
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4fcde2a694646bcdb363c23315a77a931072ed24
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992459"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="cf4db-103">Создание или замена расписания</span><span class="sxs-lookup"><span data-stu-id="cf4db-103">Create or replace schedule</span></span>

<span data-ttu-id="cf4db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf4db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf4db-105">Создание или замена объекта [расписания.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="cf4db-105">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="cf4db-106">Процесс создания расписания соответствует рекомендациям One API для длительных операций на основе ресурсов [(RELO).](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)</span><span class="sxs-lookup"><span data-stu-id="cf4db-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="cf4db-107">Если клиенты используют метод PUT, если расписание является предварительным, операция заменяет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="cf4db-107">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="cf4db-108">При расписании клиенты могут использовать метод [GET,](schedule-get.md) чтобы получить расписание и посмотреть свойство для текущего состояния `provisionStatus` подготовка.</span><span class="sxs-lookup"><span data-stu-id="cf4db-108">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="cf4db-109">Если подготовка не удалась, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.</span><span class="sxs-lookup"><span data-stu-id="cf4db-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="cf4db-110">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="cf4db-110">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="cf4db-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf4db-111">Permissions</span></span>

<span data-ttu-id="cf4db-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf4db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf4db-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf4db-114">Permission type</span></span>      | <span data-ttu-id="cf4db-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf4db-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf4db-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf4db-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cf4db-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4db-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf4db-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf4db-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf4db-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf4db-119">Not supported.</span></span>    |
|<span data-ttu-id="cf4db-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf4db-120">Application</span></span> | <span data-ttu-id="cf4db-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf4db-121">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf4db-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf4db-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="cf4db-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf4db-123">Request headers</span></span>

| <span data-ttu-id="cf4db-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf4db-124">Header</span></span>       | <span data-ttu-id="cf4db-125">Значение</span><span class="sxs-lookup"><span data-stu-id="cf4db-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf4db-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf4db-126">Authorization</span></span>  | <span data-ttu-id="cf4db-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf4db-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cf4db-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf4db-129">Content-Type</span></span>  | <span data-ttu-id="cf4db-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf4db-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf4db-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf4db-132">Request body</span></span>

<span data-ttu-id="cf4db-133">В теле запроса поставляем JSON-представление объекта [расписания.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="cf4db-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cf4db-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf4db-134">Response</span></span>

<span data-ttu-id="cf4db-135">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [расписания](../resources/schedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf4db-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf4db-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="cf4db-136">Examples</span></span>

### <a name="example-1-update-a-schedule"></a><span data-ttu-id="cf4db-137">Пример 1. Обновление расписания</span><span class="sxs-lookup"><span data-stu-id="cf4db-137">Example 1: Update a schedule</span></span>

#### <a name="request"></a><span data-ttu-id="cf4db-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf4db-138">Request</span></span>

<span data-ttu-id="cf4db-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf4db-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf4db-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf4db-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cf4db-141">C#</span><span class="sxs-lookup"><span data-stu-id="cf4db-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-put-schedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf4db-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf4db-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-put-schedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf4db-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf4db-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-put-schedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf4db-144">Java</span><span class="sxs-lookup"><span data-stu-id="cf4db-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-put-schedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cf4db-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf4db-145">Response</span></span>

<span data-ttu-id="cf4db-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf4db-146">The following is an example of the response.</span></span> 

><span data-ttu-id="cf4db-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cf4db-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-enable-location-detection-for-time-clock"></a><span data-ttu-id="cf4db-148">Пример 2. Включить обнаружение местоположения для часов времени</span><span class="sxs-lookup"><span data-stu-id="cf4db-148">Example 2: Enable location detection for time clock</span></span>

#### <a name="request"></a><span data-ttu-id="cf4db-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf4db-149">Request</span></span>

<span data-ttu-id="cf4db-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf4db-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cf4db-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf4db-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-put-schedule-2"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule

{
   "enabled":true,
   "timeZone":"America/Chicago",
   "provisionStatus":"Completed",
   "provisionStatusCode":null,
   "openShiftsEnabled":true,
   "swapShiftsRequestsEnabled":true,
   "offerShiftRequestsEnabled":true,
   "timeOffRequestsEnabled":true,
   "timeClockEnabled":true,
   "timeClockSettings":{
      "approvedLocation":{
         "altitude":1024.13,
         "latitude":26.13246,
         "longitude":24.34616
      }
   }
} 
```
# <a name="c"></a>[<span data-ttu-id="cf4db-152">C#</span><span class="sxs-lookup"><span data-stu-id="cf4db-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-put-schedule-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf4db-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf4db-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-put-schedule-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf4db-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf4db-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-put-schedule-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf4db-155">Java</span><span class="sxs-lookup"><span data-stu-id="cf4db-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-put-schedule-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cf4db-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf4db-156">Response</span></span>

<span data-ttu-id="cf4db-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf4db-157">The following is an example of the response.</span></span> 

><span data-ttu-id="cf4db-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cf4db-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "enabled":true,
   "timeZone":"America/Chicago",
   "provisionStatus":"Completed",
   "provisionStatusCode":null,
   "openShiftsEnabled":true,
   "swapShiftsRequestsEnabled":true,
   "offerShiftRequestsEnabled":true,
   "timeOffRequestsEnabled":true,
   "timeClockEnabled":true,
   "timeClockSettings":{
      "approvedLocation":{
         "altitude":1024.13,
         "latitude":26.13246,
         "longitude":24.34616
      }
   }
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


