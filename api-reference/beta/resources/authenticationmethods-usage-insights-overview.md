---
title: Работа с API отчета об использовании методов проверки подлинности
description: Отчет об использовании методов проверки подлинности помогает организации понять, как пользователи используют такие возможности Azure Active Directory, как самостоятельный сброс паролей и многофакторная проверка подлинности (MFA).
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 54f3b823fc1d1c62df07ac6dd9e61f5ea32a2871
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135505"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>Работа с API отчета об использовании методов проверки подлинности

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчеты об использовании методов проверки подлинности помогают понять, как пользователи в организации используют функции Azure Active Directory (Azure AD), такие как многофакторная проверка подлинности (MFA), Self-Service сброс пароля (SSPR) и проверка подлинности без пароля.

Эти отчеты предоставляют такие сведения, как:

- Количество пользователей, зарегистрированных для каждого метода проверки подлинности
- Количество пользователей, зарегистрированных для таких функций, как многофакторная проверка подлинности (MFA), Self-Service сброс пароля (SSPR) и проверка подлинности без пароля.
- Процент сбоев каждого метода проверки подлинности 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуются разрешения ниже. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Reports.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

Для доступа к API требуется одна [из](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) следующих ролей:

* Читатель отчетов
* Читатель сведений о безопасности
* Администратор безопасности
* Глобальный читатель
* Глобальный администратор

## <a name="licenses"></a>Лицензии

Для доступа к сведениям об использовании и статистике необходима лицензия Azure AD Premium P1 или P2. Сведения о лицензировании многофакторной идентификации Azure AD и самостоятельного сброса пароля (SSPR) можно найти на сайте цен [Azure Active Directory.](https://azure.microsoft.com/pricing/details/active-directory/)

## <a name="common-requests"></a>Распространенные запросы

В следующей таблице перечислены некоторые распространенные запросы, которые можно использовать с этим API.

| Operation | Попробовать в песочнице Graph | Описание |
| --------- | --- | ----------- |
| [getCredentialUserRegistrationcount](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | Получите количество пользователей, зарегистрированных для самостоятельного сброса паролей и многофаксной многофаксной защиты. |
| [getCredentialUsageSummary](/graph/api/resources/credentialusagesummary?view=graph-rest-beta&preserve-view=true) | [GET /credentialusagesummary](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | Получить количество пользователей, использующих самостоятельный сброс паролей. |
| [credentialUserRegistrationDetails](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationdetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | Получите сведения о пользователях для самостоятельного сброса пароля и регистрации MFA. |
| [userCredentialUsageDetails](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta&preserve-view=true) | [GET /usercredentialusagedetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | Получите сведения о пользователях для всех действий по самостоятельному сбросу паролей. |
| [usersRegisteredByFeature](/graph/api/resources/userregistrationfeaturesummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta) | Получите количество пользователей, способных выполнять многофакторную проверку подлинности, самостоятельный сброс паролей и проверку подлинности без пароля. |
| [usersRegisteredByMethod](/graph/api/resources/userregistrationmethodsummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta) | Получите количество пользователей, зарегистрированных для каждого метода проверки подлинности. |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как развернуть самостоятельный сброс пароля [Azure Active Directory.](/azure/active-directory/authentication/howto-sspr-deployment)
- Узнайте, как развернуть [Azure Active Directory MFA.](/azure/active-directory/authentication/howto-mfa-getstarted)
- Узнайте, как включить [комбинированную регистрацию данных безопасности.](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)
