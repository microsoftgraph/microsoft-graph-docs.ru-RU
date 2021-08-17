---
title: Azure Active Directory (Azure AD) Graph microsoft Graph вопросы миграции
description: Azure Active Directory (Azure AD) Graph microsoft Graph вопросы миграции.
author: FaithOmbongi
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e563b84db22589fb64af560e90c212e1c8348657
ms.sourcegitcommit: 04fee41bc130718a4c16e41bc244ad384bba2ac3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2021
ms.locfileid: "58363688"
---
# <a name="azure-active-directory-azure-ad-graph-to-microsoft-graph-migration-faq"></a>Azure Active Directory (Azure AD) Graph microsoft Graph вопросы миграции

В этой статье данная статья содержит ответы на часто задамые вопросы о переносе из Azure AD Graph в Microsoft Graph.

## <a name="how-is-microsoft-graph-different-from-azure-ad-graph-and-why-should-i-migrate-my-apps"></a>Чем Microsoft отличается Graph Azure AD Graph и почему следует перенести приложения?

API Azure AD Graph предоставляет доступ только к службам Azure AD. API microsoft Graph предоставляет единую конечную точку для доступа к службам Azure AD и другим службы Майкрософт, таким как Microsoft Teams, Microsoft Exchange и Microsoft Intune.

Microsoft Graph также более безопасна и устойчива, чем Azure AD Graph. По этой причине Azure AD Graph с 30 июня 2020 г. и будет отменен 30 июня 2022 г. После 30 июня 2022 г. ваши приложения больше не будут получать ответы из конечной точки Azure AD Graph. Миграция в microsoft Graph, чтобы избежать потери функциональных возможностей.

## <a name="as-a-developer-how-do-i-identify-apps-that-use-azure-ad-graph"></a>Как определить приложения, которые используют Azure AD Graph?

Выполните следующие действия, чтобы определить приложения с зависимостью от Azure AD Graph:

### <a name="step-1-scan-the-application-source-code"></a>Шаг 1. Сканирование исходных кодов приложений

Если у вас есть исходный код приложения, поиск `https://graph.windows.net/` URI в коде. Это конечная точка Azure AD Graph и приложения, которые называют эту конечную точку, используют Azure AD Graph. Зафиксировать значение ID приложения пострадавшего приложения.

### <a name="step-2-check-the-apps-api-permissions-on-the-azure-portal"></a>Шаг 2. Проверка разрешений API приложения на портале Azure

