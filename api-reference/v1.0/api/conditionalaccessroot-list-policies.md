---
title: Список политик
description: Получение списка объектов кондитионалакцессполици.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e77a783cd4c4ddaa630c4170a12deeb35ed59cc9
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567223"
---
# <a name="list-policies"></a><span data-ttu-id="ab197-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="ab197-103">List policies</span></span>

<span data-ttu-id="ab197-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab197-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab197-105">Получение списка объектов [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ab197-105">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab197-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab197-106">Permissions</span></span>

<span data-ttu-id="ab197-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab197-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab197-109">Permission type</span></span>                        | <span data-ttu-id="ab197-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab197-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab197-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab197-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab197-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab197-112">Policy.Read.All</span></span> |
| <span data-ttu-id="ab197-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab197-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab197-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab197-114">Not supported.</span></span> |
| <span data-ttu-id="ab197-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ab197-115">Application</span></span>                            | <span data-ttu-id="ab197-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab197-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab197-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab197-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab197-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab197-118">Optional query parameters</span></span>

<span data-ttu-id="ab197-119">Этот метод поддерживает `$skip` параметры запросов,,,, `$top` `$count` `$filter` `$orderBy` и `$select` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ab197-119">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ab197-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ab197-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab197-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab197-121">Request headers</span></span>

| <span data-ttu-id="ab197-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ab197-122">Name</span></span>      |<span data-ttu-id="ab197-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ab197-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab197-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab197-124">Authorization</span></span> | <span data-ttu-id="ab197-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ab197-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab197-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab197-126">Request body</span></span>

<span data-ttu-id="ab197-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab197-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab197-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab197-128">Response</span></span>

<span data-ttu-id="ab197-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab197-129">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab197-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ab197-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab197-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab197-131">Request</span></span>

<span data-ttu-id="ab197-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab197-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab197-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab197-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
```
# <a name="c"></a>[<span data-ttu-id="ab197-134">C#</span><span class="sxs-lookup"><span data-stu-id="ab197-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab197-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab197-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab197-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab197-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab197-137">Java</span><span class="sxs-lookup"><span data-stu-id="ab197-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="ab197-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab197-138">Response</span></span>

<span data-ttu-id="ab197-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ab197-139">The following is an example of the response.</span></span>

> <span data-ttu-id="ab197-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab197-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies",
    "value": [
        {
            "id": "ad8d2b4a-8d30-413f-88b8-144c6c8d98d9",
            "displayName": "SimplePolicy1",
            "createdDateTime": null,
            "modifiedDateTime": null,
            "state": "disabled",
            "sessionControls": null,
            "conditions": {
                "signInRiskLevels": [],
                "clientAppTypes": [
                    "all"
                ],
                "platforms": null,
                "locations": null,
                "applications": {
                    "includeApplications": [
                        "None"
                    ],
                    "excludeApplications": [],
                    "includeUserActions": []
                },
                "users": {
                    "includeUsers": [
                        "None"
                    ],
                    "excludeUsers": [],
                    "includeGroups": [],
                    "excludeGroups": [],
                    "includeRoles": [],
                    "excludeRoles": []
                }
            },
            "grantControls": {
                "operator": "OR",
                "builtInControls": [
                    "block"
                ],
                "customAuthenticationFactors": [],
                "termsOfUse": []
            }
        },
        {
            "id": "c558e346-969d-40a7-a64e-2df6c2c88490",
            "displayName": "SimplePolicy2",
            "createdDateTime": null,
            "modifiedDateTime": null,
            "state": "disabled",
            "sessionControls": null,
            "conditions": {
                "signInRiskLevels": [],
                "clientAppTypes": [
                    "all"
                ],
                "platforms": null,
                "locations": null,
                "applications": {
                    "includeApplications": [
                        "None"
                    ],
                    "excludeApplications": [],
                    "includeUserActions": []
                },
                "users": {
                    "includeUsers": [
                        "None"
                    ],
                    "excludeUsers": [],
                    "includeGroups": [],
                    "excludeGroups": [],
                    "includeRoles": [],
                    "excludeRoles": []
                }
            },
            "grantControls": {
                "operator": "OR",
                "builtInControls": [
                    "mfa"
                ],
                "customAuthenticationFactors": [],
                "termsOfUse": []
            }
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List policies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
