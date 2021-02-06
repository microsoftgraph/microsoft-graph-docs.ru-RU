---
title: Тип ресурса synchronizationSecretKeyStringValuePair
description: Представляет одно значение секрета.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: da408988c61ffa8d608fe7f36b5925107731d714
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129375"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="db457-103">Тип ресурса synchronizationSecretKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="db457-103">synchronizationSecretKeyStringValuePair resource type</span></span>

<span data-ttu-id="db457-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db457-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db457-105">Представляет одно значение секрета.</span><span class="sxs-lookup"><span data-stu-id="db457-105">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="db457-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="db457-106">Properties</span></span>
| <span data-ttu-id="db457-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="db457-107">Property</span></span>     | <span data-ttu-id="db457-108">Тип</span><span class="sxs-lookup"><span data-stu-id="db457-108">Type</span></span>   |<span data-ttu-id="db457-109">Описание</span><span class="sxs-lookup"><span data-stu-id="db457-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db457-110">key</span><span class="sxs-lookup"><span data-stu-id="db457-110">key</span></span>|<span data-ttu-id="db457-111">Строка</span><span class="sxs-lookup"><span data-stu-id="db457-111">String</span></span>| <span data-ttu-id="db457-112">Возможные значения: `None` , `UserName` , `Password` , `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord` `SandboxName` `EnforceDomain` `SyncNotificationSettings` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled` `SyncAgentCompatibilityKey` `SyncAgentADContainer` `ValidateDomain` `TestReferences` .</span><span class="sxs-lookup"><span data-stu-id="db457-112">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="db457-113">value</span><span class="sxs-lookup"><span data-stu-id="db457-113">value</span></span>|<span data-ttu-id="db457-114">String</span><span class="sxs-lookup"><span data-stu-id="db457-114">String</span></span>|<span data-ttu-id="db457-115">Значение секрета.</span><span class="sxs-lookup"><span data-stu-id="db457-115">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db457-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="db457-116">JSON representation</span></span>

<span data-ttu-id="db457-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db457-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


