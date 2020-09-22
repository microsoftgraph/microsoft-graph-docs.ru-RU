---
title: Получение Тимеоффрекуест
description: Получение свойств и связей объекта тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 267710b78fed5abfb83e7c9492c7bdff603b91d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058606"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="f205e-103">Получение Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="f205e-103">Get timeOffRequest</span></span>

<span data-ttu-id="f205e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f205e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f205e-105">Получение свойств и связей объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="f205e-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f205e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f205e-106">Permissions</span></span>

<span data-ttu-id="f205e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f205e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f205e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f205e-109">Permission type</span></span>                        | <span data-ttu-id="f205e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f205e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f205e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f205e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f205e-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f205e-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f205e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f205e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f205e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f205e-114">Not supported.</span></span> |
|<span data-ttu-id="f205e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f205e-115">Application</span></span> | <span data-ttu-id="f205e-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="f205e-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="f205e-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="f205e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="f205e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f205e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f205e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f205e-119">Optional query parameters</span></span>

<span data-ttu-id="f205e-120">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f205e-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f205e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f205e-121">Request headers</span></span>

| <span data-ttu-id="f205e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f205e-122">Name</span></span>      |<span data-ttu-id="f205e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f205e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f205e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f205e-124">Authorization</span></span> | <span data-ttu-id="f205e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f205e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f205e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f205e-127">Request body</span></span>

<span data-ttu-id="f205e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f205e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f205e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f205e-129">Response</span></span>

<span data-ttu-id="f205e-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [тимеоффрекуест](../resources/timeoffrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f205e-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f205e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f205e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f205e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f205e-132">Request</span></span>

<span data-ttu-id="f205e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f205e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f205e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f205e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="f205e-135">C#</span><span class="sxs-lookup"><span data-stu-id="f205e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f205e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f205e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f205e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f205e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f205e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f205e-138">Response</span></span>

<span data-ttu-id="f205e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f205e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f205e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f205e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Get timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


