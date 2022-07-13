---
title: Тип ресурса policyRoot
description: Тип ресурса, который предоставляет свойства навигации для одноэлементных политик.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d684759f79fbcf4316c97876c7ee7e11be6de2d5
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768114"
---
# <a name="policyroot-resource-type"></a>Тип ресурса policyRoot

Пространство имен: microsoft.graph

Тип ресурса, который предоставляет свойства навигации для одноэлементных политик.

## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи

| Связь                              | Тип                                                                                                      | Описание                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| accessReviewPolicy                        | [accessReviewPolicy](accessreviewpolicy.md)                                                               | Политика, содержащая параметры проверки доступа на уровне каталога.                                                                                                     |
| activityBasedTimeoutPolicies              | [Коллекция activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md)                                    | Политика, которая управляет временем ожидания простоя для веб-сеансов для приложений.                                                                                        |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | Политика, с помощью которой запросы на согласие создаются и управляются для всего клиента.                                                                                  |
| appManagementPolicies                     | Коллекция [appManagementPolicy](appmanagementpolicy.md)                                                  | Политики, которые применяют ограничения управления приложениями для определенных приложений и субъектов-служб, переопределяя defaultAppManagementPolicy.                   |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | Конфигурация политики для самостоятельной регистрации внешних пользователей.                                                                                   |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | Методы проверки подлинности и пользователи, которым разрешено использовать их для входа и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD). |
| authorizationPolicy                       | [Коллекция authorizationPolicy](authorizationpolicy.md)                                                  | Политика, которая управляет Azure AD авторизации.                                                                                                            |
| b2cAuthenticationMethodsPolicy            | [b2cAuthenticationMethodsPolicy](b2cauthenticationmethodspolicy.md)                                       | Политика Azure AD B2C, определяющие способ регистрации конечных пользователей с помощью локальных учетных записей.                                                                                     |
| claimsMappingPolicies                     | Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)                                                  | Политики сопоставления утверждений для протоколов WS-Fed, SAML, OAuth 2.0 и OpenID Connect для маркеров, выданных конкретному приложению.                                   |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | Пользовательские правила, определяющие сценарий доступа.                                                                                                                     |
| crossTenantAccessPolicy                   | [crossTenantAccessPolicy](crosstenantaccesspolicy.md)                           | Пользовательские правила, определяющие сценарий доступа при взаимодействии с внешними Azure AD клиентами.                                                                                                                     |
| defaultAppManagementPolicy                | [tenantAppManagementPolicy](tenantappmanagementpolicy.md)                                                 | Политика на уровне клиента, которая применяет ограничения управления приложениями для всех приложений и субъектов-служб.                                                        |
| externalIdentitiesPolicy                  | [externalIdentitiesPolicy](externalidentitiespolicy.md)                                                   | Представляет политику на уровне клиента, которая определяет, могут ли внешние пользователи покинуть клиент Azure AD с помощью элементов управления самообслуживания. |
| featureRolloutPolicies                    | [Коллекция featureRolloutPolicy](featurerolloutpolicy.md)                                                | Политика развертывания компонентов, связанная с объектом каталога.                                                                                                       |
| homeRealmDiscoveryPolicies                | Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)                                        | Политика для управления Azure AD проверки подлинности для федеративных пользователей.                                                                                          |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | Политика, представляющая параметры безопасности по умолчанию, которые защищают от распространенных атак.                                                                                |
| mobileAppManagementPolicies               | [Коллекция mobilityManagementPolicy](mobilitymanagementpolicy.md)                                        | Политика, которая определяет конфигурацию автоматической регистрации для приложения управления мобильностью (MDM или MAM).                                                            |
| permissionGrantPolicies                   | Коллекция [permissionGrantPolicy](permissiongrantpolicy.md)                                              | Политика, указывавая условия, при которых может быть предоставлено согласие.                                                                                         |
| roleManagementPolicies                    | [Коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)                     | Представляет политики управления ролами.                                                                                                                             |
| roleManagementPolicyAssignments           | [Коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) | Представляет назначения политики управления ролами.                                                                                                                   |
| tokenIssuancePolicies                     | Коллекция [tokenIssuancePolicy](tokenissuancepolicy.md)                                                  | Политика, указывавая характеристики маркеров SAML, выданных Azure AD.                                                                                     |
| tokenLifetimePolicies                     | Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)                                                  | Политика, которая управляет временем существования маркера доступа JWT, маркера идентификатора или токена SAML 1.1/2.0, выданного Azure AD.                                                |

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
