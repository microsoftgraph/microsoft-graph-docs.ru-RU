---
title: Тип ресурса Синчронизатионсекреткэйстрингвалуепаир
description: Представляет одно секретное значение.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b2c5929b7ba00a12cf66cd3f013dbf31446aba19
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217586"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="8607f-103">Тип ресурса Синчронизатионсекреткэйстрингвалуепаир</span><span class="sxs-lookup"><span data-stu-id="8607f-103">synchronizationSecretKeyStringValuePair resource type</span></span>

<span data-ttu-id="8607f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8607f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8607f-105">Представляет одно секретное значение.</span><span class="sxs-lookup"><span data-stu-id="8607f-105">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="8607f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8607f-106">Properties</span></span>
| <span data-ttu-id="8607f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8607f-107">Property</span></span>     | <span data-ttu-id="8607f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8607f-108">Type</span></span>   |<span data-ttu-id="8607f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8607f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8607f-110">key</span><span class="sxs-lookup"><span data-stu-id="8607f-110">key</span></span>|<span data-ttu-id="8607f-111">Строка</span><span class="sxs-lookup"><span data-stu-id="8607f-111">String</span></span>| <span data-ttu-id="8607f-112">`None`Возможные значения:, `UserName`, `Password`, `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `Domain` `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `TestReferences`,,,,,, `Oauth2RefreshToken`,,,,, `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord`,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,. `SandboxName` `EnforceDomain` `SyncNotificationSettings` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled` `SyncAgentCompatibilityKey` `SyncAgentADContainer` `ValidateDomain` `Url` `ClientSecret` `SingleSignOnType` `Sandbox`</span><span class="sxs-lookup"><span data-stu-id="8607f-112">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="8607f-113">value</span><span class="sxs-lookup"><span data-stu-id="8607f-113">value</span></span>|<span data-ttu-id="8607f-114">String</span><span class="sxs-lookup"><span data-stu-id="8607f-114">String</span></span>|<span data-ttu-id="8607f-115">Значение секрета.</span><span class="sxs-lookup"><span data-stu-id="8607f-115">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8607f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8607f-116">JSON representation</span></span>

<span data-ttu-id="8607f-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8607f-117">The following is a JSON representation of the resource.</span></span>

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
