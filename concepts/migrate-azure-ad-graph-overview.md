---
title: Перенос приложений Azure AD Graph в Microsoft Graph
description: Описывает миграцию приложений API Azure Active Directory (Azure AD) в API Microsoft Graph API.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: a59b32d7c042d7a6300abb97dc602700a769d3cf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333843"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Перенос приложений Azure AD Graph в Microsoft Graph

> [!IMPORTANT]
> Azure Active Directory (Azure AD) Graph, но не будет отменена 30 июня 2022 г., как было объявлено [ранее](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363). Внимательно выслушав ваши отзывы о проблемах переноса такой критической зависимости, мы задерживаем дату выхода на пенсию по крайней мере до конца этого года, 2022 г. В середине календарного года мы предоберем обновление для выхода на пенсию, в том числе выпустим дополнительные средства, которые помогут вам перенести приложения.

## <a name="why-use-microsoft-graph"></a>Зачем использовать microsoft Graph?

Microsoft Graph представляет нашу лучшую в своей породе поверхность API. Он предлагает единую конечную точку для доступа к службам Azure AD и Microsoft 365, таким как Microsoft Teams и Microsoft Intune. Использование Graph API в Microsoft более чем в два раза больше, чем в Azure AD Graph, и за последние два года мы добавили [167 новых функций](https://developer.microsoft.com/en-us/graph/changelog). Все новые функции будут доступны только в microsoft Graph.

Microsoft Graph также более безопасна и устойчива, чем Azure AD Graph.

Microsoft Graph имеет все возможности, доступные в Azure AD Graph и новых API, таких как защита удостоверений и методы проверки подлинности. Клиентские библиотеки предоставляют встроенную поддержку таких функций, как обработка повторной обработки, безопасные перенаправления, прозрачная проверка подлинности и сжатие полезной нагрузки.

Переключение Graph Microsoft, чтобы воспользоваться этими расширенными возможностями и:

- [Microsoft 365 группового управления](/graph/office365-groups-concept-overview).
- [Внешние приглашения пользователей](/graph/api/resources/invitation).
- Возможность восстановления [пользователей, Microsoft 365 групп, приложений](/graph/api/resources/directory) и директоров служб после удаления.
- [Уведомления webhook для пользователей и групп](/graph/webhooks).
- Расширенные функции управления лицензией, включая [групповое лицензирование](/graph/api/group-assignlicense).
- Функции управления удостоверением, такие как:
  - [Привилегированное управление удостоверениями](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) (PIM) для повышения пользователей до привилегированных ролей только при необходимости и в течение ограниченного периода времени.
  - [Доступ к](/graph/api/resources/accessreviewsv2-overview) отзывам о разовом или повторяющихся обзорах доступа для проверки прав доступа пользователя.
  - [Условия использования, позволяющие](/graph/api/resources/agreement) организациям представлять сведения о юридических требованиях или требованиях соответствия требованиям, например уведомления об отказе от ответственности.
- Функции безопасности, такие как:
  - [События риска удостоверения](/graph/api/resources/riskdetection).
  - [Рискованные пользователи](/graph/api/resources/riskyuser).
- [Клиентские библиотеки и примеры,](/graph/) доступные на многих других платформах и языках. Microsoft Graph SDKs предоставляет обнаруживаемый интерфейс для легкого доступа к данным при прозрачной обработке приобретения маркеров, обработки повторной обработки из-за ошибок и регулирования, безопасной обработки перенаправления и сериализации моделей и десеркализации.
- [Дополнительные возможности запроса OData](/graph/query-parameters), поддерживаемые такими ресурсами, как пользователи, группы, приложения и директора служб.

Остальные статьи в этом разделе помогают перенести приложение из Azure AD Graph в Microsoft Graph. Вы найдете:

- Контрольный список, который поможет вам спланировать миграцию.
- Руководство, описывающие определенные различия между API.
- Ссылки на дополнительные ресурсы и примеры для иллюстрации определенных различий.
- Ответы на другие вопросы или проблемы.

Отправка любых других вопросов, открытых проблем и запросов на функции через Microsoft Q&A с помощью тега [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html).

## <a name="next-steps"></a>Дальнейшие действия

- Ознакомьтесь [с контрольным списком](migrate-azure-ad-graph-planning-checklist.md) миграции приложений, чтобы спланировать миграцию.
- [Ознакомьтесь с Graph](/graph/overview) microsoft.
- Используйте [Graph Explorer](https://aka.ms/ge) для экспериментов с Microsoft Graph.
- Дополнительные информацию об обновлениях и сроках выполнения см. в [Graph Microsoft Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/).
- Получите [ответы на вопросы](/graph/migrate-azure-ad-graph-faq) о миграции.