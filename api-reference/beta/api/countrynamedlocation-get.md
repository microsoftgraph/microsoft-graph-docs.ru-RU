---
title: Получение Каунтринамедлокатион
description: Получение свойств и связей объекта Каунтринамедлокатион.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f4a5c55cf4130e9a02afd102416c93efcee441f1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387071"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="db61c-103">Получение Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="db61c-103">Get countryNamedLocation</span></span>

<span data-ttu-id="db61c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db61c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db61c-105">Получение свойств и связей объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="db61c-105">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db61c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db61c-106">Permissions</span></span>

<span data-ttu-id="db61c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db61c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db61c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db61c-109">Permission type</span></span>                        | <span data-ttu-id="db61c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db61c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db61c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db61c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db61c-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="db61c-112">Policy.Read.All</span></span> |
| <span data-ttu-id="db61c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db61c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db61c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db61c-114">Not supported.</span></span> |
| <span data-ttu-id="db61c-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="db61c-115">Application</span></span>                            | <span data-ttu-id="db61c-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="db61c-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db61c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db61c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db61c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db61c-118">Optional query parameters</span></span>

<span data-ttu-id="db61c-119">Этот метод поддерживает параметр `select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="db61c-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="db61c-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="db61c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="db61c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db61c-121">Request headers</span></span>

| <span data-ttu-id="db61c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="db61c-122">Name</span></span>      |<span data-ttu-id="db61c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="db61c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db61c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db61c-124">Authorization</span></span> | <span data-ttu-id="db61c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db61c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db61c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db61c-127">Request body</span></span>

<span data-ttu-id="db61c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db61c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db61c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="db61c-129">Response</span></span>

<span data-ttu-id="db61c-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [каунтринамедлокатион](../resources/countrynamedlocation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db61c-130">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db61c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="db61c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db61c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="db61c-132">Request</span></span>

<span data-ttu-id="db61c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db61c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db61c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="db61c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="db61c-135">C#</span><span class="sxs-lookup"><span data-stu-id="db61c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db61c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db61c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db61c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db61c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db61c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="db61c-138">Response</span></span>

<span data-ttu-id="db61c-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db61c-139">The following is an example of the response.</span></span>

> <span data-ttu-id="db61c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db61c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
