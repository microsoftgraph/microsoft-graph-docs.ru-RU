---
title: Обзор API отчетов об активности
description: Используйте API отчетов об активности в Microsoft Graph для получения доступа к отчетам Azure Active Directory, чтобы отслеживать действия пользователей в клиенте.
localization_priority: Priority
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: eba6b2af8dd6437d8996ab0bc2304c99eb7b4ac1
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129448"
---
# <a name="activity-reports-api-overview"></a>Обзор API отчетов об активности

Пространство имен: microsoft.graph

Azure Active Directory (Azure AD) отслеживает действия пользователей и создает отчеты, помогающие понять, как пользователи переходят к службам Azure AD и используют их. Чтобы анализировать данные в этих отчетах и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.

Доступность этих отчетов об активности определяется политиками хранения данных Azure AD. Подробнее см. в статье [Политики хранение данных](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="what-are-azure-ad-activity-logs"></a>Что такое журналы аудита Azure AD?

Azure AD предоставляет следующие типы отчетов об активности:

- Аудиты каталога
- Входы

### <a name="directory-audits"></a>Аудиты каталога

Отчет аудитов каталога предоставляет доступ к истории всех выполненных задач в клиенте. Отчет аудитов каталога предоставляет записи о действиях системы для обеспечения соответствия требованиям. Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:

- Кто предоставил доступ группе администраторов к каталогу пользователя?
- Какие пользователи входят в недавно приобретенное приложение?
- Сколько сбросов паролей выполнено в каталоге?

### <a name="sign-ins"></a>Входы

Отчет о входах помогает определить, кто выполнял задачи, указанные в отчетах аудитов каталога. Отчет о входах помогает ответить на представленные ниже вопросы.

- Какой шаблон входа использует пользователь?
- Сколько пользователей выполнило вход за прошлую неделю?
- Какое состояние у этих входов?

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>Как можно использовать API журнала аудита в Microsoft Graph?

Ниже приведены популярные запросы для работы с данными журнала аудита.

Operation | URL-адрес
:----------|:----
Получение действий пользователей клиента | [GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
Получение входов пользователей клиента | [GET https://graph.microsoft.com/v1.0/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a>Какие лицензии нужны?

Отчеты об активности доступны для компонентов, на которые у вас есть лицензии. Если у вас есть лицензия на определенный компонент, вам будет предоставлен доступ к соответствующим отчетам.

Например, вам нужна лицензия на Azure AD Premium P1, чтобы получить доступ к отчетам аудита самостоятельного изменения паролей.  Дополнительные сведения см. на странице [лицензий Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

Для отчетов входов требуется лицензия на Azure AD Premium.

Дополнительные сведения см. на странице [Цены на Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Дальнейшие действия

- [Зарегистрируйте приложение](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям отчетов. 
- Сведения о том, как получить журналы аудита при проверке подлинности с помощью сертификатов, см. в [руководстве по получению данных с помощью API отчетов Azure Active Directory с сертификатами](/azure/active-directory/reports-monitoring/tutorial-access-api-with-certificates).   
- Изучите действия и ресурс [directoryAudit](directoryaudit.md).
- Изучите действия и ресурс [signIn](signin.md). 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
  ]
}
-->
