---
title: тип ресурса authenticationRequirementPolicy
description: Azure AD может потребовать от пользователей пройти проверку MFA перед доступом к ресурсам. Если требуется проверка MFA, этот ресурс определяет политику, требуемую для MFA.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 287a946321e72bb2ff5002c0ed21ad0d1267b313
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647230"
---
# <a name="authenticationrequirementpolicy-resource-type"></a>тип ресурса authenticationRequirementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD может потребовать от пользователей пройти проверку MFA перед доступом к ресурсам. Если требуется проверка MFA, этот ресурс определяет политику, требуемую для MFA. 


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подробные|String|Предоставляет дополнительные данные о функции, которая определена в requirementProvider.|
|requirementProvider|requirementProvider|Определяет, какие функции Azure AD требуют MFA в этой политике. Возможные значения: `user`, `request`, `servicePrincipal`, `v1ConditionalAccess`, `multiConditionalAccess`, `tenantSessionRiskPolicy`, `accountCompromisePolicies`, `v1ConditionalAccessDependency`, `v1ConditionalAccessPolicyIdRequested`, `mfaRegistrationRequiredByIdentityProtectionPolicy`, `baselineProtection`, `mfaRegistrationRequiredByBaselineProtection`, `mfaRegistrationRequiredByMultiConditionalAccess`, `enforcedForCspAdmins`, `securityDefaults`, `mfaRegistrationRequiredBySecurityDefaults`, `proofUpCodeRequest`, `crossTenantOutboundRule`, `gpsLocationCondition`, `riskBasedPolicy`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationRequirementPolicy",
  "requirementProvider": "String",
  "detail": "String"
}
```
