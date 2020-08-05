---
title: Список Едисковерикасес
description: Получение списка дел eDiscovery.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9801598762603740fa321d5606d1e8a36aba958a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566993"
---
# <a name="list-ediscoverycases"></a><span data-ttu-id="336a9-103">Список Едисковерикасес</span><span class="sxs-lookup"><span data-stu-id="336a9-103">List ediscoveryCases</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="336a9-104">Получение списка объектов [едисковерикасе](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="336a9-104">Retrieve a list of [ediscoveryCase](../resources/ediscoverycase.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="336a9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="336a9-105">Permissions</span></span>

<span data-ttu-id="336a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="336a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="336a9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="336a9-108">Permission type</span></span>                        | <span data-ttu-id="336a9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="336a9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="336a9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="336a9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="336a9-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="336a9-111">User.Read</span></span> |
| <span data-ttu-id="336a9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="336a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="336a9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="336a9-113">Not supported.</span></span> |
| <span data-ttu-id="336a9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="336a9-114">Application</span></span>                            | <span data-ttu-id="336a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="336a9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="336a9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="336a9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases
```

## <a name="optional-query-parameters"></a><span data-ttu-id="336a9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="336a9-117">Optional query parameters</span></span>

<span data-ttu-id="336a9-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="336a9-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="336a9-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="336a9-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="336a9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="336a9-120">Request headers</span></span>

| <span data-ttu-id="336a9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="336a9-121">Name</span></span>      |<span data-ttu-id="336a9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="336a9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="336a9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="336a9-123">Authorization</span></span> | <span data-ttu-id="336a9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="336a9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="336a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="336a9-126">Request body</span></span>

<span data-ttu-id="336a9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="336a9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="336a9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="336a9-128">Response</span></span>

<span data-ttu-id="336a9-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едисковерикасе](../resources/ediscoverycase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="336a9-129">If successful, this method returns a `200 OK` response code and a collection of [ediscoveryCase](../resources/ediscoverycase.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="336a9-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="336a9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="336a9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="336a9-131">Request</span></span>

<span data-ttu-id="336a9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="336a9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="336a9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="336a9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_ediscoverycase"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases
```
# <a name="c"></a>[<span data-ttu-id="336a9-134">C#</span><span class="sxs-lookup"><span data-stu-id="336a9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="336a9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="336a9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="336a9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="336a9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="336a9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="336a9-137">Response</span></span>

<span data-ttu-id="336a9-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="336a9-138">The following is an example of the response.</span></span>

> <span data-ttu-id="336a9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="336a9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase",
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
