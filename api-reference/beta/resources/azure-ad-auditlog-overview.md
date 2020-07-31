---
title: Обзор API отчетов об активности
description: Используйте API отчетов об активности в Microsoft Graph для получения доступа к отчетам Azure Active Directory, чтобы отслеживать активность пользователей в клиенте.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: microsoft-identity-platform
author: kholtz
ms.openlocfilehash: 2eea2c8b2e169d11b7ca081d69ab02bf0e2ae66c
ms.sourcegitcommit: ff3fd4ead2b864ce6abb79915a0488d0562347f8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2020
ms.locfileid: "46524292"
---
# <a name="activity-reports-api-overview"></a>Обзор API отчетов об активности

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) отслеживает действия пользователя и создает отчеты журнала аудита, помогающие понять, как пользователи переходят к службам Azure AD и используют их. Чтобы анализировать данные в этих отчетах и создавать настраиваемые решения в соответствии с конкретными требованиями организации, используйте API Microsoft Graph в Azure AD.

## <a name="what-are-activity-reports"></a>Что такое отчеты об активности?

Azure AD предоставляет три типа отчетов об активности:

- Аудиты каталога 
- Входы
- Подготовка

### <a name="directory-audits"></a>Аудиты каталога

Отчет аудитов каталога предоставляет доступ к истории всех выполненных задач в клиенте. Отчет аудитов каталога предоставляет записи о действиях системы для соответствия требованиям. Помимо прочего, предоставляемые данные позволяют рассматривать типичные сценарии, например:

- Кто предоставил доступ группе администраторов к каталогу пользователя?
- Какие пользователи входят в недавно приобретенное приложение?
- Сколько сбросов паролей выполнено в каталоге?

### <a name="sign-ins"></a>Входы

Отчет о входах помогает определить, кто выполнял задачи, указанные в отчетах аудитов каталога. Отчет о входах помогает ответить на представленные ниже вопросы.

- Какой шаблон входа использует пользователь?
- Сколько пользователей выполнило вход за прошлую неделю?
- Какое состояние у этих входов?

### <a name="provisioning"></a>Подготовка

Отчет о подготовке позволяет просматривать все действия, выполненные службой подготовки Azure AD. Отчет о подготовке помогает ответить на представленные ниже вопросы.

- Какие группы были успешно созданы в ServiceNow?
- Какие роли были импортированы из Amazon Web Services?
- Каких пользователей не удалось создать из Workday?

## <a name="what-can-i-do-with-activity-reports-in-microsoft-graph"></a>Как можно использовать отчеты об активности в Microsoft Graph?

Ниже приведены популярные запросы для работы с данными отчетов.

Operation | URL-адрес
:----------|:----
Получение действий пользователей клиента | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
Получение входов пользователей клиента | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
Получение журналов подготовки | [https://graph.microsoft.com/beta/auditLogs/provisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/Provisioning&version=beta)

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
- Изучите ресурс [provisioningObjectSummary](provisioningobjectsummary.md).
