---
title: Создание namedLocation
description: Создайте новое имяLocation.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8a6bab90f795259fd2e52610008744434e7f6247
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437571"
---
# <a name="create-namedlocation"></a><span data-ttu-id="d2964-103">Создание namedLocation</span><span class="sxs-lookup"><span data-stu-id="d2964-103">Create namedLocation</span></span>

<span data-ttu-id="d2964-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2964-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2964-105">Создайте новый [объект с именемLocation.](../resources/namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="d2964-105">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2964-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2964-106">Permissions</span></span>

<span data-ttu-id="d2964-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2964-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2964-109">Permission type</span></span>                        | <span data-ttu-id="d2964-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2964-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2964-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2964-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2964-112">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="d2964-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="d2964-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2964-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2964-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2964-114">Not supported.</span></span> |
| <span data-ttu-id="d2964-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2964-115">Application</span></span>                            | <span data-ttu-id="d2964-116">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="d2964-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2964-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2964-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="d2964-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2964-118">Request headers</span></span>

| <span data-ttu-id="d2964-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d2964-119">Name</span></span>          | <span data-ttu-id="d2964-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d2964-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d2964-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2964-121">Authorization</span></span> | <span data-ttu-id="d2964-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2964-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2964-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2964-124">Content-Type</span></span>  | <span data-ttu-id="d2964-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2964-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2964-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2964-127">Request body</span></span>

<span data-ttu-id="d2964-128">В теле запроса укажи представление JSON объекта [ipNamedLocation](../resources/ipnamedlocation.md) или [countryNamedLocation.](../resources/countrynamedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="d2964-128">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d2964-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2964-129">Response</span></span>

<span data-ttu-id="d2964-130">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект ipNamedLocation](../resources/ipnamedlocation.md) или [объект countryNamedLocation](../resources/countrynamedlocation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2964-130">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2964-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2964-131">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="d2964-132">Пример 1. Создание ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d2964-132">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="d2964-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2964-133">Request</span></span>

<span data-ttu-id="d2964-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2964-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2964-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2964-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "displayName": "Untrusted IP named location",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="d2964-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2964-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-namedlocation-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2964-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2964-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-namedlocation-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d2964-138">C#</span><span class="sxs-lookup"><span data-stu-id="d2964-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-namedlocation-from-conditionalaccessroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2964-139">Java</span><span class="sxs-lookup"><span data-stu-id="d2964-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-namedlocation-from-conditionalaccessroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d2964-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2964-140">Response</span></span>

<span data-ttu-id="d2964-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2964-141">The following is an example of the response.</span></span>

> <span data-ttu-id="d2964-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2964-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "id": "0854951d-5fc0-4eb1-b392-9b2c9d7949c2",
    "displayName": "Untrusted IP named location",
    "modifiedDateTime": "2019-09-04T01:11:34.9387578Z",
    "createdDateTime": "2019-09-04T01:11:34.9387578Z",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="d2964-144">Пример 2. Создание страныNamedLocation</span><span class="sxs-lookup"><span data-stu-id="d2964-144">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="d2964-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2964-145">Request</span></span>

<span data-ttu-id="d2964-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2964-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Named location with unknown countries and regions",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```

#### <a name="response"></a><span data-ttu-id="d2964-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2964-147">Response</span></span>

<span data-ttu-id="d2964-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2964-148">The following is an example of the response.</span></span>

> <span data-ttu-id="d2964-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2964-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Create namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


