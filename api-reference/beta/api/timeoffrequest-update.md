---
title: Обновление тимеоффрекуест
description: Обновление свойств объекта тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4e961a197620f27de11397952c2d868dcec848c3
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895804"
---
# <a name="update-timeoffrequest"></a><span data-ttu-id="1f5c2-103">Обновление тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="1f5c2-103">Update timeoffrequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f5c2-104">Обновление свойств объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="1f5c2-104">Update the properties of [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f5c2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f5c2-105">Permissions</span></span>

<span data-ttu-id="1f5c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f5c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f5c2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f5c2-108">Permission type</span></span>                        | <span data-ttu-id="1f5c2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f5c2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f5c2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f5c2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f5c2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f5c2-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1f5c2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f5c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f5c2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-113">Not supported.</span></span> |
| <span data-ttu-id="1f5c2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f5c2-114">Application</span></span>                            | <span data-ttu-id="1f5c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f5c2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f5c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="1f5c2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f5c2-117">Request headers</span></span>

| <span data-ttu-id="1f5c2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1f5c2-118">Name</span></span>       | <span data-ttu-id="1f5c2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1f5c2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1f5c2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f5c2-120">Authorization</span></span> | <span data-ttu-id="1f5c2-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1f5c2-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f5c2-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f5c2-122">Request body</span></span>

<span data-ttu-id="1f5c2-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1f5c2-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1f5c2-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1f5c2-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f5c2-126">Property</span></span>     | <span data-ttu-id="1f5c2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1f5c2-127">Type</span></span>        | <span data-ttu-id="1f5c2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1f5c2-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f5c2-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5c2-129">endDateTime</span></span>|<span data-ttu-id="1f5c2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f5c2-130">DateTimeOffset</span></span>|<span data-ttu-id="1f5c2-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1f5c2-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f5c2-132">Например, полночь UTC 1 января 2014: ' ' 2014 – 01 – 01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="1f5c2-132">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="1f5c2-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5c2-133">startDateTime</span></span>|<span data-ttu-id="1f5c2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f5c2-134">DateTimeOffset</span></span>|<span data-ttu-id="1f5c2-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1f5c2-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f5c2-136">Например, полночь UTC 1 января 2014: ' ' 2014 – 01 – 01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="1f5c2-136">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="1f5c2-137">тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="1f5c2-137">timeOffReasonId</span></span>|<span data-ttu-id="1f5c2-138">String</span><span class="sxs-lookup"><span data-stu-id="1f5c2-138">String</span></span>|<span data-ttu-id="1f5c2-139">Причина для запрошенного времени.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-139">Reason for the requested time off.</span></span>|

## <a name="response"></a><span data-ttu-id="1f5c2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f5c2-140">Response</span></span>

<span data-ttu-id="1f5c2-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [тимеоффрекуест](../resources/timeoffrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-141">If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f5c2-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f5c2-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f5c2-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f5c2-143">Request</span></span>

<span data-ttu-id="1f5c2-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_timeoffrequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

### <a name="response"></a><span data-ttu-id="1f5c2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f5c2-145">Response</span></span>

<span data-ttu-id="1f5c2-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-146">The following is an example of the response.</span></span>

> <span data-ttu-id="1f5c2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f5c2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update timeoffrequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->