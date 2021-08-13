---
title: Перенос приложений Azure AD Graph в Microsoft Graph
description: Описывает, как перенести приложения API Azure Active Directory (Azure AD) в API Microsoft Graph API.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 2eba88d5995d44098473ad138d65df8650cbddb350ad401f731238b8c381be2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163519"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Перенос приложений Azure AD Graph в Microsoft Graph

Корпорация Graph полностью заменяет Azure Active Directory (Azure AD) Graph. Для большинства производственных приложений microsoft Graph уже может полностью поддерживать сценарии Azure AD. Теперь необходимо начать перемещение приложений Azure AD Graph Microsoft Graph.

Кроме того, microsoft Graph поддерживает множество новых наборов данных и функций Azure AD, недоступных в Azure AD Graph. Переключение на microsoft Graph, чтобы воспользоваться этими новыми API с помощью одной конечной точки, включая:

- [Microsoft 365 группового управления](/graph/office365-groups-concept-overview).
- [Внешние приглашения пользователей](/graph/api/resources/invitation?view=graph-rest-1.0).
- Возможность восстановления пользователей и [Microsoft 365 групп](/graph/api/resources/directory?view=graph-rest-1.0) после удаления.
- [Уведомления webhook для пользователей и групп.](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
- Функции управления удостоверением, такие как:
  - [Привилегированное управление удостоверениями](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) для повышения пользователей до привилегированных ролей только при необходимости и в течение ограниченного периода времени.
  - [Доступ к](/graph/api/resources/accessreviews-root?view=graph-rest-beta) отзывам о разовом или повторяющихся обзорах доступа для проверки прав доступа пользователя.
  - [Условия использования, позволяющие](/graph/api/resources/accessreviews-root?view=graph-rest-beta) организациям представлять сведения о юридических требованиях или требованиях соответствия требованиям, например уведомления об отказе от ответственности.
- Функции безопасности, такие как:
  - [События риска удостоверения](/graph/api/resources/identityriskevent?view=graph-rest-beta).
  - [Рискованные пользователи](/graph/api/resources/riskyuser?view=graph-rest-beta).
- [Клиентские библиотеки и примеры,](/graph/) доступные на многих других платформах и языках. SDKs Graph Microsoft предоставляют обнаруживаемый интерфейс для легкого доступа к данным при прозрачной обработке приобретения маркеров, обработки повторной обработки из-за ошибок и регулирования, безопасной обработки перенаправления и сериализации моделей и десериализации.

Microsoft Graph предоставляет доступ к многим дополнительным службам, чем только Azure Active Directory. Это шлюз [API для Microsoft 365 служб.](/graph/)

Остальные статьи в этом разделе помогают переместить приложение из Azure AD Graph в Microsoft Graph. Вы найдете:

- Контрольный список, который поможет вам спланировать.
- Руководство, описывающие определенные различия между API.
- Ссылки на дополнительные ресурсы и примеры для иллюстрации определенных различий.
- Ответы на другие вопросы или проблемы


## <a name="frequently-asked-questions-faq"></a>Вопросы и ответы

### <a name="is-azure-ad-graph-aad-graph-deprecated"></a>Является ли Graph Azure AD (AAD Graph) неподготовленным?  
Да. Начиная с 30 июня 2020 г. мы больше не будем добавлять новые функции в AAD Graph. До 30 июня 2022 г. мы продолжим добавлять критически важные исправления в области безопасности. API больше не будут правильно функционировать после 30 июня 2022 г.

### <a name="how-do-i-know-which-of-my-apps-are-using-aad-graph"></a>Как узнать, какие из моих приложений используют AAD Graph?  
Приложения должны быть зарегистрированы для использования AAD Graph.  Вы можете посмотреть на странице Регистрации приложений на портале клиентов Azure, чтобы узнать, зарегистрировано ли то или иное приложение для использования AAD Graph.

### <a name="how-do-i-know-which-apis-my-applications-are-calling"></a>Как узнать, какие API мои приложения звонят?
Если у вас есть исходный код приложения, вы можете ссылаться на руководства по миграции в этом разделе, чтобы помочь определить, какие API приложение использует и как перенести его в Microsoft Graph. Если у вас нет доступа к исходным кодам приложения, вы можете открыть запрос на поддержку, чтобы получить список API, вызываемого каждым приложением. [](developer-support-help-options.md#open-a-support-request)

### <a name="will-my-existing-aad-graph-apps-continue-to-work"></a>Будут ли мои существующие приложения AAD Graph работать? 
Существующие приложения будут работать без изменений до 30 июня 2022 г. Функция Graph API после этого времени не гарантируется.

### <a name="why-should-i-invest-in-moving-to-microsoft-graph"></a>Зачем мне вкладывать средства в переход на microsoft Graph?  
Microsoft Graph открывает доступ к данным и средствам искусственного интеллекта в Microsoft 365. Она предоставляет единую модель программируемости, с помощью которую можно получить доступ к огромному объему наборов данных и функций в Microsoft 365, Azure, Windows 10 и Enterprise Mobility + Security. Вы можете использовать большой объем данных в Microsoft Graph для создания и управления приложениями для организаций любого масштаба.

### <a name="will-you-release-a-tool-that-helps-me-move-my-apps-from-aad-graph-to-microsoft-graph"></a>Вы выпустите средство, которое поможет мне переместить мои приложения из AAD Graph в Microsoft Graph?  
Пока у нас нет средств для анонса, мы всегда работаем над улучшением работы платформы наших разработчиков. Это включает предоставление инструментов и данных для облегчения сохраняющихся изменений API для приложений.

### <a name="how-do-i-get-help-migrating-my-application"></a>Как получить помощь по переносу приложения?  
См. раздел Следующие действия этой статьи. Если после прочтения у вас есть дополнительные вопросы, вы можете разместить в переполнении стек с тегом или открыть проблему в репозитории `[aadgraph-deprecation]` [API GitHub](https://github.com/microsoftgraph).


## <a name="next-steps"></a>Дальнейшие действия

- Ознакомьтесь [с контрольным списком](migrate-azure-ad-graph-planning-checklist.md) миграции приложений, чтобы спланировать перемещение.
- Ознакомьтесь [с Graph](/graph/overview) microsoft.
- Используйте [Graph Explorer](https://aka.ms/ge) для экспериментов с Microsoft Graph.
- Дополнительные информацию об обновлениях и сроках выполнения см. в [Graph Microsoft Graph Azure AD Graph.](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/)

