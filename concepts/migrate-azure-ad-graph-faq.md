---
title: Azure AD Graph часто задаваемые вопросы о миграции Graph Microsoft
description: Ответы на часто задаваемые вопросы о переходе с Azure Active Directory (Azure AD) Graph на microsoft Graph.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 0605dfc2eb38f6339fe27f167599a211d1c80208
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247072"
---
# <a name="azure-ad-graph-to-microsoft-graph-migration-faq"></a>Azure AD Graph часто задаваемые вопросы о миграции Graph Microsoft

В этой статье содержатся ответы на часто задаваемые вопросы о миграции Azure Active Directory (Azure AD) Graph [в Microsoft Graph](/graph/overview).

## <a name="how-is-microsoft-graph-different-from-azure-ad-graph-and-why-should-i-migrate-my-apps"></a>Чем Microsoft Graph отличается от Azure AD Graph и почему следует переносить мои приложения?

Этот Azure AD API Graph предоставляет доступ только к Azure AD служб. Microsoft API Graph предоставляет единую конечную точку для доступа к службам Azure AD и другим службы Майкрософт, таким как Microsoft Teams, Microsoft Exchange и Microsoft Intune.

[Microsoft Graph](/graph/overview) также является более безопасным и устойчивым, чем Azure AD Graph. По этой причине Azure AD Graph был выведен из эксплуатации с 30 июня 2020 г. и будет прекращен в ближайшем будущем по мере переноса всех инвестиций в Microsoft Graph. После прекращения поддержки ваши приложения будут получать сообщения об ошибках от Azure AD Graph конечной точки. Перейдите на microsoft Graph, чтобы избежать потери функциональности.

## <a name="as-a-developer-how-do-i-identify-apps-that-use-azure-ad-graph"></a>Как разработчик может определить приложения, использующие Azure AD Graph?

Выполните следующие действия, чтобы определить приложения с зависимостью от Azure AD Graph.

### <a name="step-1-scan-the-application-source-code"></a>Шаг 1. Сканирование исходного кода приложения

Если вы владеете исходным кодом приложения, `https://graph.windows.net/` найдите URI в коде. Это конечная Azure AD Graph и приложения, вызывающие эту конечную точку, используют Azure AD Graph. Запишите значение идентификатора приложения затронутого приложения.

### <a name="step-2-check-the-apps-api-permissions-on-the-azure-portal"></a>Шаг 2. Проверка разрешений API приложения на портал Azure

