---
title: Получение Едисковерикасе
description: Получение свойств и связей объекта едисковерикасе.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 258019d4c675b39f4450e05e5846f4f5414c10d5
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510210"
---
# <a name="get-ediscoverycase"></a><span data-ttu-id="b9d79-103">Получение Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="b9d79-103">Get ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9d79-104">Получение свойств и связей объекта [едисковерикасе](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="b9d79-104">Retrieve the properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9d79-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9d79-105">Permissions</span></span>

<span data-ttu-id="b9d79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9d79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9d79-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9d79-108">Permission type</span></span>                        | <span data-ttu-id="b9d79-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9d79-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9d79-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9d79-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9d79-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="b9d79-111">User.Read</span></span>      |
| <span data-ttu-id="b9d79-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9d79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9d79-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9d79-113">Not supported.</span></span> |
| <span data-ttu-id="b9d79-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9d79-114">Application</span></span>                            | <span data-ttu-id="b9d79-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9d79-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9d79-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9d79-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9d79-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9d79-117">Optional query parameters</span></span>

<span data-ttu-id="b9d79-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b9d79-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b9d79-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b9d79-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9d79-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9d79-120">Request headers</span></span>

| <span data-ttu-id="b9d79-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b9d79-121">Name</span></span>      |<span data-ttu-id="b9d79-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b9d79-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9d79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9d79-123">Authorization</span></span> | <span data-ttu-id="b9d79-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b9d79-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9d79-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9d79-125">Request body</span></span>

<span data-ttu-id="b9d79-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9d79-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9d79-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9d79-127">Response</span></span>

<span data-ttu-id="b9d79-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [едисковерикасе](../resources/ediscoverycase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9d79-128">If successful, this method returns a `200 OK` response code and the requested [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9d79-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9d79-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9d79-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9d79-130">Request</span></span>

<span data-ttu-id="b9d79-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9d79-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ediscoverycase"
}-->

```http
GET https://graph.microsoft.com/beta/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

### <a name="response"></a><span data-ttu-id="b9d79-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9d79-132">Response</span></span>

<span data-ttu-id="b9d79-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9d79-133">The following is an example of the response.</span></span>

> <span data-ttu-id="b9d79-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9d79-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->