---
title: Создание Кондитионалакцессполици
description: Создание нового Кондитионалакцессполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 161e9824b9018d0504d48bbefa15412364c24960
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638437"
---
# <a name="create-conditionalaccesspolicy"></a><span data-ttu-id="0fa45-103">Создание Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="0fa45-103">Create conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fa45-104">Создание нового [кондитионалакцессполици](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fa45-104">Create a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa45-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa45-105">Permissions</span></span>

<span data-ttu-id="0fa45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fa45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fa45-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa45-108">Permission type</span></span>                        | <span data-ttu-id="0fa45-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fa45-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="0fa45-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fa45-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fa45-111">Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0fa45-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0fa45-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fa45-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa45-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fa45-113">Not supported.</span></span> |
|<span data-ttu-id="0fa45-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fa45-114">Application</span></span>                            | <span data-ttu-id="0fa45-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fa45-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="0fa45-116">Этот API требует нескольких разрешений.</span><span class="sxs-lookup"><span data-stu-id="0fa45-116">This API requires multiple permissions.</span></span> <span data-ttu-id="0fa45-117">Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="0fa45-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="0fa45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fa45-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /conditionalAccess/policies
```

## <a name="request-headers"></a><span data-ttu-id="0fa45-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fa45-119">Request headers</span></span>

| <span data-ttu-id="0fa45-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0fa45-120">Name</span></span>          | <span data-ttu-id="0fa45-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0fa45-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="0fa45-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fa45-122">Authorization</span></span> | <span data-ttu-id="0fa45-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fa45-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0fa45-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fa45-125">Content-Type</span></span>  | <span data-ttu-id="0fa45-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fa45-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fa45-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fa45-128">Request body</span></span>

<span data-ttu-id="0fa45-129">В тексте запроса добавьте представление объекта [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fa45-129">In the request body, supply a JSON representation of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

<span data-ttu-id="0fa45-130">Допустимая политика должна содержать по крайней [](../resources/conditionalaccessapplications.md) мере одно правило `'includeApplications': 'none'`приложения, например, одно правило [пользователя](../resources/conditionalaccessusers.md) `'includeUsers': 'none'`, например, и по крайней мере один элемент управления " [предоставление](../resources/conditionalaccessgrantcontrols.md)/[сеанса](../resources/conditionalaccesssessioncontrols.md) ".</span><span class="sxs-lookup"><span data-stu-id="0fa45-130">A valid policy should contain at least one [application](../resources/conditionalaccessapplications.md) rule - for example, `'includeApplications': 'none'`, one [user](../resources/conditionalaccessusers.md) rule - for example, `'includeUsers': 'none'`, and at least one [grant](../resources/conditionalaccessgrantcontrols.md)/[session](../resources/conditionalaccesssessioncontrols.md) control.</span></span>

## <a name="response"></a><span data-ttu-id="0fa45-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa45-131">Response</span></span>

<span data-ttu-id="0fa45-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [кондитионалакцессполици](../resources/conditionalaccesspolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fa45-132">If successful, this method returns a `201 Created` response code and a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fa45-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="0fa45-133">Examples</span></span>

### <a name="example-1-require-mfa-to-access-exchange-online-outside-of-trusted-locations"></a><span data-ttu-id="0fa45-134">Пример 1: запрос MFA для доступа к Exchange Online вне надежных расположений</span><span class="sxs-lookup"><span data-stu-id="0fa45-134">Example 1: Require MFA to access Exchange Online outside of trusted locations</span></span>

#### <a name="request"></a><span data-ttu-id="0fa45-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fa45-135">Request</span></span>
<span data-ttu-id="0fa45-136">В следующем примере показан общий запрос для использования многофакторной проверки подлинности для доступа к Exchange Online из браузера или современного клиента проверки подлинности вне надежных расположений для определенной группы.</span><span class="sxs-lookup"><span data-stu-id="0fa45-136">The following example shows a common request to require multi-factor authentication for access to Exchange Online from a browser or modern auth client outside of trusted locations for a particular group.</span></span>

><span data-ttu-id="0fa45-137">**Примечание:** Перед использованием этой операции необходимо настроить надежные расположения.</span><span class="sxs-lookup"><span data-stu-id="0fa45-137">**Note:** You must set up your trusted locations before using this operation.</span></span>

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

#### <a name="response"></a><span data-ttu-id="0fa45-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa45-138">Response</span></span>

<span data-ttu-id="0fa45-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0fa45-139">The following is an example of the response.</span></span>

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

### <a name="example-2-block-access-to-exchange-online-from-non-trusted-regions"></a><span data-ttu-id="0fa45-140">Пример 2: Блокировка доступа к Exchange Online из ненадежных регионов</span><span class="sxs-lookup"><span data-stu-id="0fa45-140">Example 2: Block access to Exchange Online from non-trusted regions</span></span>

#### <a name="request"></a><span data-ttu-id="0fa45-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fa45-141">Request</span></span>
<span data-ttu-id="0fa45-142">В приведенном ниже примере показан запрос на блокировку доступа к Exchange Online из недоверенных и неизвестных областей.</span><span class="sxs-lookup"><span data-stu-id="0fa45-142">The following example shows a request to block access to Exchange Online from non-trusted/unknown regions.</span></span>
<span data-ttu-id="0fa45-143">В этом примере предполагается, что именованное расположение с идентификатором ID = 198ad66e-87b3-4157-85a3-8a7b51794ee9 соответствует списку ненадежных и неизвестных областей.</span><span class="sxs-lookup"><span data-stu-id="0fa45-143">This example assumes that the named location with id = 198ad66e-87b3-4157-85a3-8a7b51794ee9 corresponds to a list of non-trusted/unknown regions.</span></span>

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

#### <a name="response"></a><span data-ttu-id="0fa45-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa45-144">Response</span></span>

<span data-ttu-id="0fa45-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0fa45-145">The following is an example of the response.</span></span>

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

### <a name="example-3-use-all-conditionscontrols"></a><span data-ttu-id="0fa45-146">Пример 3: использование всех условий и элементов управления</span><span class="sxs-lookup"><span data-stu-id="0fa45-146">Example 3: Use all conditions/controls</span></span>

#### <a name="request"></a><span data-ttu-id="0fa45-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fa45-147">Request</span></span>
<span data-ttu-id="0fa45-148">Ниже приведен пример запроса на использование всех условий и элементов управления.</span><span class="sxs-lookup"><span data-stu-id="0fa45-148">The following is an example of the request to use all the conditions/controls.</span></span>
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

#### <a name="response"></a><span data-ttu-id="0fa45-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa45-149">Response</span></span>

<span data-ttu-id="0fa45-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0fa45-150">The following is an example of the response.</span></span>

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
