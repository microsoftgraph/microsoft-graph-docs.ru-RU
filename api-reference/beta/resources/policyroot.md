---
title: тип ресурсов policyRoot
description: Тип ресурса, подвергая свойства навигации для однотонных политик.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6f0a5b9862a955b9508fb9a9075a848646dbcac8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688439"
---
# <a name="policyroot-resource-type"></a>тип ресурсов policyRoot

Пространство имен: microsoft.graph

Тип ресурса, подвергая свойства навигации для однотонных политик.

## <a name="methods"></a>Methods
Нет

## <a name="properties"></a>Свойства
Нет


## <a name="relationships"></a>Связи
| Связь                              | Тип                                                                                                      | Описание                                                                                                                                                             |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| accessReviewPolicy                        | [accessReviewPolicy](accessreviewpolicy.md)                                                               | Политика, которая содержит параметры обзора доступа на уровне каталогов.                                                                                                        |
| activityBasedTimeoutPolicies              | [коллекция activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md)                                    | Политика, контролируемая простоем для веб-сеансов для приложений.                                                                                           |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | Политика, в которой создаются и управляются запросы на согласие для всего клиента.                                                                                     |
| appManagementPolicies                     | Коллекция [appManagementPolicy](appmanagementpolicy.md)                                                  | Политики, применяющие ограничения управления приложениями для определенных приложений и директоров служб, переопределяющие значение defaultAppManagementPolicy.                      |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | Конфигурация политики для самостоятельной регистрации внешних пользователей.                                                                                      |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | Методы проверки подлинности и пользователи, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD).    |
| authorizationPolicy                       | [коллекция authorizationPolicy](authorizationpolicy.md)                                                  | Политика, контролируемая настройками авторизации Azure AD.                                                                                                               |
| b2cAuthenticationMethodsPolicy            | [b2cAuthenticationMethodsPolicy](b2cauthenticationmethodspolicy.md)                                       | Политики Azure AD B2C, которые определяют, как конечные пользователи регистрируются через локальные учетные записи.                                                                                        |
| claimsMappingPolicies                     | Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)                                                  | Политики сопоставления утверждений для протоколов WS-Fed, SAML, OAuth 2.0 и OpenID Подключение для маркеров, выдаваемого конкретному приложению.                                      |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | Пользовательские правила, определяемые сценарием доступа.                                                                                                                        |
| defaultAppManagementPolicy                | [tenantAppManagementPolicy](tenantappmanagementpolicy.md)                                                 | Политика для всех клиентов, которая применяет ограничения управления приложениями для всех приложений и директоров служб.                                                           |
| deviceRegistrationPolicy                  | [deviceRegistrationPolicy](deviceregistrationpolicy.md)                                                   | Представляет область политики, контролируемую ограничениями квот, дополнительной проверкой подлинности и политиками авторизации для регистрации удостоверений устройств в организации. |
| featureRolloutPolicies                    | [коллекция featureRolloutPolicy](featurerolloutpolicy.md)                                                | Политика выкатки функций, связанная с объектом каталога.                                                                                                          |
| homeRealmDiscoveryPolicies                | Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)                                        | Политика управления поведением проверки подлинности Azure AD для федерационных пользователей.                                                                                             |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | Политика, представляющую по умолчанию безопасность, защищающую от распространенных атак.                                                                                   |
| mobileAppManagementPolicies               | [коллекция mobilityManagementPolicy](mobilitymanagementpolicy.md)                                        | Политика, определяемая конфигурацией автоматической регистрации для приложения управления мобильностью (MDM или MAM).                                                               |
| permissionGrantPolicies                   | Коллекция [permissionGrantPolicy](permissiongrantpolicy.md)                                              | Политика, которая указывает условия, при которых может быть предоставлено согласие.                                                                                            |
| roleManagementPolicies                    | [коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)                     | Представляет политики управления ролью.                                                                                                                                |
| roleManagementPolicyAssignments           | [коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) | Представляет назначения политики управления ролью.                                                                                                                      |
| tokenIssuancePolicies                     | Коллекция [tokenIssuancePolicy](tokenissuancepolicy.md)                                                  | Политика, которая указывает характеристики маркеров SAML, выданных Azure AD.                                                                                        |
| tokenLifetimePolicies                     | Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)                                                  | Политика, контролируемая сроком службы маркера доступа JWT, маркера ID или маркера SAML 1.1/2.0, выданного Azure AD.                                                   |

## <a name="json-representation"></a>Представление JSON
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
  "@odata.type": "#microsoft.graph.policyRoot"
}
```

