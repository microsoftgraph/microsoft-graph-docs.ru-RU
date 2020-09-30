---
title: Получение представления
description: Получение свойств и связей объекта Review.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 3a1192a9a14181a0c5a4dac9e067e6326dba60b4
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314096"
---
# <a name="get-reviewset"></a><span data-ttu-id="c7659-103">Получение представления</span><span class="sxs-lookup"><span data-stu-id="c7659-103">Get reviewSet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7659-104">Получение свойств и связей объекта [Review](../resources/reviewset.md) .</span><span class="sxs-lookup"><span data-stu-id="c7659-104">Retrieve the properties and relationships of a [reviewSet](../resources/reviewset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7659-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7659-105">Permissions</span></span>

<span data-ttu-id="c7659-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7659-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7659-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7659-108">Permission type</span></span>                        | <span data-ttu-id="c7659-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7659-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7659-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7659-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7659-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="c7659-111">User.Read</span></span> |
| <span data-ttu-id="c7659-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7659-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7659-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7659-113">Not supported.</span></span> |
| <span data-ttu-id="c7659-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7659-114">Application</span></span>                            | <span data-ttu-id="c7659-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7659-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7659-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7659-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7659-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7659-117">Optional query parameters</span></span>

<span data-ttu-id="c7659-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c7659-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c7659-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c7659-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="c7659-120">По умолчанию возвращаются все поля набора проверки; Однако вы можете указать, какие поля необходимо возвращать с помощью `$select` параметра запроса OData.</span><span class="sxs-lookup"><span data-stu-id="c7659-120">By default, all review set fields are returned; however, you can specify certain fields to return using the OData `$select` query parameter.</span></span>  <span data-ttu-id="c7659-121">Например, чтобы возвращались только **DisplayName** и ID, добавьте в запрос следующее: `$select=displayName,Id` .</span><span class="sxs-lookup"><span data-stu-id="c7659-121">For example, to only return the **displayName** and ID, add the following to your query: `$select=displayName,Id`.</span></span>

<span data-ttu-id="c7659-122">Так как запрос может вернуть много обращений, можно отфильтровать их с помощью **DisplayName**.</span><span class="sxs-lookup"><span data-stu-id="c7659-122">Because a request can return many cases, you can filter them by using **displayName**.</span></span>  <span data-ttu-id="c7659-123">Чтобы выполнить фильтрацию по **DisplayName**, добавьте в запрос следующее: `$filter=displayName eq 'rs1'` , где имя набора проверки — RS1.</span><span class="sxs-lookup"><span data-stu-id="c7659-123">To filter by **displayName**, add the following to your query: `$filter=displayName eq 'rs1'`, where the review set name is rs1.</span></span>

<span data-ttu-id="c7659-124">Дополнительные сведения о фильтрации и указании полей можно узнать [в статье Использование выражений фильтров в URI OData ](/dynamics-nav/using-filter-expressions-in-odata-uris).</span><span class="sxs-lookup"><span data-stu-id="c7659-124">For more information about filtering and specifying fields, see [Using Filter Expressions in OData URIs ](/dynamics-nav/using-filter-expressions-in-odata-uris).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7659-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7659-125">Request headers</span></span>

| <span data-ttu-id="c7659-126">Имя</span><span class="sxs-lookup"><span data-stu-id="c7659-126">Name</span></span>      |<span data-ttu-id="c7659-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c7659-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7659-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7659-128">Authorization</span></span> | <span data-ttu-id="c7659-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7659-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7659-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7659-131">Request body</span></span>

<span data-ttu-id="c7659-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7659-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7659-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7659-133">Response</span></span>

<span data-ttu-id="c7659-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Review](../resources/reviewset.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c7659-134">If successful, this method returns a `200 OK` response code and the requested [reviewSet](../resources/reviewset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7659-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7659-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7659-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7659-136">Request</span></span>

<span data-ttu-id="c7659-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7659-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7659-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7659-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets/0157910c-57ce-4e48-bd4b-90f3c88ca32e
```
# <a name="c"></a>[<span data-ttu-id="c7659-139">C#</span><span class="sxs-lookup"><span data-stu-id="c7659-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7659-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7659-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7659-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7659-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c7659-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7659-142">Response</span></span>

<span data-ttu-id="c7659-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7659-143">The following is an example of the response.</span></span>

> <span data-ttu-id="c7659-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7659-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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