---
title: Получение Свапшифтсчанжерекуест
description: Получение свойств и связей объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d0968813f16ff4280bcd2319495ceeb98572df6f
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895818"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="2c86e-103">Получение Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="2c86e-103">Get swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c86e-104">Получение свойств и связей объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="2c86e-104">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c86e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c86e-105">Permissions</span></span>

<span data-ttu-id="2c86e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c86e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c86e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c86e-108">Permission type</span></span>                        | <span data-ttu-id="2c86e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c86e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c86e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c86e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c86e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c86e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2c86e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c86e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c86e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c86e-113">Not supported.</span></span> |
| <span data-ttu-id="2c86e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c86e-114">Application</span></span>                            | <span data-ttu-id="2c86e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c86e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c86e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c86e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c86e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2c86e-117">Optional query parameters</span></span>

<span data-ttu-id="2c86e-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2c86e-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2c86e-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2c86e-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c86e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c86e-120">Request headers</span></span>

| <span data-ttu-id="2c86e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2c86e-121">Name</span></span>      |<span data-ttu-id="2c86e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2c86e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c86e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c86e-123">Authorization</span></span> | <span data-ttu-id="2c86e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c86e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c86e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c86e-126">Request body</span></span>

<span data-ttu-id="2c86e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c86e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c86e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c86e-128">Response</span></span>

<span data-ttu-id="2c86e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c86e-129">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c86e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2c86e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2c86e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c86e-131">Request</span></span>

<span data-ttu-id="2c86e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c86e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="2c86e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c86e-133">Response</span></span>

<span data-ttu-id="2c86e-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c86e-134">The following is an example of the response.</span></span>

> <span data-ttu-id="2c86e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c86e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
