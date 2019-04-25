---
title: Обзор API журнала аудита Azure AD
description: Azure Active Directory (Azure AD) отслеживает действия пользователя, регистрирует показатели и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их. Чтобы анализировать данные, лежащие в основе этих отчетов, и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.
localization_priority: Priority
ms.openlocfilehash: 89be0007ae6c13fb48ba165ca991f5dfa9d9b9cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543897"
---
# <a name="azure-ad-audit-log-api-overview"></a>Обзор API журнала аудита Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) отслеживает действия пользователя, регистрирует показатели и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их. Чтобы анализировать данные, лежащие в основе этих отчетов, и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.

## <a name="what-are-azure-ad-activity-logs"></a>Что такое журналы аудита Azure AD?

Azure AD предоставляет два типа журналов активности:

- журналы аудита; 
- журналы входа.

### <a name="audit-logs"></a>Журналы аудита

Отчет об активности журналов аудита предоставляет доступ к истории всех выполненных задач в клиенте. Отчет журналов аудита предоставляет записи о действиях системы для соответствия требованиям. Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:

- Кто предоставил доступ группе администраторов к каталогу пользователя?

- Какие пользователи входят в недавно приобретенное приложение?

- Сколько сбросов паролей выполнено в каталоге?

### <a name="sign-in-logs"></a>Журналы входа

Отчет о действиях входа помогает определить, кто выполнял задачи, указанные в отчетах журнала аудита. Отчет о действиях входа помогает ответить на представленные ниже вопросы.

- Какой шаблон входа использует пользователь?
- Сколько пользователей выполнило вход за прошлую неделю?
- Какое состояние у этих входов?

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>Как можно использовать API журнала аудита в Microsoft Graph?

Ниже приведены популярные запросы для работы с данными журнала аудита.

Операция | URL-адрес
:----------|:----
Получение действий пользователей клиента | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
Получение входов пользователей клиента | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a>Какие лицензии нужны?

Отчеты журнала аудита доступны для компонентов, на которые у вас есть лицензии.  Если у вас есть лицензия на определенный компонент, вам будет предоставлен доступ к соответствующим журналам аудита.

Например, вам нужна лицензия на Azure AD Premium P1, чтобы получить доступ к отчетам аудита самостоятельного изменения паролей.  Дополнительные сведения см. на странице [лицензий Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

Для отчетов входов требуется лицензия на Azure AD Premium.

Дополнительные сведения см. на странице [Цены на Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Дальнейшие действия

- [Зарегистрируйте приложение](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям журнала аудита. 
- Ознакомьтесь с примерами журналов [аудита](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) и [входа](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).  
- Изучите действия и ресурс [directoryAudit](directoryaudit.md).
- Изучите действия и ресурс [signIn](signin.md). 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
