---
title: Обзор API отчетов об удостоверениях и доступе
description: Обращайтесь к отчетам об удостоверениях и доступе, чтобы получить сведения о том, как пользователи в вашей организации используют приложения в клиенте Azure Active Directory.
localization_priority: Priority
ms.prod: identity-and-access-reports
author: besiler
doc_type: conceptualPageType
ms.openlocfilehash: 567bfdfd848c2a7f1df19b8aad76a68774a6bf0e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129373"
---
# <a name="identity-and-access-reports-api-overview"></a>Обзор API отчетов об удостоверениях и доступе

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью Microsoft Graph вы можете получать доступ к отчетам об удостоверениях и доступе, чтобы получить сведения о том, как пользователи в вашей организации используют приложения в клиенте Azure Active Directory (Azure AD).

## <a name="authorization"></a>Авторизация

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Укажите разрешения, необходимые для доступа к отчетам. Дополнительные сведения см. в [справочнике по разрешениям Microsoft Graph](/graph/permissions-reference) и разделе [Разрешения для отчетов](/graph/permissions-reference#reports-permissions).

## <a name="what-are-identity-and-access-reports"></a>Что такое отчеты об удостоверениях и доступе?

Указанные ниже отчеты об удостоверениях и доступе позволяют понять работу приложений в клиенте.

- Активность приложений AD FS
- Вход в приложение
- Регистрация и использование

### <a name="ad-fs-application-activity"></a>Активность приложений AD FS

В отчете об активности приложений AD FS содержатся сведения о том, как проверяющая сторона настроена с помощью служб федерации Active Directory (AD FS), обобщенные сведения об использовании, а также о том, можно ли перенести настройку проверяющей стороны в Azure Active Directory. Дополнительные сведения см. в ресурсе [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).

### <a name="application-sign-in"></a>Вход в приложение

Оцените использование входов в приложения в своем клиенте с помощью сводного отчета или отчета, содержащего подробные сведения о входах, такие как количество входов и возникали ли какие-либо ошибки при входе. Дополнительные сведения см. в ресурсе [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).

### <a name="registration-and-usage"></a>Регистрация и использование

Узнайте подробнее, как пользователи в вашей организации используют функции Azure AD, такие как самостоятельный сброс пароля и многофакторная проверка подлинности (MFA). Вы можете определить, какие методы проверки подлинности более успешны в вашей организации, с какими типами ошибок сталкиваются пользователи и какую кампанию нужно провести, чтобы помочь пользователям с внедрением самостоятельного сброса паролей и MFA. Дополнительные сведения см. в статье [API отчетов об использовании методов проверки подлинности](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).

## <a name="next-steps"></a>Дальнейшие действия

Ресурсы и API Microsoft Graph открывают новые способы взаимодействия с пользователями и контроля их работы. Чтобы узнать больше:

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).


