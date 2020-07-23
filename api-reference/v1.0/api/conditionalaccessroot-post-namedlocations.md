---
title: Создание Намедлокатион
description: Создание нового Намедлокатион.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 99b81875c2d7df1f2b8f5fabd164c626f7af6a26
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384795"
---
# <a name="create-namedlocation"></a><span data-ttu-id="8b99c-103">Создание Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="8b99c-103">Create namedLocation</span></span>

<span data-ttu-id="8b99c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b99c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b99c-105">Создание нового объекта [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="8b99c-105">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b99c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b99c-106">Permissions</span></span>

<span data-ttu-id="8b99c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b99c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b99c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b99c-109">Permission type</span></span>                        | <span data-ttu-id="8b99c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b99c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b99c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b99c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b99c-112">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="8b99c-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="8b99c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b99c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b99c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b99c-114">Not supported.</span></span> |
| <span data-ttu-id="8b99c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b99c-115">Application</span></span>                            | <span data-ttu-id="8b99c-116">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="8b99c-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b99c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b99c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="8b99c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b99c-118">Request headers</span></span>

| <span data-ttu-id="8b99c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8b99c-119">Name</span></span>          | <span data-ttu-id="8b99c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8b99c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8b99c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b99c-121">Authorization</span></span> | <span data-ttu-id="8b99c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b99c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b99c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b99c-124">Content-Type</span></span>  | <span data-ttu-id="8b99c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b99c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b99c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b99c-127">Request body</span></span>

<span data-ttu-id="8b99c-128">В тексте запроса добавьте представление объекта [ипнамедлокатион](../resources/ipnamedlocation.md) или [КАУНТРИНАМЕДЛОКАТИОН](../resources/countrynamedlocation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b99c-128">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8b99c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b99c-129">Response</span></span>

<span data-ttu-id="8b99c-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [Ипнамедлокатион](../resources/ipnamedlocation.md) или [каунтринамедлокатион](../resources/countrynamedlocation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b99c-130">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b99c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b99c-131">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="8b99c-132">Пример 1: создание Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="8b99c-132">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="8b99c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b99c-133">Request</span></span>

<span data-ttu-id="8b99c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b99c-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
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

#### <a name="response"></a><span data-ttu-id="8b99c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b99c-135">Response</span></span>

<span data-ttu-id="8b99c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b99c-136">The following is an example of the response.</span></span>

> <span data-ttu-id="8b99c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b99c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
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
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="8b99c-139">Пример 2: создание объекта Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="8b99c-139">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="8b99c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b99c-140">Request</span></span>

<span data-ttu-id="8b99c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b99c-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
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

#### <a name="response"></a><span data-ttu-id="8b99c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b99c-142">Response</span></span>

<span data-ttu-id="8b99c-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b99c-143">The following is an example of the response.</span></span>

> <span data-ttu-id="8b99c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b99c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
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
