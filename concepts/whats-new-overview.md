---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ef374f0718ed5c8df6cd7261ccce15d1b0cdab9e
ms.sourcegitcommit: e7e5c40a616a88d21116f60b394422cf2a9077c3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48463754"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](changelog.md). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="october-2020-new-in-preview-only"></a>Октябрь 2020 г.: новые возможности только в предварительной версии

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Управляйте [политиками метода проверки подлинности](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true), чтобы определять пользователей, которые могут использовать конкретные методы многофакторной проверки подлинности для входа в Azure Active Directory. Настройте политики, чтобы определить следующее:
  - Типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.
  - Пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход без пароля с помощью телефона для входа в Azure AD.
- Настройте [метод проверки подлинности электронной почты](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true), чтобы пользователи самостоятельно сбрасывали пароли.
- Используйте [Azure AD B2C](/azure/active-directory-b2c/overview) и [выберите механизм настройки и проверки подлинности пользователей с помощью локальных учетных записей](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true).
- Используйте `Policy.ReadWrite.AuthenticationMethod` для чтения и записи политик метода проверки подлинности в организации в виде делегированного разрешения от имени вошедшего пользователя или разрешения приложения без необходимости входа пользователя.
- Укажите в [политике авторизации](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true), можно ли приглашать внешних пользователей в организацию и кому это разрешено.

## <a name="september-2020-new-and-generally-available"></a>Сентябрь 2020г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
Общая доступность необязательного свойства **transactionId** ресурса [event](/graph/api/resources/event), которое настраивается клиентским приложением, чтобы избежать лишних операций POST, если клиент повторно пытается создать то же событие. Это полезно в тех случаях, когда из-за плохого сетевого подключения клиент отключается, не успев получить от сервера ответ на предыдущий запрос клиента на создание события.

