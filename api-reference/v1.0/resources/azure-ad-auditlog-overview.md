---
title: Обзор API отчетов об активности
description: Используйте API отчетов об активности в Microsoft Graph для получения доступа к отчетам Azure Active Directory, чтобы отслеживать действия пользователей в клиенте.
localization_priority: Priority
author: khotz
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: cfb622200b5437390c6617c8bd599409fa90925f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091875"
---
# <a name="activity-reports-api-overview"></a>Обзор API отчетов об активности

Пространство имен: microsoft.graph

Azure Active Directory (Azure AD) отслеживает действия пользователей и создает отчеты, помогающие понять, как пользователи переходят к службам Azure AD и используют их. Чтобы анализировать данные в этих отчетах и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.

## <a name="what-are-azure-ad-activity-logs"></a>Что такое журналы действий Azure AD?

Azure AD предоставляет три типа отчетов об активности:

- журналы аудита;
- журналы входа.

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

- [Зарегистрируйте приложение](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal), чтобы соответствовать предварительным требованиям отчетов. 
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

