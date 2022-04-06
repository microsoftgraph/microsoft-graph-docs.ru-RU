---
title: тип ресурсов policyRoot
description: Тип ресурса, подвергая свойства навигации для однотонных политик.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9ca01343954e659da2133543a3454a56be85ecc5
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510185"
---
# <a name="policyroot-resource-type"></a>тип ресурсов policyRoot

Пространство имен: microsoft.graph

Тип ресурса, подвергая свойства навигации для однотонных политик.

## <a name="methods"></a>Methods
Нет

## <a name="properties"></a>Свойства
Нет


## <a name="relationships"></a>Связи
| Связь                              | Тип                                                                                                      | Описание                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | Методы проверки подлинности и пользователи, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD). |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | Конфигурация политики для самостоятельной регистрации внешних пользователей.                                                                                   |
| activityBasedTimeoutPolicies              | [коллекция activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md)                                    | Политика, контролируемая простоем для веб-сеансов для приложений.                                                                                        |
| authorizationPolicy                       | [коллекция authorizationPolicy](authorizationpolicy.md)                                                  | Политика, контролируемая настройками авторизации Azure AD.                                                                                                            |
| claimsMappingPolicies                     | Коллекция [claimsMappingPolicy](claimsmappingpolicy.md)                                                  | Политики сопоставления утверждений для протоколов WS-Fed, SAML, OAuth 2.0 и OpenID Подключение для маркеров, выдаваемого конкретному приложению.                                   |
| homeRealmDiscoveryPolicies                | Коллекция [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md)                                        | Политика управления поведением проверки подлинности Azure AD для федерационных пользователей.                                                                                          |
| permissionGrantPolicies                   | Коллекция [permissionGrantPolicy](permissiongrantpolicy.md)                                              | Политика, которая указывает условия, при которых может быть предоставлено согласие.                                                                                         |
| tokenIssuancePolicies                     | Коллекция [tokenIssuancePolicy](tokenissuancepolicy.md)                                                  | Политика, которая указывает характеристики маркеров SAML, выданных Azure AD.                                                                                     |
| tokenLifetimePolicies                     | Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)                                                  | Политика, контролируемая сроком службы маркера доступа JWT, маркера ID или маркера SAML 1.1/2.0, выданного Azure AD.                                                |
| featureRolloutPolicies                    | [коллекция featureRolloutPolicy](featurerolloutpolicy.md)                                                | Политика выкатки функций, связанная с объектом каталога.                                                                                                       |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | Политика, в которой создаются и управляются запросы на согласие для всего клиента.                                                                                  |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | Пользовательские правила, определяемые сценарием доступа.                                                                                                                     |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | Политика, представляющую по умолчанию безопасность, защищающую от распространенных атак.                                                                                |


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

