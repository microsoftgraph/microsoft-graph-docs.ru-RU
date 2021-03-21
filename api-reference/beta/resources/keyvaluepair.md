---
title: Тип ресурса keyValuePair
description: Пара ключевых значений для параметров действия.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8897ea3d3788ce3fa846d845cb0854101b0b2ce7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960427"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="d6e41-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="d6e41-103">keyValuePair resource type</span></span>

<span data-ttu-id="d6e41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6e41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6e41-105">Пара ключевых значений для параметров действия.</span><span class="sxs-lookup"><span data-stu-id="d6e41-105">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="d6e41-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6e41-106">Properties</span></span>

| <span data-ttu-id="d6e41-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6e41-107">Property</span></span>     | <span data-ttu-id="d6e41-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d6e41-108">Type</span></span>        | <span data-ttu-id="d6e41-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d6e41-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d6e41-110">name</span><span class="sxs-lookup"><span data-stu-id="d6e41-110">name</span></span>|<span data-ttu-id="d6e41-111">String</span><span class="sxs-lookup"><span data-stu-id="d6e41-111">String</span></span>|<span data-ttu-id="d6e41-112">Имя этой пары значений ключа.</span><span class="sxs-lookup"><span data-stu-id="d6e41-112">Name for this key-value pair.</span></span> <span data-ttu-id="d6e41-113">Возможные имена: `AdditionalWSFedEndpointCheckResult` , , , , , , ,  `AllowedAuthenticationClassReferencesCheckResult` , `AlwaysRequireAuthenticationCheckResult`   `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult`  `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult`  `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult`  `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult` .</span><span class="sxs-lookup"><span data-stu-id="d6e41-113">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span>|
|<span data-ttu-id="d6e41-114">value</span><span class="sxs-lookup"><span data-stu-id="d6e41-114">value</span></span>|<span data-ttu-id="d6e41-115">String</span><span class="sxs-lookup"><span data-stu-id="d6e41-115">String</span></span>|<span data-ttu-id="d6e41-116">Значение для этой пары ключ-значение.</span><span class="sxs-lookup"><span data-stu-id="d6e41-116">Value for this key-value pair.</span></span> <span data-ttu-id="d6e41-117">Возможные значения результатов : (когда проверка проверки прошла), (когда проверка проверки не прошла) или (когда проверка проверки является `0` `1` `2` предупреждением).</span><span class="sxs-lookup"><span data-stu-id="d6e41-117">Possible result values are `0` (when the validation check passed), `1` (when the validation check failed), or `2` (when the validation check is a warning).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6e41-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6e41-118">JSON representation</span></span>

<span data-ttu-id="d6e41-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6e41-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

