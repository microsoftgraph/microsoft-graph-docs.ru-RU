---
title: Обновление тимеоффрекуест
description: Обновление свойств объекта тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2197e0e4e2f9c78337a6d5ae06d6c1e106f77afa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863543"
---
# <a name="update-timeoffrequest"></a><span data-ttu-id="6d566-103">Обновление тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="6d566-103">Update timeoffrequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d566-104">Обновление свойств объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="6d566-104">Update the properties of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d566-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d566-105">Permissions</span></span>

<span data-ttu-id="6d566-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d566-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d566-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d566-108">Permission type</span></span>                        | <span data-ttu-id="6d566-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d566-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6d566-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d566-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d566-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d566-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6d566-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d566-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d566-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d566-113">Not supported.</span></span> |
|<span data-ttu-id="6d566-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="6d566-114">Application</span></span> | <span data-ttu-id="6d566-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="6d566-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="6d566-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d566-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="6d566-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d566-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="6d566-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d566-118">Request headers</span></span>

| <span data-ttu-id="6d566-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6d566-119">Name</span></span>       | <span data-ttu-id="6d566-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6d566-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6d566-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d566-121">Authorization</span></span> | <span data-ttu-id="6d566-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d566-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6d566-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d566-124">Content-type</span></span> | <span data-ttu-id="6d566-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d566-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d566-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d566-127">Request body</span></span>

<span data-ttu-id="6d566-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6d566-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6d566-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6d566-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6d566-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6d566-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6d566-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d566-131">Property</span></span>     | <span data-ttu-id="6d566-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6d566-132">Type</span></span>        | <span data-ttu-id="6d566-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6d566-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d566-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6d566-134">endDateTime</span></span>|<span data-ttu-id="6d566-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d566-135">DateTimeOffset</span></span>|<span data-ttu-id="6d566-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6d566-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d566-137">Например, полночь UTC 1 января 2014: ' ' 2014 – 01 – 01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="6d566-137">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="6d566-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6d566-138">startDateTime</span></span>|<span data-ttu-id="6d566-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d566-139">DateTimeOffset</span></span>|<span data-ttu-id="6d566-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6d566-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d566-141">Например, полночь UTC 1 января 2014: ' ' 2014 – 01 – 01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="6d566-141">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="6d566-142">тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="6d566-142">timeOffReasonId</span></span>|<span data-ttu-id="6d566-143">String</span><span class="sxs-lookup"><span data-stu-id="6d566-143">String</span></span>|<span data-ttu-id="6d566-144">Причина для запрошенного времени.</span><span class="sxs-lookup"><span data-stu-id="6d566-144">Reason for the requested time off.</span></span>|

## <a name="response"></a><span data-ttu-id="6d566-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d566-145">Response</span></span>

<span data-ttu-id="6d566-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [тимеоффрекуест](../resources/timeoffrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d566-146">If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d566-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="6d566-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d566-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d566-148">Request</span></span>

<span data-ttu-id="6d566-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d566-149">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6d566-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d566-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d566-151">C#</span><span class="sxs-lookup"><span data-stu-id="6d566-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d566-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d566-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d566-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d566-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d566-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d566-154">Response</span></span>

<span data-ttu-id="6d566-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6d566-155">The following is an example of the response.</span></span>

> <span data-ttu-id="6d566-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d566-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
