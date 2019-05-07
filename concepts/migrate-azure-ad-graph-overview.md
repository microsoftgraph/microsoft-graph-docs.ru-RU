---
title: Перенос приложений Azure AD Graph в Microsoft Graph
description: Описывается перенос приложений API Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 348bc7632c2e2e158d41bb1cc2da9fa3ea755ca6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630232"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Перенос приложений Azure AD Graph в Microsoft Graph

Microsoft Graph полностью заменяет Graph Azure Active Directory (Azure AD). Для большинства рабочих приложений Microsoft Graph уже может полностью поддерживать сценарии Azure AD. Теперь вы должны начать перемещение приложений Azure AD Graph в Microsoft Graph.

Кроме того, Microsoft Graph поддерживает множество новых наборов данных Azure AD и функций, недоступных в Azure AD Graph. Переключитесь на Microsoft Graph, чтобы воспользоваться всеми преимуществами этих новых API, используя одну конечную точку, в том числе:

- [Управление группами Office 365](/graph/office365-groups-concept-overview)
- [Приглашения внешних пользователей](/graph/api/resources/invitation?view=graph-rest-1.0)
- Возможность [восстановления пользователей и групп Office 365](/graph/api/resources/directory?view=graph-rest-1.0) после их удаления
- [Уведомления веб-перехватчика для пользователей и групп](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
- Функции управления удостоверениями, такие как:
  - [Привилегированное управление удостоверениями](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) для повышения уровня доступа пользователей к привилегированным ролям только при необходимости и в течение ограниченного периода времени.
  - [Проверка доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta) для одноразовых или повторяющихся проверок доступа для аттестации прав доступа пользователя
  - [Условия использования](/graph/api/resources/accessreviews-root?view=graph-rest-beta) для предоставления организациям сведений о юридических или нормативных требованиях, таких как уведомления об отказе от ответственности
- Функции безопасности, такие как:
  - [События с риском для идентификации](/graph/api/resources/identityriskevent?view=graph-rest-beta)
  - [Рискованные пользователи](/graph/api/resources/riskyuser?view=graph-rest-beta)
- [Клиентские библиотеки и примеры](/graph/) доступны на многих других платформах и языках

Microsoft Graph предоставляет доступ к большому количеству дополнительных служб, чем просто Azure Active Directory. Он также имеет [шлюз API для Microsoft 365 Services](/graph/).

Остальные статьи в этом разделе помогут переместить приложение из Azure AD Graph в Microsoft Graph. Вы найдете:

- Контрольный список, который поможет вам спланировать.
- Руководство по определенным различиям между API.
- Ссылки на дополнительные ресурсы и примеры, иллюстрирующие конкретные различия.

## <a name="next-steps"></a>Дальнейшие действия

- Изучите [Контрольный список миграции приложений](migrate-azure-ad-graph-planning-checklist.md) , чтобы помочь вам спланировать перемещение.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
- Чтобы узнать больше об обновлениях хода выполнения и временных шкалах, ознакомьтесь со статьей [Microsoft Graph или Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) в центре разработчиков Office.
