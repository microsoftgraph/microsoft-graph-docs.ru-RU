---
title: Работа с API отчета об использовании методов проверки подлинности
description: Отчет об использовании методов проверки подлинности помогает организации понять, как конечные пользователи используют Azure Active Directory, такие как сброс пароля самообслуживления и многофакторная проверка подлинности (MFA).
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 6af5d1805b09add23cfc6c36c7d10acc1e31dc75
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201612"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>Работа с API отчета об использовании методов проверки подлинности

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчеты об использовании методов проверки подлинности помогают понять, как пользователи в организации используют функции Azure Active Directory (Azure AD), такие как многофакторная проверка подлинности (MFA), Self-Service Сброс паролей (SSPR) и проверка подлинности без паролей.

Эти отчеты предоставляют такие сведения, как:

- Количество зарегистрированных пользователей для каждого метода проверки подлинности
- Сколько пользователей зарегистрировано для таких функций, как многофакторная проверка подлинности (MFA), Self-Service сброс пароля (SSPR) и проверка подлинности без паролей.
- Коэффициенты сбоя каждого метода проверки подлинности 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуются указанные ниже разрешения. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Reports.Read.All, AuditLog.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|Reports.Read.All, AuditLog.Read.All|

Чтобы получить доступ к API, требуется одна [из](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) следующих ролей:

* Читатель отчетов
* Читатель сведений о безопасности
* Администратор безопасности
* Глобальный читатель
* Глобальный администратор

## <a name="licenses"></a>Лицензии

Для доступа к использованию и сведениям требуется лицензия Azure AD Premium P1 или P2. Сведения о лицензировании Azure AD с многофакторной проверкой подлинности и [сбросом](https://azure.microsoft.com/pricing/details/active-directory/)пароля самообслуживления (SSPR) можно найти на сайте Azure Active Directory цен.

## <a name="common-requests"></a>Общие запросы

В следующей таблице перечислены некоторые распространенные запросы, которые можно использовать с помощью этого API.

| Операция | Попробовать в песочнице Graph | Описание |
| --------- | --- | ----------- |
| [getCredentialUserRegistrationcount](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | Получите число пользователей, зарегистрированных для сброса пароля самообслуживки и MFA. |
| [getCredentialUsageSummary](/graph/api/resources/credentialusagesummary?view=graph-rest-beta&preserve-view=true) | [GET /credentialusagesummary](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | Получите число пользователей, использующих сброс пароля самообслуживки. |
| [credentialUserRegistrationDetails](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta&preserve-view=true) | [GET /credentialuserregistrationdetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | Получите сведения о пользователе для сброса пароля самообслуживки и действий по регистрации MFA. |
| [userCredentialUsageDetails](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta&preserve-view=true) | [GET /usercredentialusagedetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | Сведения о пользователях для всех действий по сбросу пароля самообслуживаемой. |
| [usersRegisteredByFeature](/graph/api/resources/userregistrationfeaturesummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByFeature](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')&version=beta) | Получите число пользователей, способных выполнять многофакторную проверку подлинности, сброс пароля самообслуживления и проверку подлинности без паролей. |
| [usersRegisteredByMethod](/graph/api/resources/userregistrationmethodsummary?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/usersRegisteredByMethod](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')&version=beta) | Получите число пользователей, зарегистрированных для каждого метода проверки подлинности. |
| [userRegistrationDetails](/graph/api/resources/userRegistrationDetails?view=graph-rest-beta&preserve-view=true) | [GET /authenticationMethods/userRegistrationDetails](https://developer.microsoft.com/graph/graph-explorer?request=reports/authenticationMethods/userRegistrationDetails&version=beta) | Получите сведения о регистрации MFA для всех пользователей. |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, как [развернуть Azure Active Directory самообслуживаемого сброса пароля.](/azure/active-directory/authentication/howto-sspr-deployment)
- Узнайте, как развернуть [Azure Active Directory MFA](/azure/active-directory/authentication/howto-mfa-getstarted).
- Узнайте, как включить [комбинированную регистрацию информации о безопасности.](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined)
