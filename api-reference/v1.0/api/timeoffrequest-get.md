---
title: Get timeOffRequest
description: Извлечение свойств и связей объекта timeOffRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a55e4b9bda896084d177cef09908807162284c26
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963592"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="dd126-103">Get timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="dd126-103">Get timeOffRequest</span></span>

<span data-ttu-id="dd126-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd126-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd126-105">Извлечение свойств и связей объекта [timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="dd126-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd126-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd126-106">Permissions</span></span>

<span data-ttu-id="dd126-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd126-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd126-109">Permission type</span></span>                        | <span data-ttu-id="dd126-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd126-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="dd126-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd126-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd126-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd126-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dd126-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd126-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd126-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd126-114">Not supported.</span></span>    |
|<span data-ttu-id="dd126-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd126-115">Application</span></span> | <span data-ttu-id="dd126-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd126-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="dd126-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="dd126-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="dd126-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="dd126-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="dd126-119">в настоящее время только в закрытом предварительном просмотре и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="dd126-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="dd126-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd126-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd126-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd126-121">Optional query parameters</span></span>

<span data-ttu-id="dd126-122">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd126-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd126-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd126-123">Request headers</span></span>

| <span data-ttu-id="dd126-124">Имя</span><span class="sxs-lookup"><span data-stu-id="dd126-124">Name</span></span>      |<span data-ttu-id="dd126-125">Описание</span><span class="sxs-lookup"><span data-stu-id="dd126-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd126-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd126-126">Authorization</span></span> | <span data-ttu-id="dd126-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd126-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd126-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd126-129">Request body</span></span>

<span data-ttu-id="dd126-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd126-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd126-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd126-131">Response</span></span>

<span data-ttu-id="dd126-132">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [timeOffRequest](../resources/timeoffrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd126-132">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd126-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd126-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd126-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd126-134">Request</span></span>

<span data-ttu-id="dd126-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd126-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dd126-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd126-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="dd126-137">C#</span><span class="sxs-lookup"><span data-stu-id="dd126-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd126-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd126-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd126-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd126-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd126-140">Java</span><span class="sxs-lookup"><span data-stu-id="dd126-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="dd126-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd126-141">Response</span></span>

<span data-ttu-id="dd126-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd126-142">The following is an example of the response.</span></span>

> <span data-ttu-id="dd126-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd126-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

