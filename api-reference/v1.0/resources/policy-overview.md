---
title: Обзор API политики
description: Azure Active Directory использует политики для управления поведением функций Azure AD в организации.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 4f1b705b13518bdd1b5ede0c85c20dad0a593e2a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128479"
---
# <a name="azure-ad-policy-overview"></a>Обзор политики Azure AD

Пространство имен: microsoft.graph



Azure Active Directory (Azure AD) использует политики для управления поведением функций Azure AD в организации. Политики — это настраиваемые правила, которые можно применять к приложениям, основным службам, группам или во всей организации, для которую они назначены.

## <a name="what-policies-are-available"></a>Какие политики доступны?

| Тип политики       | Описание | Примеры |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| Представляет политику, которая управляет автоматическим выходом из веб-сеансов после периода бездействия для приложений, которые поддерживают функцию времени ожидания на основе действий.| Настройте на портале Azure период неактивности, который составляет 15 минут. |
|[claimsMappingPolicies](claimsMappingPolicy.md)| Представляет политики сопоставления утверждений для протоколов WS-Fed, SAML, OAuth 2.0 и OpenID Connect для маркеров, выдаваемой определенному приложению. | Создайте и назначьте политику, чтобы опустить основные утверждения из маркеров, выданных для основного службы. |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| Представляет политику для управления поведением проверки подлинности Azure Active Directory для федерационных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федерационных доменах.| Настройте всех пользователей так, чтобы они пропускали обнаружение домашней области и перенанастроялись непосредственно в ADFS для проверки подлинности. |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|Представляет срок действия маркеров доступа, используемых для доступа к защищенным ресурсам.| Настройте приложение с особой конфиденциальной настройкой с более коротким сроком действия маркера по умолчанию.|
|[tokenIssuancePolicy](tokenIssuancePolicy.md)|Представляет политику для указания характеристик маркеров SAML, выдавляемой Azure AD.| Настройте алгоритм подписи или версию маркера SAML, которая будет использоваться для выдачи маркера SAML.
|[identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)|Представляет политику по умолчанию для безопасности Azure AD.| Настройте политику по умолчанию для безопасности Azure AD, чтобы защититься от распространенных атак.

## <a name="next-steps"></a>Дальнейшие действия

* Просмотрите различные типы повторного управления политиками, перечисленные выше, и их различные методы.
* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

