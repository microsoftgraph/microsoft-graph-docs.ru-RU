---
title: Получить offerShiftRequest
description: Извлечение свойств и связей объекта offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7e3e26ab6978e3af3d30a4d2a6fca038ac954949
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051139"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="42e1d-103">Получить offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="42e1d-103">Get offerShiftRequest</span></span>

<span data-ttu-id="42e1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42e1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42e1d-105">Извлечение свойств и связей объекта [offerShiftRequest.](../resources/offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="42e1d-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42e1d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42e1d-106">Permissions</span></span>

<span data-ttu-id="42e1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42e1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42e1d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42e1d-109">Permission type</span></span>                        | <span data-ttu-id="42e1d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42e1d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="42e1d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42e1d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42e1d-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42e1d-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="42e1d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42e1d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42e1d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42e1d-114">Not supported.</span></span> |
| <span data-ttu-id="42e1d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="42e1d-115">Application</span></span>                            | <span data-ttu-id="42e1d-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42e1d-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42e1d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42e1d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42e1d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42e1d-118">Optional query parameters</span></span>

<span data-ttu-id="42e1d-119">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="42e1d-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42e1d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42e1d-120">Request headers</span></span>

| <span data-ttu-id="42e1d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="42e1d-121">Name</span></span>      |<span data-ttu-id="42e1d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="42e1d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42e1d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42e1d-123">Authorization</span></span> | <span data-ttu-id="42e1d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42e1d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42e1d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42e1d-126">Request body</span></span>

<span data-ttu-id="42e1d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42e1d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42e1d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="42e1d-128">Response</span></span>

<span data-ttu-id="42e1d-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [offerShiftRequest](../resources/offershiftrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="42e1d-129">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42e1d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="42e1d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42e1d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="42e1d-131">Request</span></span>

<span data-ttu-id="42e1d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42e1d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42e1d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="42e1d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="42e1d-134">C#</span><span class="sxs-lookup"><span data-stu-id="42e1d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42e1d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42e1d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42e1d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42e1d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42e1d-137">Java</span><span class="sxs-lookup"><span data-stu-id="42e1d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42e1d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="42e1d-138">Response</span></span>

<span data-ttu-id="42e1d-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="42e1d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="42e1d-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="42e1d-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientActionMessage": "recipientActionMessage-value",
  "recipientActionDateTime": "datetime-value",
  "senderShiftId": "senderShiftId-value",
  "recipientUserId": "recipientUserId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


