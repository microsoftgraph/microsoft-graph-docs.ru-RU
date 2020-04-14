---
title: Работа с API отчетов об использовании методов проверки подлинности
description: Отчет об использовании способов проверки подлинности помогает Организации определить, как их конечные пользователи используют функции Azure Active Directory, такие как самостоятельный сброс паролей и многофакторная проверка подлинности (MFA).
localization_priority: Normal
author: kholtz
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: d7f7a8e6cddf308c5681f74ca6546a9467704cc6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472202"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a>Работа с API отчетов об использовании методов проверки подлинности

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчеты об использовании способов проверки подлинности помогают определить, как пользователи в вашей организации используют возможности Azure Active Directory (Azure AD), такие как самостоятельный пароль и многофакторная проверка подлинности (MFA).

В этих отчетах представлены следующие сведения:

- Методы проверки подлинности более успешны для Организации. 
- Сведения об ошибках, с которыми работает конечный пользователь.
- Какую кампанию необходимо выполнить, чтобы помочь конечным пользователям принять использование REST пароля и MFA для самостоятельного пароля.

## <a name="common-requests"></a>Общие запросы

В следующей таблице перечислены некоторые распространенные запросы, которые можно использовать с этим API.

| Operation | Попробовать в песочнице Graph | Описание |
| --------- | --- | ----------- |
| [жеткредентиалусеррегистратионкаунт](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta) | [ПОЛУЧЕНИЕ/кредентиалусеррегистратионкаунт](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta) | Получение числа пользователей, зарегистрированных для самостоятельного сброса пароля и MFA. |
| [жеткредентиалусажесуммари](/graph/api/resources/credentialusagesummary?view=graph-rest-beta) | [ПОЛУЧЕНИЕ/кредентиалусажесуммари](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | Получение числа пользователей, использующих самостоятельный сброс пароля. |
| [кредентиалусеррегистратиондетаилс](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) | [ПОЛУЧЕНИЕ/кредентиалусеррегистратиондетаилс](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | Получение сведений о пользователях для самостоятельного сброса пароля и действий регистрации MFA. |
| [усеркредентиалусажедетаилс](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) | [ПОЛУЧЕНИЕ/усеркредентиалусажедетаилс](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | Получение сведений о пользователях для всех действий самостоятельного сброса пароля. |

## <a name="licenses"></a>Лицензии

Отчеты об использовании доступны для лицензионных функций, которые используют преимущества самостоятельного сброса пароля и MFA в клиенте.

## <a name="next-steps"></a>Дальнейшие действия

- Сведения о [развертывании средства самообслуживания Azure Active Directory для самостоятельного сброса пароля](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).
- Узнайте, как развернуть [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).
- Узнайте, как включить [регистрацию сведений о безопасности в сочетании](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).