### <a name="cloud-communications"></a>Облачные коммуникации
[Удаление участника](/graph/api/participant-delete) из [звонка](/graph/api/resources/call). Вы можете использовать эту операцию даже в тех случаях, когда нужно удалить участника из активного звонка.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [сентябрь](changelog.md#september-2020) для версии 1.0.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Общая доступность [API административных единиц](/graph/api/resources/administrativeunit), позволяющих организациям делить Azure Active Directory на подразделения, а также управлять административными обязанностями и делегировать их этим подразделениям. Эти подразделения могут представлять регионы, отделы, места возникновения затрат и т. д.

### <a name="reports"></a>Отчеты
[Получите отчет, включающий количество уникальных пользователей](/graph/api/reportroot-getemailappusageversionsusercounts) для Outlook 2019 и Outlook в Microsoft 365.

### <a name="teamwork"></a>Командная работа
- Получите свойство **lastEditedDateTime**, чтобы узнать, когда отправитель последний раз внес изменения в [сообщение чата](/graph/api/resources/chatmessage).
- Получите свойство **lastModifiedDateTime**, чтобы узнать, когда отправитель создал сообщение чата или когда любой пользователь изменил его другими способами, в том числе добавив или удалив реакции. 
- [Получайте уведомления об изменениях](webhooks.md) в [сообщениях чата](/graph/api/resources/chatmessage).
- [Обновите](/graph/api/chatmessage-update?view=graph-rest-beta&preserve-view=true) свойство **policyViolation** объекта [chatMessage](/graph/api/resources/chatmessagepreserve-view=true) в [канале](/graph/api/resources/channel&preserve-view=true) или [чате](/graph/api/resources/chat&preserve-view=true), позволив приложениям защиты от потери данных (DLP) отслеживать [нарушения политики сообщений чатов](/graph/api/resources/chatmessagepolicyviolation?preserve-view=true), чтобы сообщения не содержали данные, которые пользователи не должны отправлять.

### <a name="use-the-sdks"></a>Использование пакетов SDK
Общая доступность пакета [SDK PowerShell Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-powershell), обеспечивающего понятный и согласованный доступ ко всем возможностям Microsoft Graph.

### <a name="use-the-toolkit"></a>Использование набора средств
Воспользуйтесь новыми пошаговыми руководствами по началу работы для набора средств Microsoft Graph и насладитесь удобством набора средств:
- [Создание веб-приложения в JavaScript](./toolkit/get-started/build-a-web-app.md)
- [Создание веб-части SharePoint](./toolkit/get-started/build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./toolkit/get-started/build-a-microsoft-teams-tab.md)
- [Использование набора средств с помощью React](./toolkit/get-started/use-toolkit-with-react.md)
- [Использование набора средств с помощью Angular](./toolkit/get-started/use-toolkit-with-angular.md)

### <a name="users"></a>Пользователи
Помимо получения SMTP-адреса [пользователя](/graph/api/resources/user) с помощью свойства **mail**, теперь вы можете установить это свойство и обновить адрес электронной почты пользователя. 

## <a name="september-2020-new-in-preview-only"></a>Сентябрь 2020г.: новые возможности только в предварительной версии

### <a name="application"></a>Для приложений
Создание, перечисление и удаление [классификаций делегированных разрешений](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true), применяемых [субъектом-службой](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true). Используйте классификации делегированных разрешений в сочетании с [параметрами согласия пользователей](/azure/active-directory/manage-apps/configure-user-consent), чтобы устанавливать ограничения на то, когда пользователям разрешено предоставлять согласие приложениям.

### <a name="cloud-communications"></a>Облачные коммуникации
- Не рекомендуется использовать свойства**autoAdmittedUsers** из[onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Вместо этого следует использовать новое свойство **lobbyBypassSettings** и его [значения](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
- Используйте дополнительные параметры, связанные для объявления звонящим о присоединении или выходе из собрания по сети (свойство **isEntryExitAnnounced**), и разрешения конкретных выступающих доступа к собранию (свойство **allowedPresenters**).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- [Получите документы для каждого задания печати, связанного с принтером](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true), применив `$expand` [параметр запроса системы OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters). 
- Отфильтруйте задания печати по пользователю, который их создал, применив `$filter` [параметр системного запроса OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [сентябрь](changelog.md#september-2020) для бета-версии.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- [Получите ключ восстановления BitLocker](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true) от имени вошедшего пользователя, который является владельцем устройства или выполняет соответствующую роль. При получении ключа восстановления создается [журнал аудита](/azure/active-directory/reports-monitoring/concept-audit-logs) наравне с пользовательским интерфейсом.
- Получите общее и использованное значение [квоты каталога](/graph/api/resources/directorysizequota?view=graph-rest-beta&preserve-view=true) в [организации](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) с помощью свойства **directorySizeQuota**.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Вы можете включить [расписание](/graph/api/resources/requestschedule?view=graph-rest-beta&preserve-view=true) при запросе или удалении [назначения пользователя на пакет доступа](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true), который определяет доступ к группам, приложениям или сайтам SharePoint.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Организации могут [получить](/graph/api/continuousaccessevaluationpolicy-get?view=graph-rest-beta&preserve-view=true) или [обновить](/graph/api/continuousaccessevaluationpolicy-update?view=graph-rest-beta&preserve-view=true) [политику оценки непрерывного доступа](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true), чтобы управлять сеансами проверки подлинности в режиме реального времени.

### <a name="search"></a>Поиск

- Используйте дополнительные возможности в [API Поиска (Майкрософт)](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) для соединителей OneDrive, SharePoint, Microsoft Graph: 

  - Получайте [дополнительные типы](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types) содержимого из OneDrive и SharePoint: **drive**, **list**, **listItem** и **site**. 
  - Объединяйте свойства в области в результатах поиска для [выбранных свойств](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#get-selected-properties). 
  - Получайте настраиваемые свойства в ресурсах [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true).
  - [Сортируйте](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#sort-search-results) результаты поиска для OneDrive и SharePoint с помощью любого свойства, поддерживающего сортировку.
  - [Уточняйте результаты с помощью агрегатов](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#refine-results-using-aggregations) для OneDrive и SharePoint.
- Запрашивайте внешние данные, принятые соединителями Microsoft Graph, в [нескольких связях](./search-concept-custom-types.md).
- Воспользуйтесь улучшенным содержимым для соединителей Microsoft Graph, чтобы узнать о следующем:
  - [Управление связями](search-index-manage-connections.md)
  - [Управление схемой](search-index-manage-schema.md)
  - [Управление элементами](search-index-manage-items.md)
- Отслеживайте состояние [подключения](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) Microsoft Graph.
- Определите [внешнюю группу](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true), чтобы задать разрешения для объектов [внешних элементов](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true), добавленных в [подключение](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) Microsoft Graph. Внешние группы могут представлять группы, не относящиеся к Azure Active Directory, или похожие на группы конструкции, например бизнес-подразделения, которые устанавливают разрешения для содержимого во внешнем источнике данных.

### <a name="teamwork"></a>Командная работа
- Узнайте о дате и времени создания [канала](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) или [команды](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) Teams.


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
