---
title: Получить расписание
description: Извлечение свойств и связей объекта **расписания.**
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ec152a26d9ed7fe250334c931217726ff88e4e54
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053897"
---
# <a name="get-schedule"></a><span data-ttu-id="a14d5-103">Получить расписание</span><span class="sxs-lookup"><span data-stu-id="a14d5-103">Get schedule</span></span>

<span data-ttu-id="a14d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a14d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a14d5-105">Извлечение свойств и связей объекта [расписания.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="a14d5-105">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="a14d5-106">Процесс создания расписания соответствует рекомендациям One API для длительных операций на основе ресурсов [(RELO).](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)</span><span class="sxs-lookup"><span data-stu-id="a14d5-106">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="a14d5-107">Когда клиенты используют [метод PUT,](team-put-schedule.md)если расписание запланировали, операция обновляет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="a14d5-107">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="a14d5-108">При расписании клиенты могут использовать метод GET, чтобы получить расписание и посмотреть свойство для текущего состояния `provisionStatus` подготовка.</span><span class="sxs-lookup"><span data-stu-id="a14d5-108">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="a14d5-109">Если подготовка не удалась, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.</span><span class="sxs-lookup"><span data-stu-id="a14d5-109">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="a14d5-110">Клиенты также могут проверить конфигурацию расписания.</span><span class="sxs-lookup"><span data-stu-id="a14d5-110">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="a14d5-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a14d5-111">Permissions</span></span>

<span data-ttu-id="a14d5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a14d5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a14d5-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a14d5-114">Permission type</span></span>                        | <span data-ttu-id="a14d5-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a14d5-115">Permissions (from least to most privileged)</span></span>                                    |
|:---------------------------------------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="a14d5-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a14d5-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="a14d5-117">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a14d5-117">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a14d5-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a14d5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a14d5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a14d5-119">Not supported.</span></span>                                                                 |
| <span data-ttu-id="a14d5-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="a14d5-120">Application</span></span>                            | <span data-ttu-id="a14d5-121">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a14d5-121">Schedule.Read.All, Schedule.ReadWrite.All</span></span>                                      |

## <a name="http-request"></a><span data-ttu-id="a14d5-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a14d5-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a14d5-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a14d5-123">Optional query parameters</span></span>

<span data-ttu-id="a14d5-124">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a14d5-124">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a14d5-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a14d5-125">Request headers</span></span>

| <span data-ttu-id="a14d5-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a14d5-126">Header</span></span>       | <span data-ttu-id="a14d5-127">Значение</span><span class="sxs-lookup"><span data-stu-id="a14d5-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a14d5-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a14d5-128">Authorization</span></span>  | <span data-ttu-id="a14d5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a14d5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a14d5-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a14d5-131">Content-Type</span></span>  | <span data-ttu-id="a14d5-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a14d5-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a14d5-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a14d5-134">Request body</span></span>
<span data-ttu-id="a14d5-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a14d5-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a14d5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a14d5-136">Response</span></span>

<span data-ttu-id="a14d5-137">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [расписания](../resources/schedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a14d5-137">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a14d5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a14d5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a14d5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a14d5-139">Request</span></span>

<span data-ttu-id="a14d5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a14d5-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a14d5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a14d5-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule
```
# <a name="c"></a>[<span data-ttu-id="a14d5-142">C#</span><span class="sxs-lookup"><span data-stu-id="a14d5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a14d5-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a14d5-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a14d5-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a14d5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a14d5-145">Java</span><span class="sxs-lookup"><span data-stu-id="a14d5-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="a14d5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a14d5-146">Response</span></span>

<span data-ttu-id="a14d5-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a14d5-147">The following is an example of the response.</span></span>

><span data-ttu-id="a14d5-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a14d5-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

