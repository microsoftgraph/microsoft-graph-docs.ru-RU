---
title: Get timeOffRequest
description: Извлечение свойств и связей объекта timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 187dfaeeb6888c9717f6270166cbee61c6816082
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953934"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="c5bbc-103">Get timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="c5bbc-103">Get timeOffRequest</span></span>

<span data-ttu-id="c5bbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5bbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5bbc-105">Извлечение свойств и связей объекта [timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c5bbc-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5bbc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bbc-106">Permissions</span></span>

<span data-ttu-id="c5bbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5bbc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5bbc-109">Permission type</span></span>                        | <span data-ttu-id="c5bbc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5bbc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c5bbc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5bbc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5bbc-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5bbc-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c5bbc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5bbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5bbc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-114">Not supported.</span></span> |
|<span data-ttu-id="c5bbc-115">Application</span><span class="sxs-lookup"><span data-stu-id="c5bbc-115">Application</span></span> | <span data-ttu-id="c5bbc-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="c5bbc-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="c5bbc-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="c5bbc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5bbc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5bbc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c5bbc-119">Optional query parameters</span></span>

<span data-ttu-id="c5bbc-120">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5bbc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5bbc-121">Request headers</span></span>

| <span data-ttu-id="c5bbc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c5bbc-122">Name</span></span>      |<span data-ttu-id="c5bbc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c5bbc-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5bbc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5bbc-124">Authorization</span></span> | <span data-ttu-id="c5bbc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5bbc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5bbc-127">Request body</span></span>

<span data-ttu-id="c5bbc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5bbc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5bbc-129">Response</span></span>

<span data-ttu-id="c5bbc-130">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [timeOffRequest](../resources/timeoffrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5bbc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c5bbc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5bbc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5bbc-132">Request</span></span>

<span data-ttu-id="c5bbc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5bbc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5bbc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="c5bbc-135">C#</span><span class="sxs-lookup"><span data-stu-id="c5bbc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5bbc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5bbc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5bbc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5bbc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5bbc-138">Java</span><span class="sxs-lookup"><span data-stu-id="c5bbc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5bbc-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5bbc-139">Response</span></span>

<span data-ttu-id="c5bbc-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-140">The following is an example of the response.</span></span>

> <span data-ttu-id="c5bbc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5bbc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


