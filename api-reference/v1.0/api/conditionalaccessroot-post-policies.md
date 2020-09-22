---
title: Создание Кондитионалакцессполици
description: Создание нового Кондитионалакцессполици.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 654f6b23a92544a62290d81b76263d8b3c57b37c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094890"
---
# <a name="create-conditionalaccesspolicy"></a><span data-ttu-id="7bbd2-103">Создание Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="7bbd2-103">Create conditionalAccessPolicy</span></span>

<span data-ttu-id="7bbd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bbd2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bbd2-105">Создание нового [кондитионалакцессполици](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bbd2-105">Create a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7bbd2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bbd2-106">Permissions</span></span>

<span data-ttu-id="7bbd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bbd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7bbd2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bbd2-109">Permission type</span></span>                        | <span data-ttu-id="7bbd2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bbd2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7bbd2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bbd2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bbd2-112">Policy. Read. ALL, Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="7bbd2-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
| <span data-ttu-id="7bbd2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bbd2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bbd2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-114">Not supported.</span></span> |
| <span data-ttu-id="7bbd2-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7bbd2-115">Application</span></span>                            | <span data-ttu-id="7bbd2-116">Policy. Read. ALL, Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="7bbd2-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bbd2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bbd2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/policies
```

## <a name="request-headers"></a><span data-ttu-id="7bbd2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bbd2-118">Request headers</span></span>

| <span data-ttu-id="7bbd2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7bbd2-119">Name</span></span>          | <span data-ttu-id="7bbd2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7bbd2-120">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="7bbd2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bbd2-121">Authorization</span></span> | <span data-ttu-id="7bbd2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7bbd2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bbd2-124">Content-Type</span></span>  | <span data-ttu-id="7bbd2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bbd2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bbd2-127">Request body</span></span>

<span data-ttu-id="7bbd2-128">В тексте запроса добавьте представление объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-128">In the request body, supply a JSON representation of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

<span data-ttu-id="7bbd2-129">Допустимая политика должна содержать по крайней мере один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="7bbd2-129">A valid policy should contain at least one of the following:</span></span>

* <span data-ttu-id="7bbd2-130">правило [приложения](../resources/conditionalaccessapplications.md) .</span><span class="sxs-lookup"><span data-stu-id="7bbd2-130">[application](../resources/conditionalaccessapplications.md) rule.</span></span> <span data-ttu-id="7bbd2-131">Например, `'includeApplications': 'none'`.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-131">For example, `'includeApplications': 'none'`.</span></span>
* <span data-ttu-id="7bbd2-132">правило [пользователя](../resources/conditionalaccessusers.md) .</span><span class="sxs-lookup"><span data-stu-id="7bbd2-132">[user](../resources/conditionalaccessusers.md) rule.</span></span> <span data-ttu-id="7bbd2-133">Например, `'includeUsers': 'none'`.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-133">For example, `'includeUsers': 'none'`.</span></span>
* <span data-ttu-id="7bbd2-134">[Grant (предоставление](../resources/conditionalaccessgrantcontrols.md) / ) Управление [сеансом](../resources/conditionalaccesssessioncontrols.md) .</span><span class="sxs-lookup"><span data-stu-id="7bbd2-134">[grant](../resources/conditionalaccessgrantcontrols.md)/[session](../resources/conditionalaccesssessioncontrols.md) control.</span></span>

## <a name="response"></a><span data-ttu-id="7bbd2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bbd2-135">Response</span></span>

<span data-ttu-id="7bbd2-136">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-136">If successful, this method returns a `201 Created` response code and a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bbd2-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="7bbd2-137">Examples</span></span>

### <a name="example-1-require-mfa-to-access-exchange-online-outside-of-trusted-locations"></a><span data-ttu-id="7bbd2-138">Пример 1: запрос MFA для доступа к Exchange Online вне надежных расположений</span><span class="sxs-lookup"><span data-stu-id="7bbd2-138">Example 1: Require MFA to access Exchange Online outside of trusted locations</span></span>

#### <a name="request"></a><span data-ttu-id="7bbd2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bbd2-139">Request</span></span>
<span data-ttu-id="7bbd2-140">В следующем примере показан общий запрос на проверку подлинности многофакторной проверки подлинности для доступа к Exchange Online из современных клиентов проверки подлинности вне надежных расположений для определенной группы.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-140">The following example shows a common request to require multi-factor authentication for access to Exchange Online from modern authentication clients outside of trusted locations for a particular group.</span></span>

><span data-ttu-id="7bbd2-141">**Примечание:** Перед использованием этой операции необходимо настроить надежные расположения.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-141">**Note:** You must set up your trusted locations before using this operation.</span></span>

# <a name="http"></a>[<span data-ttu-id="7bbd2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bbd2-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Access to EXO requires MFA",
    "state": "enabled",
    "conditions": {
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "browser"
        ],
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        },
        "locations": {
            "includeLocations": [
                "All"
            ],
            "excludeLocations": [
                "AllTrusted"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="7bbd2-143">C#</span><span class="sxs-lookup"><span data-stu-id="7bbd2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bbd2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bbd2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bbd2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bbd2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7bbd2-146">Java</span><span class="sxs-lookup"><span data-stu-id="7bbd2-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="7bbd2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bbd2-147">Response</span></span>

<span data-ttu-id="7bbd2-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "7359d0e0-d8a9-4afa-8a93-e23e099d7be8",
    "displayName": "Access to EXO requires MFA",
    "createdDateTime": "2019-10-14T19:52:00.050958Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "signInRiskLevels": [],
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "browser"
        ],
        "platforms": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
            "excludeGroups": [],
            "includeRoles": [],
            "excludeRoles": []
        },
        "locations": {
            "includeLocations": [
                "All"
            ],
            "excludeLocations": [
                "AllTrusted"
            ]
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
```

### <a name="example-2-block-access-to-exchange-online-from-non-trusted-regions"></a><span data-ttu-id="7bbd2-149">Пример 2: Блокировка доступа к Exchange Online из ненадежных регионов</span><span class="sxs-lookup"><span data-stu-id="7bbd2-149">Example 2: Block access to Exchange Online from non-trusted regions</span></span>

#### <a name="request"></a><span data-ttu-id="7bbd2-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bbd2-150">Request</span></span>
<span data-ttu-id="7bbd2-151">В приведенном ниже примере показан запрос на блокировку доступа к Exchange Online из недоверенных и неизвестных областей.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-151">The following example shows a request to block access to Exchange Online from non-trusted/unknown regions.</span></span>
<span data-ttu-id="7bbd2-152">В этом примере предполагается, что именованное расположение с идентификатором ID = 198ad66e-87b3-4157-85a3-8a7b51794ee9 соответствует списку ненадежных и неизвестных областей.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-152">This example assumes that the named location with id = 198ad66e-87b3-4157-85a3-8a7b51794ee9 corresponds to a list of non-trusted/unknown regions.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Block access to EXO non-trusted regions.",
    "state": "enabled",
    "conditions": {
        "clientAppTypes": [
            "all"
        ],
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        },
        "locations": {
            "includeLocations": [
                "198ad66e-87b3-4157-85a3-8a7b51794ee9"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "block"
        ]
    }
}
```

#### <a name="response"></a><span data-ttu-id="7bbd2-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bbd2-153">Response</span></span>

<span data-ttu-id="7bbd2-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "c98e6c3d-f6ca-42ea-a927-773b6f12a0c2",
    "displayName": "Block access to EXO non-trusted regions.",
    "createdDateTime": "2019-10-14T19:53:11.3705634Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "signInRiskLevels": [],
        "clientAppTypes": [
            "all"
        ],
        "platforms": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
            "excludeGroups": [],
            "includeRoles": [],
            "excludeRoles": []
        },
        "locations": {
            "includeLocations": [
                "198ad66e-87b3-4157-85a3-8a7b51794ee9"
            ],
            "excludeLocations": []
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
}
```

