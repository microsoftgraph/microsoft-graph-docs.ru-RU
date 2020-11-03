---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 9da26e00f398ec29ce138a598d9bc7d1faba8bbf
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849125"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](changelog.md). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_ , в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="october-2020-new-and-generally-available"></a>Октябрь 2020 г.: новые и общедоступные возможности

### <a name="application"></a>Приложение
- Разрешите [адрес электронной почты в качестве альтернативного имени для входа в Azure AD](/azure/active-directory/authentication/howto-authentication-use-email-signin) с помощью политики [обнаружения домашней области](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery). Политика обнаружения домашней области определяет, требовать ли от пользователя проверки подлинности после предоставления пользователем имени для входа. В этом случае настройка свойства **AlternateIdLogin** ресурса [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) может разрешить пользователю входить с помощью адреса электронной почты.
- Получайте сведения о проверенном издателе для объектов [application](/graph/api/resources/application) или [servicePrincipal](/graph/api/resources/serviceprincipal) и [настройте](/graph/api/application-setverifiedpublisher) или [удалите](/graph/api/application-unsetverifiedpublisher) сведения о проверенном издателе для объекта **application**.

### <a name="change-notifications"></a>Уведомления об изменениях
Приложения рабочей среды теперь могут подписываться на уведомления жизненного цикла элементов Outlook [message](/graph/api/resources/message), [event](/graph/api/resources/event) и [contact](/graph/api/resources/contact), а также элемента Teams [chatMessage](/graph/api/resources/chatmessage), чтобы [сократить количество пропущенных уведомлений о подписках и изменениях](webhooks-lifecycle.md).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Общая доступность расширенных параметров системных запросов OData (`$count`, `$search` и `$filter`) для объектов каталогов.
- Ознакомьтесь с примерами, демонстрирующими преобразование OData для объектов каталога.
- Списки расширенных API см. в разделе удостоверения и доступа в обновлениях за [октябрь](changelog.md#october-2020) журнала изменений.

### <a name="teamwork"></a>Командная работа
- Общая доступность полного набора операций CRUD для ресурса [conversationMember](/graph/api/resources/conversationmember) и [aadUserConversationMember](/graph/api/resources/aaduserconversationmember). Эти ресурсы представляют участника чата или беседы канала, который может быть или не быть пользователем в Azure AD.
- Общая доступность уведомлений жизненного цикла для ресурсов [chatMessage](/graph/api/resources/chatmessage) в Teams для [сокращения количества пропущенных уведомлений о подписках и изменениях](webhooks-lifecycle.md).

### <a name="to-do-tasks"></a>Задачи To-Do
Общая доступность [API Microsoft To Do](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true) — используйте API To-Do в приложении рабочей среды для создания задач и управления ими в рамках рабочего процесса пользователя, например при создании задачи из письма.  

### <a name="users"></a>Пользователи
Получайте новые свойства, относящиеся к [пользователю](/graph/api/resources/user), который является корпоративным сотрудником: дата найма, связь с организацией, например отдел и место возникновения затрат, и тип сотрудника, например консультант, подрядчик или поставщик. Для этих свойств требуется указать параметр запроса OData `$select` в операции GET.

## <a name="october-2020-new-in-preview-only"></a>Октябрь 2020 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Собрание по сети
- Определите роль участника в [собрании по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) в качестве участника или выступающего, используя свойство **role** типа [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo?view=graph-rest-beta&preserve-view=true).
- Получайте объект [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) путем [фильтрации по свойству joinWebUrl собрания](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-3-retrieve-an-online-meeting-by-joinweburl).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать

- Прекращение поддержки действия **uploadData** , вместо которого применяется [создание сеанса отправки](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) для [отправки документа](upload-data-to-upload-session.md) на принтер или общий принтер.
- Прекращение поддержки свойства **printDocument** в [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true), вместо которого применяется аналогичное свойство **configuration** в [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Получайте URL-адрес исходного или конечного задания для перенаправляемого объекта **printJob** , используя свойство **redirectedFrom** или **redirectedTo**.
- Получайте текущее состояние **printJob** , используя свойство **state** и новое свойство **details**.
- Получайте коллекцию общих принтеров, связанных с объектом [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), используя связь **shares**. 
- Прекращение поддержки свойства **processingStateReasons** объекта **printer** , вместо которого применяется свойство **status**. Свойство **status** относится к типу [printer status](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) и представляет свойство **details**. Используйте свойство **details** для определения причины текущего состояния принтера.
- Прекращение поддержки свойства **feedDirections** в [printerCapabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true), вместо которого применяется свойство **feedOrientations** для получения ориентации подачи лотка, поддерживаемой принтером.
- Сведения о нескольких переименованиях API и свойств, а также о прекращении поддержки нескольких элементов см. в разделе облачной печати в обновлениях за [октябрь](changelog.md#october-2020) журнала изменений.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [октябрь](changelog.md#october-2020) для бета-версии.

### <a name="files"></a>Файлы
[Отменяйте](/graph/api/permission-revokegrants?view=graph-rest-beta&preserve-view=true) доступ к элементу [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) или [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true), предоставленный с помощью ссылки для общего доступа.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Управляйте [политиками метода проверки подлинности](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true), чтобы определять пользователей, которые могут использовать конкретные методы многофакторной проверки подлинности для входа в Azure Active Directory. Настройте политики, чтобы определить следующее:
  - Типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.
  - Пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход без пароля с помощью телефона для входа в Azure AD.
- Настройте [метод проверки подлинности электронной почты](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true), чтобы пользователи самостоятельно сбрасывали пароли.
- Используйте [Azure AD B2C](/azure/active-directory-b2c/overview) и [выберите механизм настройки и проверки подлинности пользователей с помощью локальных учетных записей](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true).
- Используйте `Policy.ReadWrite.AuthenticationMethod` для чтения и записи политик метода проверки подлинности в организации в виде делегированного разрешения от имени вошедшего пользователя или разрешения приложения без необходимости входа пользователя.
- Укажите в [политике авторизации](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true), можно ли приглашать внешних пользователей в организацию и кому это разрешено.

### <a name="people-and-workplace-intelligence--insights"></a>Люди и рабочая аналитика | Аналитика 
Администраторы могут просмотреть [примеры использования командлетов PowerShell](insights-customize-item-insights-privacy.md#how-to-configure-item-insights-setting-via-powershell), чтобы настроить параметры аналитики элементов для организации.

### <a name="teamwork"></a>Командная работа
- Используйте атрибут **channelCreationMode** экземпляра, чтобы указать, что создается [канал](https://docs.microsoft.com/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true#instance-attributes) для обслуживания миграции данных. Используйте атрибут [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true), чтобы указать на завершение миграции и возможность публикации и чтения сообщений участниками.
- Используйте атрибут **teamCreationMode** экземпляра, чтобы указать, что создается [команда](https://docs.microsoft.com/graph/api/resources/team?view=graph-rest-beta&preserve-view=true#instance-attributes) для обслуживания миграции. Используйте атрибут [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true), чтобы указать на завершение миграции и возможность выполнения операций участников и публикации сообщений участниками.


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
- Получите свойство **lastEditedDateTime** , чтобы узнать, когда отправитель последний раз внес изменения в [сообщение чата](/graph/api/resources/chatmessage).
- Получите свойство **lastModifiedDateTime** , чтобы узнать, когда отправитель создал сообщение чата или когда любой пользователь изменил его другими способами, в том числе добавив или удалив реакции. 
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
Помимо получения SMTP-адреса [пользователя](/graph/api/resources/user) с помощью свойства **mail** , теперь вы можете установить это свойство и обновить адрес электронной почты пользователя. 

## <a name="september-2020-new-in-preview-only"></a>Сентябрь 2020г.: новые возможности только в предварительной версии

### <a name="application"></a>Для приложений
Создание, перечисление и удаление [классификаций делегированных разрешений](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true), применяемых [субъектом-службой](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true). Используйте классификации делегированных разрешений в сочетании с [параметрами согласия пользователей](/azure/active-directory/manage-apps/configure-user-consent), чтобы устанавливать ограничения на то, когда пользователям разрешено предоставлять согласие приложениям.

### <a name="cloud-communications"></a>Облачные коммуникации
- Не рекомендуется использовать свойства **autoAdmittedUsers** из [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Вместо этого следует использовать новое свойство **lobbyBypassSettings** и его [значения](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
- Используйте дополнительные параметры, связанные для объявления звонящим о присоединении или выходе из собрания по сети (свойство **isEntryExitAnnounced** ), и разрешения конкретных выступающих доступа к собранию (свойство **allowedPresenters** ).

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

  - Получайте [дополнительные типы](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types) содержимого из OneDrive и SharePoint: **drive** , **list** , **listItem** и **site**. 
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

    2. Повышение до **_общедоступного_ состояния (GA)** , если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
