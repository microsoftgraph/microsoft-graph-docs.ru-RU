---
title: синхронизацияSecretKeyStringValuePair типа ресурса
description: Представляет одно секретное значение.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: f954427ad24a9fea6570dbb38c3de177b3498e92
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401602"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="4fc96-103">синхронизацияSecretKeyStringValuePair типа ресурса</span><span class="sxs-lookup"><span data-stu-id="4fc96-103">synchronizationSecretKeyStringValuePair resource type</span></span>

<span data-ttu-id="4fc96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fc96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fc96-105">Представляет одно секретное значение.</span><span class="sxs-lookup"><span data-stu-id="4fc96-105">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="4fc96-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fc96-106">Properties</span></span>
| <span data-ttu-id="4fc96-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fc96-107">Property</span></span>     | <span data-ttu-id="4fc96-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4fc96-108">Type</span></span>   |<span data-ttu-id="4fc96-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4fc96-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fc96-110">key</span><span class="sxs-lookup"><span data-stu-id="4fc96-110">key</span></span>|<span data-ttu-id="4fc96-111">синхронизацияSecret</span><span class="sxs-lookup"><span data-stu-id="4fc96-111">synchronizationSecret</span></span>| <span data-ttu-id="4fc96-112">Возможные значения: , . `None` `UserName` `Password` `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord` `SandboxName` `EnforceDomain` `SyncNotificationSettings` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled` `SyncAgentCompatibilityKey` `SyncAgentADContainer` `ValidateDomain` `Oauth2TokenExchangeUri` `Oauth2AuthorizationUri` `AuthenticationType` `TestReferences` `ConnectionString`</span><span class="sxs-lookup"><span data-stu-id="4fc96-112">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `Oauth2TokenExchangeUri`, `Oauth2AuthorizationUri`, `AuthenticationType`, `TestReferences`, `ConnectionString`.</span></span>|
|<span data-ttu-id="4fc96-113">value</span><span class="sxs-lookup"><span data-stu-id="4fc96-113">value</span></span>|<span data-ttu-id="4fc96-114">String</span><span class="sxs-lookup"><span data-stu-id="4fc96-114">String</span></span>|<span data-ttu-id="4fc96-115">Значение секрета.</span><span class="sxs-lookup"><span data-stu-id="4fc96-115">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4fc96-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fc96-116">JSON representation</span></span>

<span data-ttu-id="4fc96-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fc96-117">The following is a JSON representation of the resource.</span></span>

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


