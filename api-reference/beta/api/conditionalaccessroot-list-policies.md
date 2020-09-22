---
title: Список политик
description: Получение списка объектов Кондитионалакцессполици.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ca1ea67f64f0eba5905ae160d00f1673d4b0dab5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982448"
---
# <a name="list-policies"></a><span data-ttu-id="da485-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="da485-103">List policies</span></span>

<span data-ttu-id="da485-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da485-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da485-105">Получение списка объектов [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="da485-105">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="da485-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da485-106">Permissions</span></span>

<span data-ttu-id="da485-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da485-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da485-109">Permission type</span></span>                        | <span data-ttu-id="da485-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da485-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="da485-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da485-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da485-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="da485-112">Policy.Read.All</span></span> |
|<span data-ttu-id="da485-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da485-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da485-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da485-114">Not supported.</span></span> |
|<span data-ttu-id="da485-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da485-115">Application</span></span>                            | <span data-ttu-id="da485-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="da485-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da485-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da485-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da485-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da485-118">Optional query parameters</span></span>

<span data-ttu-id="da485-119">Этот метод поддерживает `$skip` параметры запросов,,,, `$top` `$count` `$filter` `$orderBy` и `$select` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="da485-119">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="da485-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="da485-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="da485-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da485-121">Request headers</span></span>

| <span data-ttu-id="da485-122">Имя</span><span class="sxs-lookup"><span data-stu-id="da485-122">Name</span></span>      |<span data-ttu-id="da485-123">Описание</span><span class="sxs-lookup"><span data-stu-id="da485-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da485-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="da485-124">Authorization</span></span> | <span data-ttu-id="da485-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="da485-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="da485-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="da485-126">Request body</span></span>

<span data-ttu-id="da485-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da485-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da485-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="da485-128">Response</span></span>

<span data-ttu-id="da485-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da485-129">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da485-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="da485-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da485-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="da485-131">Request</span></span>

<span data-ttu-id="da485-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da485-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da485-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="da485-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies?$filter=displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'
```
# <a name="c"></a>[<span data-ttu-id="da485-134">C#</span><span class="sxs-lookup"><span data-stu-id="da485-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da485-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da485-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da485-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da485-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da485-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="da485-137">Response</span></span>

<span data-ttu-id="da485-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da485-138">The following is an example of the response.</span></span>

> <span data-ttu-id="da485-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da485-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies",
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
                "deviceStates": null,
                "devices": null,
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
                "deviceStates": null,
                "devices": null,
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


