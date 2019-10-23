---
title: Получение Кондитионалакцессполици
description: Получение свойств и связей объекта Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1672dd7be866f9b53ff226c1751c418baa350304
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638409"
---
# <a name="get-conditionalaccesspolicy"></a><span data-ttu-id="c353c-103">Получение Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c353c-103">Get conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c353c-104">Получение свойств и связей объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c353c-104">Retrieve the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c353c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c353c-105">Permissions</span></span>

<span data-ttu-id="c353c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c353c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c353c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c353c-108">Permission type</span></span>                        | <span data-ttu-id="c353c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c353c-109">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="c353c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c353c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c353c-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c353c-111">Policy.Read.All</span></span> |
|<span data-ttu-id="c353c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c353c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c353c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c353c-113">Not supported.</span></span> |
|<span data-ttu-id="c353c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c353c-114">Application</span></span>                            | <span data-ttu-id="c353c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c353c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c353c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c353c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/policies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c353c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c353c-117">Optional query parameters</span></span>

<span data-ttu-id="c353c-118">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c353c-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="c353c-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c353c-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c353c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c353c-120">Request headers</span></span>

| <span data-ttu-id="c353c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c353c-121">Name</span></span>      |<span data-ttu-id="c353c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c353c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c353c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c353c-123">Authorization</span></span> | <span data-ttu-id="c353c-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c353c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c353c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c353c-125">Request body</span></span>

<span data-ttu-id="c353c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c353c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c353c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c353c-127">Response</span></span>

<span data-ttu-id="c353c-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c353c-128">If successful, this method returns a `200 OK` response code and the requested [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c353c-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c353c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c353c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c353c-130">Request</span></span>

<span data-ttu-id="c353c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c353c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicy"
}-->

```http
GET https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```

### <a name="response"></a><span data-ttu-id="c353c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c353c-132">Response</span></span>

<span data-ttu-id="c353c-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c353c-133">The following is an example of the response.</span></span>

> <span data-ttu-id="c353c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c353c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies/$entity",
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
            "modern",
            "easSupported",
            "easUnsupported",
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
        },
        "deviceStates": {
            "includeStates": [
                "All"
            ],
            "excludeStates": [
                "Compliant"
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