### <a name="example-3-use-all-conditions-and-controls"></a><span data-ttu-id="7bbd2-155">Пример 3: использование всех условий и элементов управления</span><span class="sxs-lookup"><span data-stu-id="7bbd2-155">Example 3: Use all conditions and controls</span></span>

#### <a name="request"></a><span data-ttu-id="7bbd2-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bbd2-156">Request</span></span>
<span data-ttu-id="7bbd2-157">Ниже приведен пример запроса на использование всех условий и элементов управления.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-157">The following is an example of the request to use all the conditions and controls.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Demo app for documentation",
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium"
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

#### <a name="response"></a><span data-ttu-id="7bbd2-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bbd2-158">Response</span></span>

<span data-ttu-id="7bbd2-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "6b5e999b-0ba8-4186-a106-e0296c1c4358",
    "displayName": "Demo app for documentation",
    "createdDateTime": "2019-09-26T23:12:16.0792706Z",
    "modifiedDateTime": null,
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium"
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

### <a name="example-4-require-mfa-to-exchange-online-from-non-compliant-devices"></a><span data-ttu-id="7bbd2-160">Пример 4: запрос MFA для Exchange Online с устройств, не соответствующих требованиям</span><span class="sxs-lookup"><span data-stu-id="7bbd2-160">Example 4: Require MFA to Exchange Online from non-compliant devices</span></span>

#### <a name="request"></a><span data-ttu-id="7bbd2-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bbd2-161">Request</span></span>
<span data-ttu-id="7bbd2-162">В приведенном ниже примере показано, как запросить MFA для Exchange Online с помощью устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-162">The following example shows a request to require MFA to Exchange Online from non-compliant devices.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Require MFA to EXO from non-compliant devices.",
    "state": "enabled",
    "conditions": {
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ]
    }
}
```

#### <a name="response"></a><span data-ttu-id="7bbd2-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bbd2-163">Response</span></span>

<span data-ttu-id="7bbd2-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7bbd2-164">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
     "id": "b3f1298e-8e93-49af-bdbf-94cf7d453ca3",
    "displayName": "Require MFA to EXO from non-compliant devices.",
    "createdDateTime": "2020-04-01T00:55:12.9571747Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "userRiskLevels": [],
        "signInRiskLevels": [],
        "clientAppTypes": [
            "all"
        ],
        "platforms": null,
        "locations": null,
        "times": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": [],
            "includeProtectionLevels": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

