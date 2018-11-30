---
title: Тип ресурса synchronizationSecretKeyStringValuePair
description: 'Представляет одно значение секрета. '
ms.openlocfilehash: 31aa5d983a0117591d3be75939b2c881a9782e7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082328"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="a5185-103">Тип ресурса synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="a5185-103">synchronizationSecretKeyStringValuePair resource type</span></span>

> <span data-ttu-id="a5185-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5185-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5185-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5185-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5185-106">Представляет одно значение секрета.</span><span class="sxs-lookup"><span data-stu-id="a5185-106">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="a5185-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5185-107">Properties</span></span>
| <span data-ttu-id="a5185-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5185-108">Property</span></span>     | <span data-ttu-id="a5185-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a5185-109">Type</span></span>   |<span data-ttu-id="a5185-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5185-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5185-111">key</span><span class="sxs-lookup"><span data-stu-id="a5185-111">key</span></span>|<span data-ttu-id="a5185-112">String</span><span class="sxs-lookup"><span data-stu-id="a5185-112">String</span></span>| <span data-ttu-id="a5185-113">Возможные значения: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken` , `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="a5185-113">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="a5185-114">value</span><span class="sxs-lookup"><span data-stu-id="a5185-114">value</span></span>|<span data-ttu-id="a5185-115">String</span><span class="sxs-lookup"><span data-stu-id="a5185-115">String</span></span>|<span data-ttu-id="a5185-116">Значение секрета.</span><span class="sxs-lookup"><span data-stu-id="a5185-116">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5185-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5185-117">JSON representation</span></span>

<span data-ttu-id="a5185-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5185-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->