1. Во входе на портал [Azure](https://portal.azure.com) в качестве глобального администратора.
1. Поиск и выбор **Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В **окне регистраций приложений** выберите вкладку **Все приложения,** а затем выберите параметр **Добавить фильтры.** Выберите параметр **Application (client) ID** из списка доступных фильтров и выберите **Apply**.  Всплывет фильтр.
1. В текстовом окне введите ИД приложения, полученный в шаге 1, и выберите **Применить**. Список сужен до указанного приложения.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="Фильтрация по приложениям по ID приложения." border="true":::

1. Выберите приложение. Это показывает меню приложения.
1. В левой области окна выберите **разрешения API.** При этом раскрываются настроенные разрешения API для вашего приложения, в том числе Graph Azure AD.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/configuredPermissions.png" alt-text="Список разрешений API приложения с портала Azure." border="true":::


## <a name="as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph"></a>Как определить приложения в клиенте, которые используют Azure AD Graph?

Используйте один из следующих трех методов для идентификации приложений в клиенте с зависимостью от Azure AD Graph.

### <a name="method-1-through-network-proxy-logs"></a>Метод 1. С помощью журналов прокси-серверов сети

Проверьте журналы трафика сетевого сервера с помощью прокси-фильтра для любых приложений, вызываемой `https://graph.windows.net/` конечной точкой. Эти приложения используют Azure AD Graph.

### <a name="method-2-use-the-app-registrations-menu-of-the-azure-portal"></a>Метод 2. Используйте меню регистрации приложений на портале Azure

1. Во входе на портал [Azure](https://portal.azure.com) в качестве глобального администратора.
1. Поиск и выбор **Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В окне регистраций приложений выберите вкладку **Все приложения,** а затем выберите параметр **Добавить фильтры.** Выберите параметр **Запрашиваемого API** из списка доступных фильтров и выберите **Apply**. Всплывет **фильтр запрашиваемой API.**

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI.png" alt-text="Фильтрация приложений по запрашиваемой API." border="true":::

5. Выберите **API Майкрософт**. Выберите падение **API** и **выберите** Azure Active Directory Graph. Нажмите **Применить**. В этом списке перечислены все приложения с зависимостью от Azure AD Graph.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI-AAD.png" alt-text="Фильтруются приложения, которые используют azure AD Graph." border="true":::

### <a name="method-3-use-a-powershell-script"></a>Метод 3. Использование сценария PowerShell

Скачайте и [запустите этот скрипт PowerShell.](https://github.com/microsoft/AzureADGraphApps)



## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-how-do-i-find-the-details-of-each-app-including-its-owner"></a>Корпорация Майкрософт отправила мне электронное письмо со списком ID приложений с помощью Azure AD Graph. Как найти сведения о каждом приложении, включая его владельца?

1. Во входе на портал [Azure](https://portal.azure.com) в качестве глобального администратора.
1. Поиск и выбор **Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В окне регистраций приложений выберите вкладку **Все приложения** и выберите параметр **Добавить фильтры.** Выберите параметр **Application (client) ID** из списка доступных фильтров и выберите **Apply**.  Всплывет фильтр.
1. Введите ID приложения в текстовом окне и выберите **Применить**. Список сужен до указанного приложения.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="Фильтрация по приложениям по ID приложения." border="true":::

6. Выберите приложение. Это показывает меню приложения. В левой области окна параметры меню, такие как **Owners,** позволяют получить сведения о приложении.

## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-are-these-all-the-affected-apps"></a>Корпорация Майкрософт отправила мне электронное письмо со списком ID приложений с помощью Azure AD Graph. Это все затронутые приложения?

В этом списке запечатлены только приложения, используемые в течение последних 28 дней и называемые конечным Graph Azure AD. Так как некоторые приложения могут использовать сезонные, их ID приложения может быть захвачен в списке одного месяца, но не в другом. Чтобы получить полный список затронутых приложений, рекомендуется следовать одному из [трех](#as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph) перечисленных ранее методов.

## <a name="im-a-subscription-owner-and-microsoft-sent-me-an-email-about-azure-ad-graph-deprecation-with-a-list-of-app-ids-what-should-i-do"></a>Я владелец подписки, и Корпорация Майкрософт отправила мне сообщение об амортизации Azure AD Graph со списком ID приложений. Что мне делать?

Получаемая электронная почта включает в себя ID клиента, связанные с ID-адресами приложений. Выполните следующие действия, чтобы получить технические контактные данные для определенных клиентов.
1. Во входе на [портал Azure в](https://portal.azure.com) качестве администратора.
1. Если вы владелец подписки в нескольких клиентах Azure AD, сначала переключение на соответствующий клиент или каталог.
    1. В правом верхнем окне выберите значок профиля и выберите **каталог Switch.** Это показывает **параметры портала | Окно каталогов и подписки.** 
    1. Из списка используйте вкладку **Switch,** чтобы перейти в каталог, который соответствует ИД клиента, полученному в электронной почте. Активный каталог помечен **current**.
    1. Закройте окно.
1. В соответствующем каталоге поиск и **выбор** Azure Active Directory . Это показывает меню для активного клиента. 
1. В левой области окна в статье **Управление** выберите **свойства**.
1. В **окне** свойств клиента сначала убедитесь, что значение tenant ID совпадает с ИД клиента, полученным в электронной почте. Извлечения **технических контактных** данных, чтобы связаться с клиентом, чтобы они могли быть осведомлены об амортизации.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/tenantTechnicalContact.png" alt-text="Найдите технический контакт клиента." border="true":::

## <a name="i-know-apps-that-are-using-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph"></a>Я знаю приложения, использующие azure AD Graph. Как перенести их в Microsoft Graph?

Чтобы перенести приложения из Azure AD Graph в Microsoft Graph, выполните контрольный список планирования [миграции приложений.](migrate-azure-ad-graph-planning-checklist.md)

## <a name="i-dont-own-some-apps-in-my-tenant-but-they-use-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph-api-can-i-find-the-owner-of-such-apps"></a>У меня нет некоторых приложений в клиенте, но они используют Azure AD Graph. Как перенести их в API Graph Майкрософт? Могу ли я найти владельца таких приложений?

Сначала подтвердите полный список приложений, которые принадлежат вашему клиенту или сторонним приложениям, интегрированным в клиента.

1. Во входе на [портал Azure в](https://portal.azure.com) качестве администратора.
1. Поиск и выбор **Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В окне регистраций приложений выберите вкладку **Все приложения.**
1. Выберите приложение. Это показывает меню приложения.
1. В левом окне параметры меню раскрывают сведения о приложении, в том числе о его владельцах.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppOwners.png" alt-text="Найдите владельцев приложений." border="true":::


## <a name="can-i-request-for-an-exception-if-im-unable-to-meet-the-june-30-2022-migration-deadline"></a>Могу ли я запросить исключение, если не удается выполнить крайний срок миграции 30 июня 2022 г.?  

Исключения из этого амортизации не существуют. После 30 июня 2022 г. ваши приложения больше не будут получать ответы из Graph Azure AD. 

## <a name="i-need-to-create-new-apps-to-use-azure-ad-graph-but-the-azure-ad-graph-api-permission-sign-up-is-closed-how-can-i-create-my-app"></a>Мне нужно создать новые приложения для использования Azure AD Graph но регистрацию разрешения Graph API Azure API закрывается. Как создать приложение?

Во-первых, рекомендуется следовать [](migrate-azure-ad-graph-planning-checklist.md) контрольным списком планирования миграции приложений, чтобы помочь вам перейти к API Graph Microsoft. 

Если вы определили пробел, в котором microsoft Graph не поддерживает функцию, поддерживаемую Azure AD Graph, поработать с администратором клиента или владельцем подписки, чтобы сообщить о разрыве. Если мы убедитесь, что это действительно пробел, который Graph API Microsoft не выполняет, мы поможем вам создать приложение. Однако это не означает исключение из амортизации. Приложение с помощью Azure AD Graph будет по-прежнему работать после 30 июня 2022 г.


## <a name="see-also"></a>См. также

+ [Контрольный список для переноса приложений](migrate-azure-ad-graph-request-differences.md)
