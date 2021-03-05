---
title: Get conditionalAccessPolicy
description: Извлечение свойств и связей объекта conditionalAccessPolicy.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 30432a8c70253f092366782f5d8ff537905894da
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442126"
---
# <a name="get-conditionalaccesspolicy"></a><span data-ttu-id="a439f-103">Get conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a439f-103">Get conditionalAccessPolicy</span></span>

<span data-ttu-id="a439f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a439f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a439f-105">Извлечение свойств и связей объекта [conditionalAccessPolicy.](../resources/conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a439f-105">Retrieve the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a439f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a439f-106">Permissions</span></span>

<span data-ttu-id="a439f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a439f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a439f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a439f-109">Permission type</span></span>                        | <span data-ttu-id="a439f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a439f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a439f-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a439f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a439f-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a439f-112">Policy.Read.All</span></span> |
| <span data-ttu-id="a439f-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a439f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a439f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a439f-114">Not supported.</span></span> |
| <span data-ttu-id="a439f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a439f-115">Application</span></span>                            | <span data-ttu-id="a439f-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a439f-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a439f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a439f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/policies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a439f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a439f-118">Optional query parameters</span></span>

<span data-ttu-id="a439f-119">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a439f-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="a439f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a439f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a439f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a439f-121">Request headers</span></span>

| <span data-ttu-id="a439f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a439f-122">Name</span></span>      |<span data-ttu-id="a439f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a439f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a439f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a439f-124">Authorization</span></span> | <span data-ttu-id="a439f-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a439f-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a439f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a439f-126">Request body</span></span>

<span data-ttu-id="a439f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a439f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a439f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a439f-128">Response</span></span>

<span data-ttu-id="a439f-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a439f-129">If successful, this method returns a `200 OK` response code and the requested [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a439f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a439f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a439f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a439f-131">Request</span></span>

<span data-ttu-id="a439f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a439f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a439f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a439f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="a439f-134">C#</span><span class="sxs-lookup"><span data-stu-id="a439f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a439f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a439f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a439f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a439f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a439f-137">Java</span><span class="sxs-lookup"><span data-stu-id="a439f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conditionalaccesspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="a439f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a439f-138">Response</span></span>

<span data-ttu-id="a439f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a439f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a439f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a439f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "6b5e999b-0ba8-4186-a106-e0296c1c4358",
    "displayName": "Demo app for documentation",
    "createdDateTime": "2019-09-26T23:12:16.0792706Z",
    "modifiedDateTime": "2019-09-27T00:12:12.5986473Z",
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "medium",
            "low"
        ],
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "exchangeActiveSync",
            "other"
        ],
        "applications": {
            "includeApplications": [
                "All"
            ],
            "excludeApplications": [
                "499b84ac-1321-427f-aa17-267ca6975798",
                "00000007-0000-0000-c000-000000000000",
                "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                "00000012-0000-0000-c000-000000000000",
                "797f4846-ba00-4fd7-ba43-dac1f8f63013",
                "05a65629-4c1b-48c1-a78b-804c4abdd4af",
                "7df0a125-d3be-4c96-aa54-591f83ff541c"
            ],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [
                "a702a13d-a437-4a07-8a7e-8c052de62dfd"
            ],
            "excludeUsers": [
                "124c5b6a-ffa5-483a-9b88-04c3fce5574a",
                "GuestsOrExternalUsers"
            ],
            "includeGroups": [],
            "excludeGroups": [],
            "includeRoles": [
                "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
                "cf1c38e5-3621-4004-a7cb-879624dced7c",
                "c4e39bd9-1100-46d3-8c65-fb160da0071f"
            ],
            "excludeRoles": [
                "b0f54661-2d74-4c50-afa3-1ec803f12efe"
            ]
        },
        "platforms": {
            "includePlatforms": [
                "all"
            ],
            "excludePlatforms": [
                "iOS",
                "windowsPhone"
            ]
        },
        "locations": {
            "includeLocations": [
                "AllTrusted"
            ],
            "excludeLocations": [
                "00000000-0000-0000-0000-000000000000",
                "d2136c9c-b049-47ae-b9cf-316e04ef7198"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa",
            "compliantDevice",
            "domainJoinedDevice",
            "approvedApplication",
            "compliantApplication"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": [
            "ce580154-086a-40fd-91df-8a60abac81a0",
            "7f29d675-caff-43e1-8a53-1b8516ed2075"
        ]
    },
    "sessionControls": {
        "applicationEnforcedRestrictions": null,
        "persistentBrowser": null,
        "cloudAppSecurity": {
            "cloudAppSecurityType": "blockDownloads",
            "isEnabled": true
        },
        "signInFrequency": {
            "value": 4,
            "type": "hours",
            "isEnabled": true
        }
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

