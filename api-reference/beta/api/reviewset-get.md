---
title: Получение представления
description: Получение свойств и связей объекта Review.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: a5ad5609e1d4645bf984870fde6ad1996cb487e2
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510345"
---
# <a name="get-reviewset"></a><span data-ttu-id="2d9c3-103">Получение представления</span><span class="sxs-lookup"><span data-stu-id="2d9c3-103">Get reviewSet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d9c3-104">Получение свойств и связей объекта [Review](../resources/reviewset.md) .</span><span class="sxs-lookup"><span data-stu-id="2d9c3-104">Retrieve the properties and relationships of a [reviewSet](../resources/reviewset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d9c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d9c3-105">Permissions</span></span>

<span data-ttu-id="2d9c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d9c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d9c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d9c3-108">Permission type</span></span>                        | <span data-ttu-id="2d9c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d9c3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2d9c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d9c3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d9c3-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="2d9c3-111">User.Read</span></span> |
| <span data-ttu-id="2d9c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d9c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d9c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-113">Not supported.</span></span> |
| <span data-ttu-id="2d9c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d9c3-114">Application</span></span>                            | <span data-ttu-id="2d9c3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d9c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d9c3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d9c3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d9c3-117">Optional query parameters</span></span>

<span data-ttu-id="2d9c3-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2d9c3-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2d9c3-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="2d9c3-120">По умолчанию возвращаются все поля набора проверки; Однако вы можете указать, какие поля необходимо возвращать с помощью `$select` параметра запроса OData.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-120">By default, all review set fields are returned; however, you can specify certain fields to return using the OData `$select` query parameter.</span></span>  <span data-ttu-id="2d9c3-121">Например, чтобы возвращались только **DisplayName** и ID, добавьте в запрос следующее: `$select=displayName,Id` .</span><span class="sxs-lookup"><span data-stu-id="2d9c3-121">For example, to only return the **displayName** and ID, add the following to your query: `$select=displayName,Id`.</span></span>

<span data-ttu-id="2d9c3-122">Так как запрос может вернуть много обращений, можно отфильтровать их с помощью **DisplayName**.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-122">Because a request can return many cases, you can filter them by using **displayName**.</span></span>  <span data-ttu-id="2d9c3-123">Чтобы выполнить фильтрацию по **DisplayName**, добавьте в запрос следующее: `$filter=displayName eq 'rs1'` , где имя набора проверки — RS1.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-123">To filter by **displayName**, add the following to your query: `$filter=displayName eq 'rs1'`, where the review set name is rs1.</span></span>

<span data-ttu-id="2d9c3-124">Дополнительные сведения о фильтрации и указании полей можно узнать [в статье Использование выражений фильтров в URI OData ](https://docs.microsoft.com/dynamics-nav/using-filter-expressions-in-odata-uris).</span><span class="sxs-lookup"><span data-stu-id="2d9c3-124">For more information about filtering and specifying fields, see [Using Filter Expressions in OData URIs ](https://docs.microsoft.com/dynamics-nav/using-filter-expressions-in-odata-uris).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d9c3-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d9c3-125">Request headers</span></span>

| <span data-ttu-id="2d9c3-126">Имя</span><span class="sxs-lookup"><span data-stu-id="2d9c3-126">Name</span></span>      |<span data-ttu-id="2d9c3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2d9c3-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2d9c3-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d9c3-128">Authorization</span></span> | <span data-ttu-id="2d9c3-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d9c3-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d9c3-131">Request body</span></span>

<span data-ttu-id="2d9c3-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d9c3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9c3-133">Response</span></span>

<span data-ttu-id="2d9c3-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Review](../resources/reviewset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-134">If successful, this method returns a `200 OK` response code and the requested [reviewSet](../resources/reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d9c3-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d9c3-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d9c3-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d9c3-136">Request</span></span>

<span data-ttu-id="2d9c3-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reviewset"
}-->

```http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e
```

### <a name="response"></a><span data-ttu-id="2d9c3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d9c3-138">Response</span></span>

<span data-ttu-id="2d9c3-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-139">The following is an example of the response.</span></span>

> <span data-ttu-id="2d9c3-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d9c3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d')/reviewSets/$entity",
    "id": "0157910c-57ce-4e48-bd4b-90f3c88ca32e",
    "displayName": "My Reviewset 3",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-11T08:40:14.9486058Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
