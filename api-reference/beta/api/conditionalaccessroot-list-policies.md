---
title: Список политик
description: Получение списка объектов Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c79ab7fe3993a2007b367db9992ae4fbf3b7ee0d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936668"
---
# <a name="list-policies"></a><span data-ttu-id="810ce-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="810ce-103">List policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="810ce-104">Получение списка объектов [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="810ce-104">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="810ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="810ce-105">Permissions</span></span>

<span data-ttu-id="810ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="810ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="810ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="810ce-108">Permission type</span></span>                        | <span data-ttu-id="810ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="810ce-109">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="810ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="810ce-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="810ce-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="810ce-111">Policy.Read.All</span></span> |
|<span data-ttu-id="810ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="810ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="810ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="810ce-113">Not supported.</span></span> |
|<span data-ttu-id="810ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="810ce-114">Application</span></span>                            | <span data-ttu-id="810ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="810ce-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="810ce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="810ce-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="810ce-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="810ce-117">Optional query parameters</span></span>

<span data-ttu-id="810ce-118">Этот метод поддерживает параметры `$skip`запросов `$top`, `$count` `$filter` `$orderBy`,,, и `$select` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="810ce-118">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="810ce-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="810ce-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="810ce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="810ce-120">Request headers</span></span>

| <span data-ttu-id="810ce-121">Имя</span><span class="sxs-lookup"><span data-stu-id="810ce-121">Name</span></span>      |<span data-ttu-id="810ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="810ce-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="810ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="810ce-123">Authorization</span></span> | <span data-ttu-id="810ce-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="810ce-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="810ce-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="810ce-125">Request body</span></span>

<span data-ttu-id="810ce-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="810ce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="810ce-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="810ce-127">Response</span></span>

<span data-ttu-id="810ce-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="810ce-128">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="810ce-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="810ce-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="810ce-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="810ce-130">Request</span></span>

<span data-ttu-id="810ce-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="810ce-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="810ce-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="810ce-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/policies?$filter=displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="810ce-133">C#</span><span class="sxs-lookup"><span data-stu-id="810ce-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="810ce-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="810ce-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="810ce-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="810ce-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="810ce-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="810ce-136">Response</span></span>

<span data-ttu-id="810ce-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="810ce-137">The following is an example of the response.</span></span>

> <span data-ttu-id="810ce-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="810ce-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
                "clientAppTypes": [],
                "platforms": null,
                "locations": null,
                "deviceStates": null,
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
                "clientAppTypes": [],
                "platforms": null,
                "locations": null,
                "deviceStates": null,
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
