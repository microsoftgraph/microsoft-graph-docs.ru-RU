---
title: Список политик
description: Получение списка объектов Кондитионалакцессполици.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7fc97177ee453a4968aafc52514c5fb58dafb2fe
ms.sourcegitcommit: 5d4bf35774eba6de21f4252b46f7e9d8f64a517f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/08/2020
ms.locfileid: "44168529"
---
# <a name="list-policies"></a><span data-ttu-id="fdbba-103">Список политик</span><span class="sxs-lookup"><span data-stu-id="fdbba-103">List policies</span></span>

<span data-ttu-id="fdbba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdbba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdbba-105">Получение списка объектов [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="fdbba-105">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdbba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fdbba-106">Permissions</span></span>

<span data-ttu-id="fdbba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdbba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdbba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdbba-109">Permission type</span></span>                        | <span data-ttu-id="fdbba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdbba-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="fdbba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdbba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fdbba-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdbba-112">Policy.Read.All</span></span> |
|<span data-ttu-id="fdbba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdbba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdbba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdbba-114">Not supported.</span></span> |
|<span data-ttu-id="fdbba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdbba-115">Application</span></span>                            | <span data-ttu-id="fdbba-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdbba-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdbba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdbba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdbba-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fdbba-118">Optional query parameters</span></span>

<span data-ttu-id="fdbba-119">Этот метод поддерживает параметры `$skip`запросов `$top`, `$count` `$filter` `$orderBy`,,, и `$select` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fdbba-119">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="fdbba-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fdbba-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdbba-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdbba-121">Request headers</span></span>

| <span data-ttu-id="fdbba-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fdbba-122">Name</span></span>      |<span data-ttu-id="fdbba-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fdbba-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fdbba-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdbba-124">Authorization</span></span> | <span data-ttu-id="fdbba-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="fdbba-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdbba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdbba-126">Request body</span></span>

<span data-ttu-id="fdbba-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fdbba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdbba-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdbba-128">Response</span></span>

<span data-ttu-id="fdbba-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fdbba-129">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fdbba-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="fdbba-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fdbba-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdbba-131">Request</span></span>

<span data-ttu-id="fdbba-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdbba-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fdbba-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdbba-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies?$filter=displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'
```
# <a name="c"></a>[<span data-ttu-id="fdbba-134">C#</span><span class="sxs-lookup"><span data-stu-id="fdbba-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdbba-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdbba-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdbba-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdbba-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fdbba-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdbba-137">Response</span></span>

<span data-ttu-id="fdbba-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fdbba-138">The following is an example of the response.</span></span>

> <span data-ttu-id="fdbba-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdbba-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
