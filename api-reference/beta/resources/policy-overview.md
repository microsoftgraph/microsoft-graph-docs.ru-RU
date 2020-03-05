---
title: Общие сведения об API политики
description: Azure Active Directory использует политики для управления поведением компонентов Azure AD в вашей организации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c439cf8f53a6ce7a9be146e02888ba4a819101ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521616"
---
# <a name="azure-ad-policy-overview"></a>Общие сведения о политике Azure AD

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) использует политики для управления поведением компонентов Azure AD в вашей организации. Политики это настраиваемые правила, которые можно применять к приложениям, субъектам, группам или всем организациям, которым они назначены.

## <a name="what-policies-are-available"></a>Какие политики доступны?

| Тип политики       | Описание | Примеры |
|:-------------|:------------|:------------|
|[activityBasedTimeoutPolicies](activityBasedTimeoutPolicy.md)| Представляет политику, которая управляет автоматическим выходом для веб-сеансов после определенного периода бездействия для приложений, поддерживающих функции времени ожидания на основе действий.| Настройте на портале Azure время ожидания простоя в 15 минут. |
|[claimsMappingPolicies](claimsMappingPolicy.md)| Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением. | Создайте и назначьте политику для пропуска базовых утверждений от маркеров, выданных участнику службы. |
|[homeRealmDiscoveryPolicies](homeRealmDiscoveryPolicy.md)| Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.| Настройте все пользователи для пропуска обнаружения домашней области и маршрутизации непосредственно в ADFS для проверки подлинности. |
|[tokenLifetimePolicies](tokenlifetimepolicy.md)|Представляет срок жизни маркеров доступа, используемых для доступа к защищенным ресурсам.| Настройка особенно конфиденциального приложения с использованием более короткого срока действия маркера по умолчанию.|

## <a name="next-steps"></a>Дальнейшие действия

* Просмотрите различные типы ресурсов политики, перечисленные выше, и их различные методы.
* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
