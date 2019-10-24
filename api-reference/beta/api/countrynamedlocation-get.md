---
title: Получение Каунтринамедлокатион
description: Получение свойств и связей объекта Каунтринамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f5b557b7dd5a3f892a8bf2c81a92c83ba67d5a7c
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653694"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="306fd-103">Получение Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="306fd-103">Get countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="306fd-104">Получение свойств и связей объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="306fd-104">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="306fd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="306fd-105">Permissions</span></span>

<span data-ttu-id="306fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="306fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="306fd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="306fd-108">Permission type</span></span>                        | <span data-ttu-id="306fd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="306fd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="306fd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="306fd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="306fd-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="306fd-111">Policy.Read.All</span></span> |
| <span data-ttu-id="306fd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="306fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="306fd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="306fd-113">Not supported.</span></span> |
| <span data-ttu-id="306fd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="306fd-114">Application</span></span>                            | <span data-ttu-id="306fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="306fd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="306fd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="306fd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="306fd-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="306fd-117">Optional query parameters</span></span>

<span data-ttu-id="306fd-118">Этот метод поддерживает параметр `select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="306fd-118">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="306fd-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="306fd-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="306fd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="306fd-120">Request headers</span></span>

| <span data-ttu-id="306fd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="306fd-121">Name</span></span>      |<span data-ttu-id="306fd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="306fd-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="306fd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="306fd-123">Authorization</span></span> | <span data-ttu-id="306fd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="306fd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="306fd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="306fd-126">Request body</span></span>

<span data-ttu-id="306fd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="306fd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="306fd-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="306fd-128">Response</span></span>

<span data-ttu-id="306fd-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [каунтринамедлокатион](../resources/countrynamedlocation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="306fd-129">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="306fd-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="306fd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="306fd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="306fd-131">Request</span></span>

<span data-ttu-id="306fd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="306fd-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```http
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```

### <a name="response"></a><span data-ttu-id="306fd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="306fd-133">Response</span></span>

<span data-ttu-id="306fd-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="306fd-134">The following is an example of the response.</span></span>

> <span data-ttu-id="306fd-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="306fd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "id": "1c4427fd-0885-4a3d-8b23-09a899ffa959",
    "displayName": "Named location with unknown countries and regions",
    "modifiedDateTime": "2019-09-04T01:08:02.5249255Z",
    "createdDateTime": "2019-09-04T01:08:02.5249255Z",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get countryNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
