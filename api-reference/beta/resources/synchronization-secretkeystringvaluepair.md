---
title: Тип ресурса Синчронизатионсекреткэйстрингвалуепаир
description: 'Представляет одно секретное значение. '
localization_priority: Normal
ms.openlocfilehash: 36ec5ababb6c972bad336b3cfa8da4d34ba66c55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342900"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a>Тип ресурса Синчронизатионсекреткэйстрингвалуепаир

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет одно секретное значение. 

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|key|String| Возможные значения: `None`, `UserName`, `Password`, `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` `Domain` `ConsumerKey`,,,,,,,,,,,,,,,,,,,,, `ClientSecret` `SingleSignOnType` `Sandbox` `Url` , `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.|
|value|String|Значение секрета.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
