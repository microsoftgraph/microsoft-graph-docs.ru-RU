---
title: Получение Оффершифтрекуест
description: Получение свойств и связей объекта Оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 37ef0a62174ab2464993025ab170eedc42d904af
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313669"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="f4e06-103">Получение Оффершифтрекуест</span><span class="sxs-lookup"><span data-stu-id="f4e06-103">Get offerShiftRequest</span></span>

<span data-ttu-id="f4e06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4e06-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4e06-105">Получение свойств и связей объекта [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="f4e06-105">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4e06-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4e06-106">Permissions</span></span>

<span data-ttu-id="f4e06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4e06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4e06-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4e06-109">Permission type</span></span>                        | <span data-ttu-id="f4e06-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4e06-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f4e06-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4e06-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4e06-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f4e06-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f4e06-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4e06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4e06-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4e06-114">Not supported.</span></span> |
| <span data-ttu-id="f4e06-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4e06-115">Application</span></span>                            | <span data-ttu-id="f4e06-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f4e06-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4e06-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4e06-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4e06-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f4e06-118">Optional query parameters</span></span>

<span data-ttu-id="f4e06-119">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f4e06-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4e06-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4e06-120">Request headers</span></span>

| <span data-ttu-id="f4e06-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f4e06-121">Name</span></span>      |<span data-ttu-id="f4e06-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f4e06-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4e06-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4e06-123">Authorization</span></span> | <span data-ttu-id="f4e06-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4e06-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4e06-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4e06-126">Request body</span></span>

<span data-ttu-id="f4e06-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4e06-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4e06-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4e06-128">Response</span></span>

<span data-ttu-id="f4e06-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [оффершифтрекуест](../resources/offershiftrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4e06-129">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4e06-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f4e06-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4e06-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4e06-131">Request</span></span>

<span data-ttu-id="f4e06-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4e06-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4e06-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4e06-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}
```
# <a name="c"></a>[<span data-ttu-id="f4e06-134">C#</span><span class="sxs-lookup"><span data-stu-id="f4e06-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-offershiftrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4e06-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4e06-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-offershiftrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4e06-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4e06-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-offershiftrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4e06-137">Java</span><span class="sxs-lookup"><span data-stu-id="f4e06-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-offershiftrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="f4e06-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4e06-138">Response</span></span>

<span data-ttu-id="f4e06-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f4e06-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f4e06-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4e06-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

