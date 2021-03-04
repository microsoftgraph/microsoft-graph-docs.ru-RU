---
title: Случаи списка
description: Извлечение списка случаев получения электронных данных.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 18cae9c7306c3e45207f381a7c208c77df0eb434
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447137"
---
# <a name="list-cases"></a><span data-ttu-id="f2d7b-103">Случаи списка</span><span class="sxs-lookup"><span data-stu-id="f2d7b-103">List cases</span></span>

<span data-ttu-id="f2d7b-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f2d7b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2d7b-105">Извлечение списка [объектов-кейсов.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="f2d7b-105">Retrieve a list of [case](../resources/ediscovery-case.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2d7b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2d7b-106">Permissions</span></span>

<span data-ttu-id="f2d7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2d7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2d7b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2d7b-109">Permission type</span></span>|<span data-ttu-id="f2d7b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2d7b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2d7b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2d7b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2d7b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d7b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f2d7b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2d7b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2d7b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-114">Not supported.</span></span>|
|<span data-ttu-id="f2d7b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2d7b-115">Application</span></span>|<span data-ttu-id="f2d7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2d7b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2d7b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2d7b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2d7b-118">Optional query parameters</span></span>

<span data-ttu-id="f2d7b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f2d7b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f2d7b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2d7b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2d7b-121">Request headers</span></span>

| <span data-ttu-id="f2d7b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f2d7b-122">Name</span></span>      |<span data-ttu-id="f2d7b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f2d7b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f2d7b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2d7b-124">Authorization</span></span> | <span data-ttu-id="f2d7b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2d7b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2d7b-127">Request body</span></span>

<span data-ttu-id="f2d7b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2d7b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2d7b-129">Response</span></span>

<span data-ttu-id="f2d7b-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2d7b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2d7b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2d7b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2d7b-132">Request</span></span>

<span data-ttu-id="f2d7b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2d7b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2d7b-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "list_case"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases
```

# <a name="c"></a>[<span data-ttu-id="f2d7b-135">C#</span><span class="sxs-lookup"><span data-stu-id="f2d7b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2d7b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2d7b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2d7b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2d7b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2d7b-138">Java</span><span class="sxs-lookup"><span data-stu-id="f2d7b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f2d7b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2d7b-139">Response</span></span>

<span data-ttu-id="f2d7b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="f2d7b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2d7b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "odata.nextLink":"https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skipToken=159dc1d7-f84f-439e-9d57-4a4d3af0abe5",
    "value": [
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
        },
        {
            "id": "b956a1b5-6b74-47db-af83-97d1fdad4ddc",
            "displayName": "My Case 2",
            "description": "",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-02-18T22:42:28.5505500Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-02-18T22:42:28.5505500Z",
            "status": "active",
            "closedBy": null,
            "closedDateTime": null,
            "externalId": ""
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List cases",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
