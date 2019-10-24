---
title: Создание Намедлокатион
description: Создание нового Намедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5d6962a9cae9eb3a49177ecaa4d17a0c4181881
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653729"
---
# <a name="create-namedlocation"></a><span data-ttu-id="8e8a7-103">Создание Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="8e8a7-103">Create namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e8a7-104">Создание нового объекта [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="8e8a7-104">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e8a7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e8a7-105">Permissions</span></span>

<span data-ttu-id="8e8a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e8a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e8a7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e8a7-108">Permission type</span></span>                        | <span data-ttu-id="8e8a7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e8a7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e8a7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e8a7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e8a7-111">Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="8e8a7-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8e8a7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e8a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e8a7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-113">Not supported.</span></span> |
| <span data-ttu-id="8e8a7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e8a7-114">Application</span></span>                            | <span data-ttu-id="8e8a7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="8e8a7-116">Этот API требует нескольких разрешений.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-116">This API requires multiple permissions.</span></span> <span data-ttu-id="8e8a7-117">Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="8e8a7-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="8e8a7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e8a7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="8e8a7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e8a7-119">Request headers</span></span>

| <span data-ttu-id="8e8a7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8e8a7-120">Name</span></span>          | <span data-ttu-id="8e8a7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8e8a7-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e8a7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e8a7-122">Authorization</span></span> | <span data-ttu-id="8e8a7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e8a7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e8a7-125">Content-Type</span></span>  | <span data-ttu-id="8e8a7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e8a7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e8a7-128">Request body</span></span>

<span data-ttu-id="8e8a7-129">В тексте запроса добавьте представление объекта [ипнамедлокатион](../resources/ipnamedlocation.md) или [КАУНТРИНАМЕДЛОКАТИОН](../resources/countrynamedlocation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-129">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8e8a7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e8a7-130">Response</span></span>

<span data-ttu-id="8e8a7-131">В случае успешного выполнения этот метод возвращает `201 Created`код отклика и новый объект [ипнамедлокатион](../resources/ipnamedlocation.md) или [каунтринамедлокатион](../resources/countrynamedlocation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-131">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e8a7-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="8e8a7-132">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="8e8a7-133">Пример 1: создание Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="8e8a7-133">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="8e8a7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e8a7-134">Request</span></span>

<span data-ttu-id="8e8a7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-135">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="8e8a7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e8a7-136">Response</span></span>

<span data-ttu-id="8e8a7-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8e8a7-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="8e8a7-140">Пример 2: создание объекта Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="8e8a7-140">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="8e8a7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e8a7-141">Request</span></span>

<span data-ttu-id="8e8a7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-142">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="8e8a7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e8a7-143">Response</span></span>

<span data-ttu-id="8e8a7-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-144">The following is an example of the response.</span></span>

> <span data-ttu-id="8e8a7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e8a7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
