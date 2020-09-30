---
title: Список Оффершифтрекуест
description: Получение свойств и связей всех объектов Оффершифтрекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7ed2eaaa150bbb708fdc45c6078493f30f471488
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313739"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="5c923-103">Список Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="5c923-103">List offerShiftRequest</span></span>

<span data-ttu-id="5c923-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c923-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c923-105">Получение свойств и связей всех объектов [оффершифтрекуест](../resources/offershiftrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="5c923-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c923-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c923-106">Permissions</span></span>

<span data-ttu-id="5c923-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c923-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c923-109">Permission type</span></span>                        | <span data-ttu-id="5c923-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c923-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5c923-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c923-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c923-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5c923-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5c923-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c923-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c923-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c923-114">Not supported.</span></span> |
| <span data-ttu-id="5c923-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c923-115">Application</span></span>                            | <span data-ttu-id="5c923-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c923-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c923-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c923-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c923-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c923-118">Optional query parameters</span></span>

<span data-ttu-id="5c923-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5c923-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c923-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5c923-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c923-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c923-121">Request headers</span></span>

| <span data-ttu-id="5c923-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5c923-122">Name</span></span>      |<span data-ttu-id="5c923-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5c923-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c923-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c923-124">Authorization</span></span> | <span data-ttu-id="5c923-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c923-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c923-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c923-127">Request body</span></span>

<span data-ttu-id="5c923-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c923-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c923-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c923-129">Response</span></span>

<span data-ttu-id="5c923-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c923-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c923-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c923-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c923-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c923-132">Request</span></span>

<span data-ttu-id="5c923-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c923-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c923-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c923-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="5c923-135">C#</span><span class="sxs-lookup"><span data-stu-id="5c923-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c923-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c923-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c923-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c923-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5c923-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c923-138">Response</span></span>

<span data-ttu-id="5c923-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5c923-139">The following is an example of the response.</span></span>

> <span data-ttu-id="5c923-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c923-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


