---
title: Тип ресурса policyRoot
description: Тип ресурса, который предоставляет свойства навигации для одноэлементных политик.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f91bdf76395b44c4041a64ce81716158455de3cf
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133498"
---
# <a name="policyroot-resource-type"></a>Тип ресурса policyRoot

Пространство имен: microsoft.graph

Тип ресурса, который предоставляет свойства навигации для одноэлементных политик. Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор политики. Наследуется от [сущности](../resources/entity.md).|


## <a name="relationships"></a>Связи
| Связь                              | Тип                                                                                                      | Описание                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityBasedTimeoutPolicies              | [Коллекция activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md)                                    | Политика, которая управляет временем ожидания простоя для веб-сеансов для приложений.                                                                                        |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | Политика, с помощью которой запросы на согласие создаются и управляются для всего клиента.                                                                                  |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | Конфигурация политики для самостоятельной регистрации внешних пользователей.                                                                                   |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | Методы проверки подлинности и пользователи, которым разрешено использовать их для входа и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD). |
| authorizationPolicy                       | [Коллекция authorizationPolicy](authorizationpolicy.md)                                                  | Политика, которая управляет Azure AD авторизации.                                                                                                            |
| claimsMappingPolicies                     | Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)                                                  | Политики сопоставления утверждений для протоколов WS-Fed, SAML, OAuth 2.0 и OpenID Подключение для маркеров, выданных конкретному приложению.                                   |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | Пользовательские правила, определяющие сценарий доступа.                                                                                                                     |
| featureRolloutPolicies                    | [Коллекция featureRolloutPolicy](featurerolloutpolicy.md)                                                | Политика развертывания компонентов, связанная с объектом каталога.                                                                                                       |
| homeRealmDiscoveryPolicies                | Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)                                        | Политика для управления Azure AD проверки подлинности для федеративных пользователей.                                                                                          |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | Политика, представляющая параметры безопасности по умолчанию, которые защищают от распространенных атак.                                                                                |
| permissionGrantPolicies                   | Коллекция [permissionGrantPolicy](permissiongrantpolicy.md)                                              | Политика, указывавая условия, при которых может быть предоставлено согласие.                                                                                         |
|roleManagementPolicies|[Коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)| Указывает различные политики, связанные с областями и ролями. |
|roleManagementPolicyAssignments|[Коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)| Назначение политики управления ролем объекту определения роли. |
| tokenIssuancePolicies                     | Коллекция [tokenIssuancePolicy](tokenissuancepolicy.md)                                                  | Политика, указывавая характеристики маркеров SAML, выданных Azure AD.                                                                                     |
| tokenLifetimePolicies                     | Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)                                                  | Политика, которая управляет временем существования маркера доступа JWT, маркера идентификатора или токена SAML 1.1/2.0, выданного Azure AD.                                                |


## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot",
  "id": "String (identifier)"
}
```

