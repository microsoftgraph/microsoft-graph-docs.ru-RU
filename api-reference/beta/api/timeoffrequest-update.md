---
title: Обновление тимеоффрекуест
description: Обновление свойств объекта тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8d5a230f11bfd9d4727821d54f723a2e30de40be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452248"
---
# <a name="update-timeoffrequest"></a><span data-ttu-id="a6fe7-103">Обновление тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="a6fe7-103">Update timeoffrequest</span></span>

<span data-ttu-id="a6fe7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6fe7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6fe7-105">Обновление свойств объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a6fe7-105">Update the properties of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6fe7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6fe7-106">Permissions</span></span>

<span data-ttu-id="a6fe7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6fe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6fe7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6fe7-109">Permission type</span></span>                        | <span data-ttu-id="a6fe7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6fe7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a6fe7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6fe7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6fe7-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6fe7-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a6fe7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6fe7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6fe7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-114">Not supported.</span></span> |
|<span data-ttu-id="a6fe7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6fe7-115">Application</span></span> | <span data-ttu-id="a6fe7-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="a6fe7-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="a6fe7-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="a6fe7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6fe7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="a6fe7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6fe7-119">Request headers</span></span>

| <span data-ttu-id="a6fe7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a6fe7-120">Name</span></span>       | <span data-ttu-id="a6fe7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a6fe7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a6fe7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6fe7-122">Authorization</span></span> | <span data-ttu-id="a6fe7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6fe7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6fe7-125">Content-type</span></span> | <span data-ttu-id="a6fe7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6fe7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6fe7-128">Request body</span></span>

<span data-ttu-id="a6fe7-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a6fe7-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a6fe7-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a6fe7-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6fe7-132">Property</span></span>     | <span data-ttu-id="a6fe7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a6fe7-133">Type</span></span>        | <span data-ttu-id="a6fe7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a6fe7-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a6fe7-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a6fe7-135">endDateTime</span></span>|<span data-ttu-id="a6fe7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6fe7-136">DateTimeOffset</span></span>|<span data-ttu-id="a6fe7-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a6fe7-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a6fe7-138">Например, полночь UTC 1 января 2014: ' ' 2014 – 01 – 01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="a6fe7-138">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="a6fe7-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a6fe7-139">startDateTime</span></span>|<span data-ttu-id="a6fe7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6fe7-140">DateTimeOffset</span></span>|<span data-ttu-id="a6fe7-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a6fe7-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a6fe7-142">Например, полночь UTC 1 января 2014: ' ' 2014 – 01 – 01T00:00:00Z '</span><span class="sxs-lookup"><span data-stu-id="a6fe7-142">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="a6fe7-143">тимеоффреасонид</span><span class="sxs-lookup"><span data-stu-id="a6fe7-143">timeOffReasonId</span></span>|<span data-ttu-id="a6fe7-144">String</span><span class="sxs-lookup"><span data-stu-id="a6fe7-144">String</span></span>|<span data-ttu-id="a6fe7-145">Причина для запрошенного времени.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-145">Reason for the requested time off.</span></span>|

## <a name="response"></a><span data-ttu-id="a6fe7-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6fe7-146">Response</span></span>

<span data-ttu-id="a6fe7-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [тимеоффрекуест](../resources/timeoffrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-147">If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6fe7-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="a6fe7-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6fe7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6fe7-149">Request</span></span>

<span data-ttu-id="a6fe7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6fe7-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6fe7-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6fe7-152">C#</span><span class="sxs-lookup"><span data-stu-id="a6fe7-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6fe7-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6fe7-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6fe7-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6fe7-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6fe7-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6fe7-155">Response</span></span>

<span data-ttu-id="a6fe7-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-156">The following is an example of the response.</span></span>

> <span data-ttu-id="a6fe7-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6fe7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
