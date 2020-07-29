---
title: Получение Ревиевсеткуери
description: Получение свойств и связей объекта ревиевсеткуери обнаружения электронных данных.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 8add5af1daa40d1bce177cb22b3c44242ea0a0c4
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510282"
---
# <a name="get-reviewsetquery"></a><span data-ttu-id="5556c-103">Получение Ревиевсеткуери</span><span class="sxs-lookup"><span data-stu-id="5556c-103">Get reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5556c-104">Получение свойств и связей объекта [Ревиевсеткуери](../resources/reviewsetquery.md) обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="5556c-104">Retrieve the properties and relationships of an eDiscovery [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5556c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5556c-105">Permissions</span></span>

<span data-ttu-id="5556c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5556c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5556c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5556c-108">Permission type</span></span>                        | <span data-ttu-id="5556c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5556c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5556c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5556c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5556c-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="5556c-111">User.Read</span></span> |
| <span data-ttu-id="5556c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5556c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5556c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5556c-113">Not supported.</span></span> |
| <span data-ttu-id="5556c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5556c-114">Application</span></span>                            | <span data-ttu-id="5556c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5556c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5556c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5556c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5556c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5556c-117">Optional query parameters</span></span>

<span data-ttu-id="5556c-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5556c-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5556c-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5556c-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5556c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5556c-120">Request headers</span></span>

| <span data-ttu-id="5556c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5556c-121">Name</span></span>      |<span data-ttu-id="5556c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5556c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5556c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5556c-123">Authorization</span></span> | <span data-ttu-id="5556c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5556c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5556c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5556c-126">Request body</span></span>

<span data-ttu-id="5556c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5556c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5556c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5556c-128">Response</span></span>

<span data-ttu-id="5556c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [ревиевсеткуери](../resources/reviewsetquery.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5556c-129">If successful, this method returns a `200 OK` response code and the requested [reviewSetQuery](../resources/reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5556c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5556c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5556c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5556c-131">Request</span></span>

<span data-ttu-id="5556c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5556c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reviewsetquery"
}-->

```http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```

### <a name="response"></a><span data-ttu-id="5556c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5556c-133">Response</span></span>

<span data-ttu-id="5556c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5556c-134">The following is an example of the response.</span></span>

> <span data-ttu-id="5556c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5556c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries/$entity",
    "id": "6b5358b0-2ce2-4369-b9cf-65392fe56807",
    "displayName": "My Query 1",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-09T09:05:12.3756813Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-03-09T09:05:12.3756813Z",
    "query": "subject:\"Quarterly Financials\""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
