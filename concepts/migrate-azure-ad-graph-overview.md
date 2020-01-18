---
title: Перенос приложений Azure AD Graph в Microsoft Graph
description: Описывается перенос приложений API Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9a817e7fbc056994d98fa32ec945d8e9c2deda5
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234056"
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
- [Клиентские библиотеки и примеры](/graph/) доступны на многих других платформах и языках. Пакеты SDK Microsoft Graph предоставляют обнаруживаемый интерфейс для простого доступа к данным, а также непрозрачно обрабатывает получение маркеров, повторная попытка обработки из-за ошибок и регулирования, обработка безопасного перенаправления и сериализация и десериализация модели.

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
