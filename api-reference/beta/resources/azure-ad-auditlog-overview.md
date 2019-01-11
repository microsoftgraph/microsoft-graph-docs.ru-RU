---
title: Общие сведения о интерфейс API журнала аудита Azure AD
description: Azure Active Directory (Azure AD) отслеживает показатели активности и входа пользователя и создает аудита отчеты по журналу, которые помогут вам понять, как пользователям доступ к и эффективного использования служб Azure AD. Используйте Microsoft Graph API для Azure AD для анализа данных базового этих отчетов и для создания пользовательских решений для конкретных требованиям вашей организации.
localization_priority: Priority
ms.openlocfilehash: 07d285ce4e7fbf736900c1d6d4acdf159b451424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826224"
---
# <a name="azure-ad-audit-log-api-overview"></a>Общие сведения о интерфейс API журнала аудита Azure AD

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Azure Active Directory (Azure AD) отслеживает показатели активности и входа пользователя и создает аудита отчеты по журналу, которые помогут вам понять, как пользователям доступ к и эффективного использования служб Azure AD. Используйте Microsoft Graph API для Azure AD для анализа данных базового этих отчетов и для создания пользовательских решений для конкретных требованиям вашей организации.

## <a name="what-are-azure-ad-activity-logs"></a>Что такое действие Azure AD журналы?

Azure AD обеспечивает два типа журналы активности.

- журналы аудита 
- журналы входа

### <a name="audit-logs"></a>Журналы аудита

Отчете журналы аудита предоставляет доступ к журналу каждой задачи выполняется в вашего клиента. Отчет о журналы аудита предоставляет записей действий системы для соответствия требованиям. Помимо прочего предоставленных данных позволяет вам устранения распространенных сценариев, таких как:

- Доступ к группе администрирования, предоставленные пользователю каталога?

- Пользователей, которые вход с использованием недавно приобретенного приложения?

- Сбрасывает пароли сколько были внесены в пределах каталога?

### <a name="sign-in-logs"></a>Войдите в журналах

Войти в отчете приводятся рекомендации по определению, выполнения задач, о которых сообщает отчеты по журналу аудита. Войти в отчете помогает ответить на вопросы:

- Что такое входа в шаблоне пользователя?
- Сколько пользователей вышли ходе за прошлую неделю?
- Что такое состояние этих войти в систему?

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>Что можно сделать с помощью журнала аудита интерфейсы API в Microsoft Graph

Вот популярные запросы для работы с данными журнала аудита.

Операция | URL-адрес
:----------|:----
Получение клиентом действия пользователя | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
Получение клиентом входы | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a>Какие лицензий требуется?

Отчеты по журналу аудита, доступных для функции, которые ли применена лицензия.  Если у вас есть лицензии для конкретного компонента, также имеют доступ к его журналы аудита.

Например требуется лицензия P1 Azure AD Premium для доступа к отчетам аудита самостоятельного пароль.  Для получения дополнительных сведений см. [: Лицензирование Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

Входа в отчетах требуется лицензия на Azure AD Premium.

Для получения дополнительных сведений см [Цена Azure AD](https://azure.microsoft.com/pricing/details/active-directory/).

## <a name="next-steps"></a>Дальнейшие действия

- [Регистрация приложения](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) для удовлетворения необходимых компонентов журнала аудита. 
- Сведения из [журнала аудита](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) и [примеры, вход](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).  
- Ознакомьтесь с [directoryAudit](directoryaudit.md) ресурсов и действия.
- Просмотрите [входить](signin.md) ресурсов и действия. 
