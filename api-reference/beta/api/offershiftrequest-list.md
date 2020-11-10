---
title: Список Оффершифтрекуест
description: Получение свойств и связей всех объектов Оффершифтрекуест в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 244c96b26cc55ac4cc727979517ab5ce75b0c509
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981288"
---
# <a name="list-offershiftrequest"></a><span data-ttu-id="1908b-103">Список Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="1908b-103">List offerShiftRequest</span></span>

<span data-ttu-id="1908b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1908b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1908b-105">Получение свойств и связей всех объектов [оффершифтрекуест](../resources/offershiftrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="1908b-105">Retrieve the properties and relationships of all [offerShiftRequest](../resources/offershiftrequest.md) objects in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1908b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1908b-106">Permissions</span></span>

<span data-ttu-id="1908b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1908b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1908b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1908b-109">Permission type</span></span>                        | <span data-ttu-id="1908b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1908b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1908b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1908b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1908b-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1908b-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1908b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1908b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1908b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1908b-114">Not supported.</span></span> |
| <span data-ttu-id="1908b-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1908b-115">Application</span></span>                            | <span data-ttu-id="1908b-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1908b-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1908b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1908b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1908b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1908b-118">Optional query parameters</span></span>

<span data-ttu-id="1908b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1908b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1908b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1908b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1908b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1908b-121">Request headers</span></span>

| <span data-ttu-id="1908b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1908b-122">Name</span></span>      |<span data-ttu-id="1908b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1908b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1908b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1908b-124">Authorization</span></span> | <span data-ttu-id="1908b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1908b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1908b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1908b-127">Request body</span></span>

<span data-ttu-id="1908b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1908b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1908b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1908b-129">Response</span></span>

<span data-ttu-id="1908b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1908b-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1908b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1908b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1908b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1908b-132">Request</span></span>

<span data-ttu-id="1908b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1908b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1908b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1908b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests
```
# <a name="c"></a>[<span data-ttu-id="1908b-135">C#</span><span class="sxs-lookup"><span data-stu-id="1908b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1908b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1908b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1908b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1908b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1908b-138">Java</span><span class="sxs-lookup"><span data-stu-id="1908b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1908b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1908b-139">Response</span></span>

<span data-ttu-id="1908b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1908b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1908b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1908b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


