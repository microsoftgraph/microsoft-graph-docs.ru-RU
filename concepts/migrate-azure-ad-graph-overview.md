---
title: Перенос Графа Azure Active Directory (Azure AD) в Microsoft Graph
description: Узнайте, как перенести приложения Azure Active Directory (Azure AD) Graph в Microsoft Graph перед Azure AD Graph.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 12e080c58217a159d011a14a854f1bab3456f5fc
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577758"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Перенос Azure AD Graph в Microsoft Graph

> [!IMPORTANT]
> Azure Active Directory (Azure AD) — нерекомендуемый, но не будет прекращен 30 июня 2022 г., как было объявлено [ранее](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363). Внимательно высмеяв ваши отзывы о проблемах миграции такой критической зависимости, мы откладываем дату прекращения использования по крайней мере до конца этого года, 2022 г. В середине календарного года мы предоставьте обновление о прекращении поддержки, включая выпуск дополнительных средств для переноса приложений.

## <a name="why-use-microsoft-graph"></a>Зачем использовать Microsoft Graph?

Microsoft Graph — это наша лучшая в своем классе поверхность API. Она предлагает единую конечную точку для доступа к Azure AD и службам Microsoft 365, таким как Microsoft Teams и Microsoft Intune. Использование API Graph Microsoft более чем в два раза больше, чем Azure AD Graph, и за последние два года мы добавили [167 новых функций](https://developer.microsoft.com/en-us/graph/changelog). Все новые функции будут доступны только через Microsoft Graph.

Microsoft Graph также является более безопасным и устойчивым, чем Azure AD Graph.

Microsoft Graph имеет все возможности, доступные в Azure AD Graph, и новые API, такие как защита идентификации и методы проверки подлинности. Клиентские библиотеки предлагают встроенную поддержку таких функций, как обработка повторных попыток, безопасные перенаправления, прозрачная проверка подлинности и сжатие полезных данных.

Переключитесь на Microsoft Graph, чтобы воспользоваться преимуществами этих расширенных возможностей и:

- [Управление группой Microsoft 365](/graph/office365-groups-concept-overview).
- [Приглашения внешних пользователей](/graph/api/resources/invitation).
- Возможность восстановления пользователей, групп, приложений и субъектов-служб [Microsoft 365](/graph/api/resources/directory) после их удаления.
- [Уведомления веб-перехватчиков о пользователях и группах](/graph/webhooks).
- Расширенные функции управления лицензиями, включая [групповое лицензирование](/graph/api/group-assignlicense).
- Функции управления удостоверениями, такие как:
  - [Управление привилегированными пользователями](/graph/api/resources/privilegedidentitymanagement-root) (PIM) для повышения прав пользователей до привилегированных ролей только при необходимости и в течение ограниченного периода времени.
  - [Проверка доступа](/graph/api/resources/accessreviewsv2-overview) для однофакторной или повторяющейся проверки доступа для аттестации прав доступа пользователя.
  - [Условия использования, позволяющие](/graph/api/resources/agreement) организациям предоставлять сведения о юридических требованиях или требованиях к соответствию, например уведомления об отказе от ответственности.
- Функции безопасности, такие как:
  - [События риска идентификации](/graph/api/resources/riskdetection).
  - [Рискованные пользователи](/graph/api/resources/riskyuser).
- [Клиентские библиотеки и примеры, доступные](/graph/) на многих других платформах и языках. Пакеты SDK Microsoft Graph предоставляют доступный для обнаружения интерфейс для легкого доступа к данным при прозрачной обработке получения маркеров, обработки повторных попыток из-за ошибок и регулирования, безопасной обработки перенаправления, сериализации и десериализации модели.
- [Дополнительные возможности запросов OData,](/graph/query-parameters) поддерживаемые такими ресурсами, как пользователи, группы, приложения и субъекты-службы.

Остальные статьи в этом разделе помогут вам перенести приложение из Azure AD Graph в Microsoft Graph. Вы найдете:

- Контрольный список для планирования миграции.
- Руководство, описывающий конкретные различия между API.
- Ссылки на дополнительные ресурсы и примеры для иллюстрации конкретных различий.
- Часто задаваемые вопросы о других вопросах или проблемах.

Отправьте любые другие вопросы, открытые проблемы и запросы функций через Microsoft Q&A с помощью [тега azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html).

## <a name="next-steps"></a>Дальнейшие действия

- Ознакомьтесь с [контрольным списком миграции](migrate-azure-ad-graph-planning-checklist.md) приложений, чтобы спланировать миграцию.
- [Изучите основные](/graph/overview) понятия и методики Microsoft Graph.
- Используйте [песочницу Graph](https://aka.ms/ge) для экспериментов с Microsoft Graph.
- Дополнительные сведения об обновлениях хода выполнения и временных шкалах в [Microsoft Graph или Azure AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/).
- Получите [ответы на вопросы](/graph/migrate-azure-ad-graph-faq) о миграции.