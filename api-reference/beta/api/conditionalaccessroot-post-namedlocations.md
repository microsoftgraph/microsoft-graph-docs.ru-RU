---
title: Создание Намедлокатион
description: Создание нового Намедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 21927e1cc85048603217a1067d40274c5d6c80b7
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636780"
---
# <a name="create-namedlocation"></a><span data-ttu-id="ca3b0-103">Создание Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="ca3b0-103">Create namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca3b0-104">Создание нового объекта [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="ca3b0-104">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca3b0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca3b0-105">Permissions</span></span>

<span data-ttu-id="ca3b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca3b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca3b0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca3b0-108">Permission type</span></span>                        | <span data-ttu-id="ca3b0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca3b0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ca3b0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca3b0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca3b0-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="ca3b0-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="ca3b0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca3b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca3b0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-113">Not supported.</span></span> |
| <span data-ttu-id="ca3b0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca3b0-114">Application</span></span>                            | <span data-ttu-id="ca3b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca3b0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca3b0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="ca3b0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca3b0-117">Request headers</span></span>

| <span data-ttu-id="ca3b0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ca3b0-118">Name</span></span>          | <span data-ttu-id="ca3b0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ca3b0-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ca3b0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca3b0-120">Authorization</span></span> | <span data-ttu-id="ca3b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca3b0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca3b0-123">Content-Type</span></span>  | <span data-ttu-id="ca3b0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca3b0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca3b0-126">Request body</span></span>

<span data-ttu-id="ca3b0-127">В тексте запроса добавьте представление объекта [ипнамедлокатион](../resources/ipnamedlocation.md) или [КАУНТРИНАМЕДЛОКАТИОН](../resources/countrynamedlocation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-127">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ca3b0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca3b0-128">Response</span></span>

<span data-ttu-id="ca3b0-129">В случае успешного выполнения этот метод возвращает `201 Created`код отклика и новый объект [ипнамедлокатион](../resources/ipnamedlocation.md) или [каунтринамедлокатион](../resources/countrynamedlocation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-129">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca3b0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca3b0-130">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="ca3b0-131">Пример 1: создание Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="ca3b0-131">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="ca3b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca3b0-132">Request</span></span>

<span data-ttu-id="ca3b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ca3b0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca3b0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/namedLocations
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca3b0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca3b0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-namedlocation-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ca3b0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca3b0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-namedlocation-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca3b0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca3b0-137">Response</span></span>

<span data-ttu-id="ca3b0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ca3b0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="ca3b0-141">Пример 2: создание объекта Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="ca3b0-141">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="ca3b0-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca3b0-142">Request</span></span>

<span data-ttu-id="ca3b0-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/namedLocations
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

#### <a name="response"></a><span data-ttu-id="ca3b0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca3b0-144">Response</span></span>

<span data-ttu-id="ca3b0-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-145">The following is an example of the response.</span></span>

> <span data-ttu-id="ca3b0-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca3b0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
