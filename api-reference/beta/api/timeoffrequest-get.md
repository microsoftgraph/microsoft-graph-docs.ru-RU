---
title: Получение Тимеоффрекуест
description: Получение свойств и связей объекта тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 29c2ac88bf1253d3a00a395d990f1974bda50815
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895800"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="5554b-103">Получение Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="5554b-103">Get timeOffRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5554b-104">Получение свойств и связей объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="5554b-104">Retrieve the properties and relationships of [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5554b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5554b-105">Permissions</span></span>

<span data-ttu-id="5554b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5554b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5554b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5554b-108">Permission type</span></span>                        | <span data-ttu-id="5554b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5554b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5554b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5554b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5554b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5554b-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5554b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5554b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5554b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5554b-113">Not supported.</span></span> |
| <span data-ttu-id="5554b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5554b-114">Application</span></span>                            | <span data-ttu-id="5554b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5554b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5554b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5554b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5554b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5554b-117">Optional query parameters</span></span>

<span data-ttu-id="5554b-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5554b-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5554b-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5554b-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5554b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5554b-120">Request headers</span></span>

| <span data-ttu-id="5554b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5554b-121">Name</span></span>      |<span data-ttu-id="5554b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5554b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5554b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5554b-123">Authorization</span></span> | <span data-ttu-id="5554b-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5554b-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5554b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5554b-125">Request body</span></span>

<span data-ttu-id="5554b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5554b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5554b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5554b-127">Response</span></span>

<span data-ttu-id="5554b-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [тимеоффрекуест](../resources/timeoffrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5554b-128">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5554b-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="5554b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5554b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5554b-130">Request</span></span>

<span data-ttu-id="5554b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5554b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```

### <a name="response"></a><span data-ttu-id="5554b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5554b-132">Response</span></span>

<span data-ttu-id="5554b-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5554b-133">The following is an example of the response.</span></span>

> <span data-ttu-id="5554b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5554b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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