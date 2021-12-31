---
title: Перенос приложений Azure AD Graph в Microsoft Graph
description: Описывает, как перенести приложения API Azure Active Directory (Azure AD) в API Microsoft Graph API.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 100fa23b9fdd7b82e201ed2fc6139f62ca93f74c
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651283"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Перенос приложений Azure AD Graph в Microsoft Graph

> [!WARNING]
> **Azure Active Directory (Azure AD) Graph амортизации**. Чтобы избежать потери функциональных возможностей, переадрежите приложения в Microsoft Graph до 30 июня 2022 г., когда конечные точки API Azure AD Graph перестанут отвечать на запросы.
>
> Корпорация Майкрософт продолжит техническую поддержку и применяет исправления безопасности для Azure AD Graph до 30 июня 2022 г., когда все функции и поддержка будут работать. Если до 30 июня 2022 г. не удастся перенести приложения в Microsoft Graph, вы ставите под угрозу их функциональность и стабильность.

[Azure AD Graph является неконтрассленной.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363) Обновите приложения Azure AD Graph, чтобы использовать Microsoft Graph сейчас.

## <a name="why-use-microsoft-graph"></a>Зачем использовать microsoft Graph?

Azure AD Graph доступ только к службам Azure AD. Microsoft Graph предоставляет единую конечную точку для доступа к службам Azure AD и другим Microsoft 365, таким как Microsoft Teams, Microsoft Exchange и Microsoft Intune. Для большинства производственных приложений корпорация Майкрософт Graph полностью поддерживает сценарии Azure AD.

Microsoft Graph также более безопасна и устойчива, чем Azure AD Graph.

Кроме того, microsoft Graph поддерживает множество новых наборов данных и функций Azure AD, недоступных в Azure AD Graph, в том числе в Windows 10 и Enterprise Mobility + Security (EMS). Переключение на microsoft Graph, чтобы воспользоваться этими новыми API с помощью одной конечной точки, включая:

- [Microsoft 365 группового управления](/graph/office365-groups-concept-overview).
- [Внешние приглашения пользователей](/graph/api/resources/invitation).
- Возможность восстановления [пользователей, Microsoft 365 групп,](/graph/api/resources/directory) приложений и директоров служб после удаления.
- [Уведомления webhook для пользователей и групп.](/graph/webhooks)
- Расширенные функции управления лицензией, включая [групповое лицензирование.](/graph/api/group-assignlicense)
- Функции управления удостоверением, такие как:
  - [Привилегированное управление удостоверениями](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) (PIM) для повышения пользователей до привилегированных ролей только при необходимости и в течение ограниченного периода времени.
  - [Доступ к](/graph/api/resources/accessreviewsv2-overview) отзывам о разовом или повторяющихся обзорах доступа для проверки прав доступа пользователя.
  - [Условия использования, позволяющие](/graph/api/resources/agreement) организациям представлять сведения о юридических требованиях или требованиях соответствия требованиям, например уведомления об отказе от ответственности.
- Функции безопасности, такие как:
  - [События риска удостоверения](/graph/api/resources/riskdetection).
  - [Рискованные пользователи](/graph/api/resources/riskyuser).
- [Клиентские библиотеки и примеры,](/graph/) доступные на многих других платформах и языках. SDKs Graph Microsoft предоставляют обнаруживаемый интерфейс для легкого доступа к данным при прозрачной обработке приобретения маркеров, обработки повторной обработки из-за ошибок и регулирования, безопасной обработки перенаправления и сериализации моделей и десериализации.
- Дополнительные [возможности запроса OData,](/graph/query-parameters) поддерживаемые такими ресурсами, как пользователи, группы, приложения и директора служб.

Остальные статьи в этом разделе помогают перенести приложение из Azure AD Graph в Microsoft Graph. Вы найдете:

- Контрольный список, который поможет вам спланировать миграцию.
- Руководство, описывающие определенные различия между API.
- Ссылки на дополнительные ресурсы и примеры для иллюстрации определенных различий.
- Ответы на другие вопросы или проблемы.

## <a name="next-steps"></a>Дальнейшие действия

- Ознакомьтесь [с контрольным списком](migrate-azure-ad-graph-planning-checklist.md) миграции приложений, чтобы спланировать миграцию.
- Ознакомьтесь [с Graph](/graph/overview) microsoft.
- Используйте [Graph Explorer](https://aka.ms/ge) для экспериментов с Microsoft Graph.
- Дополнительные информацию об обновлениях и сроках выполнения см. в [Graph Microsoft Graph Azure AD Graph.](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/)
- Получите [ответы на вопросы](/graph/migrate-azure-ad-graph-faq) о миграции.