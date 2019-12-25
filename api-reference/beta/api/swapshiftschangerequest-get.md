---
title: Получение Свапшифтсчанжерекуест
description: Получение свойств и связей объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e229fa0d85ab876a61cfff2958d3961f4b42637c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865065"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="dafeb-103">Получение Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="dafeb-103">Get swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dafeb-104">Получение свойств и связей объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="dafeb-104">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dafeb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dafeb-105">Permissions</span></span>

<span data-ttu-id="dafeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dafeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dafeb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dafeb-108">Permission type</span></span>                        | <span data-ttu-id="dafeb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dafeb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dafeb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dafeb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dafeb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dafeb-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="dafeb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dafeb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dafeb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dafeb-113">Not supported.</span></span> |
| <span data-ttu-id="dafeb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dafeb-114">Application</span></span>                            | <span data-ttu-id="dafeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dafeb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dafeb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dafeb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dafeb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dafeb-117">Optional query parameters</span></span>

<span data-ttu-id="dafeb-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dafeb-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dafeb-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dafeb-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dafeb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dafeb-120">Request headers</span></span>

| <span data-ttu-id="dafeb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dafeb-121">Name</span></span>      |<span data-ttu-id="dafeb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dafeb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dafeb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dafeb-123">Authorization</span></span> | <span data-ttu-id="dafeb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dafeb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dafeb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dafeb-126">Request body</span></span>

<span data-ttu-id="dafeb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dafeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dafeb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="dafeb-128">Response</span></span>

<span data-ttu-id="dafeb-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dafeb-129">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dafeb-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="dafeb-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dafeb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dafeb-131">Request</span></span>

<span data-ttu-id="dafeb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dafeb-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dafeb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dafeb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dafeb-134">C#</span><span class="sxs-lookup"><span data-stu-id="dafeb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dafeb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dafeb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dafeb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dafeb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dafeb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dafeb-137">Response</span></span>

<span data-ttu-id="dafeb-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dafeb-138">The following is an example of the response.</span></span>

> <span data-ttu-id="dafeb-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dafeb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientShiftId": "recipientShiftId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
