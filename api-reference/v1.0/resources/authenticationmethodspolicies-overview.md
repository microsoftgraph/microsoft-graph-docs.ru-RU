---
title: Обзор API политики методов проверки подлинности Azure AD
description: Политики методов проверки подлинности определяют, какие методы проверки подлинности могут использоваться пользователями в Azure AD.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: cd3e67f249a4afabc946aaa09c1c4e7448ad99f7
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971079"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a>Обзор API политик методов проверки подлинности Azure AD

Пространство имен: microsoft.graph

Политики методов проверки подлинности определяют методы проверки подлинности и пользователей, которым разрешено использовать их для входа и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD).[](/azure/active-directory/authentication/concept-authentication-methods) Политики методов проверки подлинности, которыми можно управлять в Microsoft Graph, включают ключи безопасности FIDO2 и вход на телефон без пароля с помощью приложения Microsoft Authenticator.

API-интерфейсы политик методов проверки подлинности используются для управления параметрами политики. Например,

* Определите типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.
* Определите пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход на телефон без пароля для входа в Azure AD.
* Определите пользователей или группы пользователей, которым следует напомнить о настройке Microsoft Authenticator для MFA с помощью push-уведомлений.

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a>Какими политиками методов проверки подлинности можно управлять в Microsoft Graph?

|Политика метода проверки подлинности       | Описание |
|:---------------------------|:------------|:------------|
|[emailauthenticationmethodconfiguration](emailauthenticationmethodconfiguration.md)|Определите пользователей, которые могут использовать электронную почту OTP в клиенте Azure AD.|
|[fido2authenticationmethodconfiguration](fido2authenticationmethodconfiguration.md)| Определите ограничения ключей безопасности FIDO2 и пользователей, которые могут использовать их для входа в Azure AD.|
|[microsoftauthenticatorauthenticationmethodconfiguration](microsoftauthenticatorauthenticationmethodconfiguration.md)|Определите пользователей, которые могут использовать Microsoft Authenticator в клиенте Azure AD.|
|[temporaryAccessPassAuthenticationMethod](temporaryaccesspassauthenticationmethodconfiguration.md)|Определите параметры конфигурации и пользователей или группы, которым разрешено использовать метод проверки подлинности временного прохода доступа.|

## <a name="policies-available-for-authentication-methods-registration-campaign"></a>Политики, доступные для кампании регистрации методов проверки подлинности:
|Политика       | Описание |
|:---------------------------|:------------|
|[authenticationMethodsRegistrationCampaign](authenticationmethodsregistrationcampaign.md)| Определите пользователей, которым следует напомнить о настройке метода проверки подлинности (в настоящее время поддерживается только для Microsoft Authenticator).|

## <a name="next-steps"></a>Дальнейшие действия

* Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
