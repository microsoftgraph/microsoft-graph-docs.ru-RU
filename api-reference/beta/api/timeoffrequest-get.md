---
title: Get timeOffRequest
description: Извлечение свойств и связей объекта timeoffrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c961704a21112dbd738102ea0ab14c81bbd3a28f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048941"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="2f4c4-103">Get timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="2f4c4-103">Get timeOffRequest</span></span>

<span data-ttu-id="2f4c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f4c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f4c4-105">Извлечение свойств и связей объекта [timeoffrequest.](../resources/timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2f4c4-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f4c4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f4c4-106">Permissions</span></span>

<span data-ttu-id="2f4c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f4c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f4c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f4c4-109">Permission type</span></span>                        | <span data-ttu-id="2f4c4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f4c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f4c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f4c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f4c4-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f4c4-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2f4c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f4c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f4c4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-114">Not supported.</span></span> |
|<span data-ttu-id="2f4c4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2f4c4-115">Application</span></span> | <span data-ttu-id="2f4c4-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="2f4c4-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="2f4c4-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f4c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f4c4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f4c4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f4c4-119">Optional query parameters</span></span>

<span data-ttu-id="2f4c4-120">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f4c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f4c4-121">Request headers</span></span>

| <span data-ttu-id="2f4c4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2f4c4-122">Name</span></span>      |<span data-ttu-id="2f4c4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2f4c4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2f4c4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f4c4-124">Authorization</span></span> | <span data-ttu-id="2f4c4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f4c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f4c4-127">Request body</span></span>

<span data-ttu-id="2f4c4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f4c4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f4c4-129">Response</span></span>

<span data-ttu-id="2f4c4-130">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [timeOffRequest](../resources/timeoffrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-130">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f4c4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="2f4c4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f4c4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f4c4-132">Request</span></span>

<span data-ttu-id="2f4c4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f4c4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f4c4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="2f4c4-135">C#</span><span class="sxs-lookup"><span data-stu-id="2f4c4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f4c4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f4c4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f4c4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f4c4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f4c4-138">Java</span><span class="sxs-lookup"><span data-stu-id="2f4c4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f4c4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f4c4-139">Response</span></span>

<span data-ttu-id="2f4c4-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-140">The following is an example of the response.</span></span>

> <span data-ttu-id="2f4c4-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2f4c4-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