1. Войдите [в портал Azure в](https://portal.azure.com) качестве глобального администратора.
1. Найдите **и выберите Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В **окне Регистрация приложений** включите **предварительный Регистрация приложений поиска**. Перейдите **на вкладку "Все приложения** ", а затем выберите **параметр "Добавить фильтры** ". Выберите параметр **идентификатора приложения (клиента)** из списка доступных фильтров и нажмите кнопку " **Применить"**.  Отобразит фильтр.
1. В текстовом поле введите идентификатор приложения, полученный на шаге 1, и нажмите кнопку " **Применить"**. Список сужается до указанного приложения.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="Фильтрация по приложениям по идентификатору приложения." border="true":::

1. Выберите приложение. Откроется меню приложения.
1. В левой области окна выберите разрешения **API**. Это позволяет отобразить настроенные разрешения API для вашего приложения, включая Azure AD Graph разрешений.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/configuredPermissions.png" alt-text="Список разрешений API приложения из портал Azure." border="true":::


## <a name="as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph"></a>Как ИТ-администратору определить приложения в клиенте, которые используют Azure AD Graph?

Используйте один из следующих трех методов для идентификации приложений в клиенте с зависимостью от Azure AD Graph.

### <a name="method-1-through-network-proxy-logs"></a>Метод 1. С помощью журналов прокси-сервера сети

Проверьте журналы трафика сетевого сервера через прокси-сервер фильтра для всех приложений, вызывающих конечную `https://graph.windows.net/` точку. Эти приложения используют Azure AD Graph.

### <a name="method-2-use-the-app-registrations-menu-of-the-azure-portal"></a>Метод 2. Используйте Регистрация приложений меню портал Azure

1. Войдите [в портал Azure в](https://portal.azure.com) качестве глобального администратора.
1. Найдите **и выберите Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В **окне Регистрация приложений** включите **предварительный Регистрация приложений поиска**. Перейдите **на вкладку "Все приложения** ", а затем выберите **параметр "Добавить фильтры** ". Выберите параметр **"Запрашиваемый API** " из списка доступных фильтров и нажмите кнопку " **Применить"**. **Отобразит фильтр запрашиваемого API**.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI.png" alt-text="Фильтрация приложений по запрошенным API." border="true":::

5. Выберите **API Майкрософт**. Выберите **раскрывающийся список API** **и выберите Azure Active Directory Graph**. Нажмите **Применить**. Здесь перечислены все приложения с зависимостью от Azure AD Graph.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI-AAD.png" alt-text="Фильтрация приложений, использующих Azure AD Graph." border="true":::

### <a name="method-3-use-a-powershell-script"></a>Метод 3. Использование скрипта PowerShell

Скачайте и [запустите этот сценарий PowerShell](https://github.com/microsoft/AzureADGraphApps). Используйте этот метод для получения приложений с домашним каталогом в клиенте и приложений с их домашними каталогами в других клиентах.


## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-how-do-i-find-the-details-of-each-app-including-its-owner"></a>Корпорация Майкрософт отправила мне сообщение электронной почты со списком идентификаторов приложений, использующих Azure AD Graph. Разделы справки найти сведения о каждом приложении, включая его владельца?

1. Войдите [в портал Azure в](https://portal.azure.com) качестве глобального администратора.
1. Найдите **и выберите Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В **окне Регистрация приложений** включите **предварительный Регистрация приложений поиска**. Перейдите **на вкладку "Все приложения** ", а затем выберите **параметр "Добавить фильтры** ". Выберите параметр **идентификатора приложения (клиента)** из списка доступных фильтров и нажмите кнопку " **Применить"**.  Отобразит фильтр.
1. Введите идентификатор приложения в текстовом поле и нажмите кнопку " **Применить"**. Список сужается до указанного приложения.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="Фильтрация по приложениям по идентификатору приложения." border="true":::

6. Выберите приложение. Откроется меню приложения. В левой области окна параметры меню, такие как "Владельцы", позволяют получить сведения о приложении.

## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-are-these-all-the-affected-apps"></a>Корпорация Майкрософт отправила мне сообщение электронной почты со списком идентификаторов приложений, использующих Azure AD Graph. Это все затронутые приложения?

В этом списке фиксируются только приложения, используемые в течение последних 28 дней и вызываемые Azure AD Graph конечной точкой. Так как некоторые приложения могут использовать сезонное использование, их идентификатор может быть записан в списке за один месяц, но не в другом. Чтобы получить полный список затронутых приложений, рекомендуется следовать одному [из трех](#as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph) указанных выше методов.

## <a name="im-a-subscription-owner-and-microsoft-sent-me-an-email-about-azure-ad-graph-deprecation-with-a-list-of-app-ids-what-should-i-do"></a>Я владелец подписки, и корпорация Майкрософт отправила мне сообщение Azure AD Graph о прекращении поддержки со списком идентификаторов приложений. Что мне делать?

Получаемые сообщения электронной почты содержат идентификаторы клиентов, связанные с идентификаторами приложений. Выполните следующие действия, чтобы получить технические контактные данные для конкретных клиентов.
1. Войдите [в портал Azure с](https://portal.azure.com) правами администратора.
1. Если вы являетесь владельцем подписки в нескольких Azure AD клиентах, сначала переключитесь на соответствующий клиент или каталог.
    1. В правом верхнем углу окна щелкните значок профиля и выберите " **Переключить каталог"**. Откроется список **параметров портала | Окно каталогов и подписок** . 
    1. В списке используйте вкладку **"** Переключить", чтобы перейти в каталог, идентификатор каталога которого соответствует идентификатору клиента, полученному в сообщении электронной почты. Active Directory помечен как **"Текущий"**.
    1. Закройте окно.
1. В соответствующем каталоге найдите и **выберите Azure Active Directory.** Откроется меню для активного клиента. 
1. В левой области окна в **разделе "Управление**" выберите **"Свойства"**.
1. В **окне свойств клиента** сначала убедитесь, что значение идентификатора клиента соответствует идентификатору клиента, полученному в сообщении электронной почты. Получите сведения **о техническом** контакте для связи с клиентом, чтобы он знал об устаревании.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/tenantTechnicalContact.png" alt-text="Поиск технического контакта клиента." border="true":::

## <a name="i-know-apps-that-are-using-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph"></a>Я знаю приложения, использующие Azure AD Graph. Разделы справки перенести их в Microsoft Graph?

Чтобы перенести приложения из Azure AD Graph в Microsoft Graph, следуйте контрольным спискам планирования [миграции приложений](migrate-azure-ad-graph-planning-checklist.md).

## <a name="i-dont-own-some-apps-in-my-tenant-but-they-use-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph-api-can-i-find-the-owner-of-such-apps"></a>У меня нет приложений в моем клиенте, но они используют Azure AD Graph. Разделы справки перенести их в Microsoft API Graph? Можно ли найти владельца таких приложений?

Сначала подтвердите полный список приложений, принадлежащих вашему клиенту или сторонним приложениям, интегрированным в клиент.

1. Войдите [в портал Azure с](https://portal.azure.com) правами администратора.
1. Найдите **и выберите Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В окне Регистрация приложений выберите вкладку **"Все приложения**".
1. Выберите приложение. Откроется меню приложения.
1. В левой области окна параметры меню показывают сведения о приложении, включая его владельцев.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppOwners.png" alt-text="Найдите владельцев приложений." border="true":::


## <a name="my-organization-runs-azure-stack-hub-what-actions-should-i-take"></a>В моей организации работает Azure Stack Hub. Какие действия следует выполнить?

Если в вашей организации используется Azure Stack Hub, самое важное действие — следовать политике обслуживания [Azure Stack Hub](/azure-stack/operator/azure-stack-servicing-policy).

Чтобы выполнить миграцию, клиенты будут получать уведомления на портале администрирования Azure Stack Hub для обновления каталогов домашних и гостевых клиентов. Миграцией в Microsoft Graph будет управлять интегрированная среда обновления системы.

## <a name="i-need-to-add-new-azure-ad-graph-permissions-to-my-app-but-i-cant-select-azure-ad-graph-as-a-required-permission-for-my-app-registration-how-can-i-add-the-azure-ad-graph-permissions"></a>Мне нужно добавить новые разрешения Azure AD Graph приложения, но я не могу выбрать Azure AD Graph в качестве необходимого разрешения для регистрации приложения. Как добавить разрешения Azure AD Graph разрешений?

Во-первых, рекомендуется выполнить контрольный [](migrate-azure-ad-graph-planning-checklist.md) список планирования миграции приложений, чтобы помочь вам перевести приложения в microsoft API Graph.

Если вы обнаружили разрыв, в котором Microsoft Graph не поддерживает функцию, доступную в Azure AD Graph, сообщите нам об этом с помощью Microsoft Q&A с помощью тега [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html).

Если вам по-прежнему Azure AD Graph разрешения для приложений, используйте одно из следующих обходных решений.

+ Используйте портал Azure, чтобы найти API, которые использует ваша организация
+ Обновление манифеста приложения на портал Azure
+ Использование API [приложения](/graph/api/resources/application) в Microsoft Graph для обновления [объекта requiredResourceAccess](/graph/api/resources/requiredresourceaccess)
+ Использование [командлета Update-MgApplicationcmdlet](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)  в microsoft Graph PowerShell

Примеры использования перечисленных обходных решений см. в статье "Использование Microsoft Graph для настройки необходимых разрешений Azure AD Graph для [регистрации приложения"](migrate-azure-ad-graph-configure-permissions.md).

>**Примечание:** Добавление Azure AD Graph разрешений с помощью этих обходных решений не будет поддерживаться после прекращения использования Azure AD Graph. Все приложения, использующие Azure AD Graph, по-прежнему перестанут работать после прекращения поддержки.



## <a name="see-also"></a>См. также

+ [Контрольный список для переноса приложений](migrate-azure-ad-graph-request-differences.md)
