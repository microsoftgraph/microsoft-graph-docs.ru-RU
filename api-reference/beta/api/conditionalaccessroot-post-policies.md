---
title: Создание Кондитионалакцессполици
description: Создание нового Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e49181cffed3b8217822ab7e80ebcae0508a885b
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926731"
---
# <a name="create-conditionalaccesspolicy"></a><span data-ttu-id="d4065-103">Создание Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="d4065-103">Create conditionalAccessPolicy</span></span>

<span data-ttu-id="d4065-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4065-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4065-105">Создание нового [кондитионалакцессполици](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4065-105">Create a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4065-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4065-106">Permissions</span></span>

<span data-ttu-id="d4065-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4065-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4065-109">Permission type</span></span>                        | <span data-ttu-id="d4065-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4065-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="d4065-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4065-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4065-112">Policy. Read. ALL, Policy. ReadWrite. Кондитионалакцесс и Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d4065-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="d4065-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4065-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4065-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4065-114">Not supported.</span></span> |
|<span data-ttu-id="d4065-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4065-115">Application</span></span>                            | <span data-ttu-id="d4065-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4065-116">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="d4065-117">У этого API есть [известная проблема](/graph/known-issues#permissions) , связанная с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="d4065-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="d4065-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4065-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /conditionalAccess/policies
```

## <a name="request-headers"></a><span data-ttu-id="d4065-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4065-119">Request headers</span></span>

| <span data-ttu-id="d4065-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d4065-120">Name</span></span>          | <span data-ttu-id="d4065-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d4065-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="d4065-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4065-122">Authorization</span></span> | <span data-ttu-id="d4065-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4065-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d4065-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4065-125">Content-Type</span></span>  | <span data-ttu-id="d4065-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4065-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4065-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4065-128">Request body</span></span>

<span data-ttu-id="d4065-129">В тексте запроса добавьте представление объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4065-129">In the request body, supply a JSON representation of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

<span data-ttu-id="d4065-130">Допустимая политика должна содержать по крайней [application](../resources/conditionalaccessapplications.md) мере одно правило `'includeApplications': 'none'`приложения, например, одно правило [пользователя](../resources/conditionalaccessusers.md) `'includeUsers': 'none'`, например, и по крайней мере один элемент управления " [предоставление](../resources/conditionalaccessgrantcontrols.md)/[сеанса](../resources/conditionalaccesssessioncontrols.md) ".</span><span class="sxs-lookup"><span data-stu-id="d4065-130">A valid policy should contain at least one [application](../resources/conditionalaccessapplications.md) rule - for example, `'includeApplications': 'none'`, one [user](../resources/conditionalaccessusers.md) rule - for example, `'includeUsers': 'none'`, and at least one [grant](../resources/conditionalaccessgrantcontrols.md)/[session](../resources/conditionalaccesssessioncontrols.md) control.</span></span>

## <a name="response"></a><span data-ttu-id="d4065-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4065-131">Response</span></span>

<span data-ttu-id="d4065-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4065-132">If successful, this method returns a `201 Created` response code and a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4065-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4065-133">Examples</span></span>

### <a name="example-1-require-mfa-to-access-exchange-online-outside-of-trusted-locations"></a><span data-ttu-id="d4065-134">Пример 1: запрос MFA для доступа к Exchange Online вне надежных расположений</span><span class="sxs-lookup"><span data-stu-id="d4065-134">Example 1: Require MFA to access Exchange Online outside of trusted locations</span></span>

#### <a name="request"></a><span data-ttu-id="d4065-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4065-135">Request</span></span>
<span data-ttu-id="d4065-136">В следующем примере показан общий запрос для использования многофакторной проверки подлинности для доступа к Exchange Online из браузера или современного клиента проверки подлинности вне надежных расположений для определенной группы.</span><span class="sxs-lookup"><span data-stu-id="d4065-136">The following example shows a common request to require multi-factor authentication for access to Exchange Online from a browser or modern auth client outside of trusted locations for a particular group.</span></span>

><span data-ttu-id="d4065-137">**Примечание:** Перед использованием этой операции необходимо настроить надежные расположения.</span><span class="sxs-lookup"><span data-stu-id="d4065-137">**Note:** You must set up your trusted locations before using this operation.</span></span>


# <a name="http"></a>[<span data-ttu-id="d4065-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4065-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Access to EXO requires MFA",
    "state": "enabled",
    "conditions": {
        "clientAppTypes": [
            "modern",
            "browser"
        ],
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"],
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
# <a name="c"></a>[<span data-ttu-id="d4065-139">C#</span><span class="sxs-lookup"><span data-stu-id="d4065-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4065-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4065-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4065-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4065-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d4065-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4065-142">Response</span></span>

<span data-ttu-id="d4065-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4065-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies/$entity",
    "id": "7359d0e0-d8a9-4afa-8a93-e23e099d7be8",
    "displayName": "Access to EXO requires MFA",
    "createdDateTime": "2019-10-14T19:52:00.050958Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "signInRiskLevels": [],
        "clientAppTypes": [
            "modern",
            "browser"
        ],
        "platforms": null,
        "deviceStates": null,
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

### <a name="example-2-block-access-to-exchange-online-from-non-trusted-regions"></a><span data-ttu-id="d4065-144">Пример 2: Блокировка доступа к Exchange Online из ненадежных регионов</span><span class="sxs-lookup"><span data-stu-id="d4065-144">Example 2: Block access to Exchange Online from non-trusted regions</span></span>

#### <a name="request"></a><span data-ttu-id="d4065-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4065-145">Request</span></span>
<span data-ttu-id="d4065-146">В приведенном ниже примере показан запрос на блокировку доступа к Exchange Online из недоверенных и неизвестных областей.</span><span class="sxs-lookup"><span data-stu-id="d4065-146">The following example shows a request to block access to Exchange Online from non-trusted/unknown regions.</span></span>
<span data-ttu-id="d4065-147">В этом примере предполагается, что именованное расположение с идентификатором ID = 198ad66e-87b3-4157-85a3-8a7b51794ee9 соответствует списку ненадежных и неизвестных областей.</span><span class="sxs-lookup"><span data-stu-id="d4065-147">This example assumes that the named location with id = 198ad66e-87b3-4157-85a3-8a7b51794ee9 corresponds to a list of non-trusted/unknown regions.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Block access to EXO non-trusted regions.",
    "state": "enabled",
    "conditions": {
        "clientAppTypes": [
            "modern",
            "browser",
            "easSupported",
            "easUnsupported",
            "other"
        ],
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"],
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

#### <a name="response"></a><span data-ttu-id="d4065-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4065-148">Response</span></span>

<span data-ttu-id="d4065-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4065-149">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://canary.graph.microsoft.com/testprodbetaconditionalAccessBetaDocs/$metadata#conditionalAccess/policies/$entity",
    "id": "c98e6c3d-f6ca-42ea-a927-773b6f12a0c2",
    "displayName": "Block access to EXO non-trusted regions.",
    "createdDateTime": "2019-10-14T19:53:11.3705634Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "signInRiskLevels": [],
        "clientAppTypes": [
            "modern",
            "browser",
            "easSupported",
            "easUnsupported",
            "other"
        ],
        "platforms": null,
        "deviceStates": null,
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

### <a name="example-3-use-all-conditionscontrols"></a><span data-ttu-id="d4065-150">Пример 3: использование всех условий и элементов управления</span><span class="sxs-lookup"><span data-stu-id="d4065-150">Example 3: Use all conditions/controls</span></span>

#### <a name="request"></a><span data-ttu-id="d4065-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4065-151">Request</span></span>
<span data-ttu-id="d4065-152">Ниже приведен пример запроса на использование всех условий и элементов управления.</span><span class="sxs-lookup"><span data-stu-id="d4065-152">The following is an example of the request to use all the conditions/controls.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/conditionalAccess/policies
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

#### <a name="response"></a><span data-ttu-id="d4065-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4065-153">Response</span></span>

<span data-ttu-id="d4065-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d4065-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies/$entity",
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
  "description": "Create conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
