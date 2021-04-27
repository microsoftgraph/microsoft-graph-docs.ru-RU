---
title: List offerShiftRequest
description: Извлечение свойств и связей всех объектов offerShiftRequest в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aff40c4a4801fd7f9cb6229f0073d9f7247f81e6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038280"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="4761f-103">List offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="4761f-103">List offerShiftRequest</span></span>

<span data-ttu-id="4761f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4761f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4761f-105">Извлечение свойств и связей всех [объектов offerShiftRequest](../resources/offershiftrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="4761f-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="4761f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4761f-106">Permissions</span></span>

<span data-ttu-id="4761f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4761f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4761f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4761f-109">Permission type</span></span>                        | <span data-ttu-id="4761f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4761f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4761f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4761f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4761f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4761f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4761f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4761f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4761f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4761f-114">Not supported.</span></span> |
| <span data-ttu-id="4761f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4761f-115">Application</span></span>                            | <span data-ttu-id="4761f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4761f-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4761f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4761f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4761f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4761f-118">Optional query parameters</span></span>

<span data-ttu-id="4761f-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4761f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4761f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4761f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4761f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4761f-121">Request headers</span></span>

| <span data-ttu-id="4761f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4761f-122">Name</span></span>      |<span data-ttu-id="4761f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4761f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4761f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4761f-124">Authorization</span></span> | <span data-ttu-id="4761f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4761f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4761f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4761f-127">Request body</span></span>

<span data-ttu-id="4761f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4761f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4761f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4761f-129">Response</span></span>

<span data-ttu-id="4761f-130">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [offerShiftRequest](../resources/offershiftrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4761f-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4761f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4761f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4761f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4761f-132">Request</span></span>

<span data-ttu-id="4761f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4761f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4761f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4761f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="4761f-135">C#</span><span class="sxs-lookup"><span data-stu-id="4761f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4761f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4761f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4761f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4761f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4761f-138">Java</span><span class="sxs-lookup"><span data-stu-id="4761f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4761f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4761f-139">Response</span></span>

<span data-ttu-id="4761f-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4761f-140">The following is an example of the response.</span></span>

> <span data-ttu-id="4761f-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4761f-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


