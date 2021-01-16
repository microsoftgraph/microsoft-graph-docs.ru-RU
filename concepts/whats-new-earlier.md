---
title: Обзор предыдущих выпусков Microsoft Graph
description: Новые возможности в предыдущих выпусках Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 0414c2414a6765c7e0c29114c2239d15bbe71cea
ms.sourcegitcommit: 8f156a80b2f76cefa271a536c238721aff6931bf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883419"
---
# <a name="highlights-of-earlier-releases"></a>Обзор предыдущих выпусков

## <a name="november-2020-new-and-generally-available"></a>Ноябрь 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачная коммуникация
- Общая доступность свойства **роль** типа [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo), разделяющего участников [виртуального собрания](/graph/api/resources/onlinemeeting) на участников и докладчиков.
- Общая доступность свойства **lobbyBypassSettings** и его [значений](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) для допуска пользователей к виртуальному собранию.
- Общая доступность свойства **isEntryExitAnnounced** для настройки параметров объявления пользователей, присоединяющихся к виртуальному собранию или покидающих его.
- Общая доступность свойства **allowedPresenters** для разрешения отдельным пользователям выступать на собрании.

### <a name="search"></a>Поиск
- Общая доступность [API запросов](/graph/api/resources/search-api-overview) Поиска (Майкрософт), поддерживающих поиск данных следующих типов:
  - [Сообщения Outlook](./search-concept-messages.md)
  - [События календаря Outlook](./search-concept-events.md)
  - [Ресурсы OneDrive и SharePoint](./search-concept-files.md).

### <a name="teamwork"></a>Командная работа

- Общая доступность разрешений с согласием для конкретных ресурсов (RSC). Разрешения RSC позволяют владельцам команд предоставлять детальные разрешения рабочим приложениям на доступ и/или изменение конкретных данных команды, например на чтение параметров команды или изменение названий каналов, описаний и других параметров.
- Общая доступность API, применяемых к [каналу](/graph/api/resources/channel) или сообщениям в канале. API включают:
  - [Создание](/graph/api/conversationmember-add) или [удаление](/graph/api/conversationmember-delete) участника беседы из канала.
  - [Обновление роли участника](/graph/api/conversationmember-update) в канале.
  - Получение конкретного сообщения или всех сообщений в канале.
  - Получение конкретного ответа или всех ответов в канале.
  - [Отслеживание новых или обновленных сообщений в канале](/graph/api/chatmessage-delta).


## <a name="november-2020-new-in-preview-only"></a>Ноябрь 2020 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
Дебют [API облачного ПК](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true), позволяющего организациям выполнять подготовку виртуальных компьютеров для сотрудников и управлять этими компьютерами. Используйте его в сочетании с API Intune для управления физическими и виртуальными конечными точками.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
[Подписка на уведомления об изменениях](webhooks.md) в [определении задачи печати](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [ноябрь](changelog.md#november-2020) для бета-версии.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Указание URL-адресов для отправки маркеров входа пользователей и URI для кодов авторизации и маркеров доступа в свойстве **spa** [приложения](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true).
- Настройка внешнего вида и удобства использования экранов входа в Azure Active Directory посредством [свойств бренда организации](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). Организации могут выполнять настройку на основе региональных параметров для отдельных пользователей.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Дебютное представление интерфейса [API проверки доступа в целях предоставления членства в группе](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) для регулярной проверки доступа пользователей. Интерфейс позволяет обеспечивать постоянный доступ только нужным пользователям и эффективно управлять членством в группе.

### <a name="search"></a>Поиск
Вы можете объединять числовые или строковые результаты поиска, импортированные [соединителями Microsoft Graph](/microsoftsearch/connectors-overview), которые настроены в качестве уточняемых в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Ознакомьтесь с дополнительными сведениями об [уточнении результатов поиска с помощью агрегирования](search-concept-aggregation.md).

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

- Прекращение поддержки действия **uploadData**, вместо которого применяется [создание сеанса отправки](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) для [отправки документа](upload-data-to-upload-session.md) на принтер или общий принтер.
- Прекращение поддержки свойства **printDocument** в [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true), вместо которого применяется аналогичное свойство **configuration** в [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Получайте URL-адрес исходного или конечного задания для перенаправляемого объекта **printJob**, используя свойство **redirectedFrom** или **redirectedTo**.
- Получайте текущее состояние **printJob**, используя свойство **state** и новое свойство **details**.
- Получайте коллекцию общих принтеров, связанных с объектом [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), используя связь **shares**. 
- Прекращение поддержки свойства **processingStateReasons** объекта **printer**, вместо которого применяется свойство **status**. Свойство **status** относится к типу [printer status](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) и представляет свойство **details**. Используйте свойство **details** для определения причины текущего состояния принтера.
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
- Используйте атрибут **channelCreationMode** экземпляра, чтобы указать, что создается [канал](/graph/api/resources/channel?preserve-view=true&view=graph-rest-beta#instance-attributes) для обслуживания миграции данных. Используйте атрибут [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true), чтобы указать на завершение миграции и возможность публикации и чтения сообщений участниками.
- Используйте атрибут **teamCreationMode** экземпляра, чтобы указать, что создается [команда](/graph/api/resources/team?preserve-view=true&view=graph-rest-beta#instance-attributes) для обслуживания миграции. Используйте атрибут [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true), чтобы указать на завершение миграции и возможность выполнения операций участников и публикации сообщений участниками.

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
- Не рекомендуется использовать свойства **autoAdmittedUsers** из [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Вместо этого следует использовать новое свойство **lobbyBypassSettings** и его [значения](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
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


## <a name="august-2020-new-and-generally-available"></a>Август 2020 г.: новые и общедоступные возможности

### <a name="change-notifications"></a>Уведомления об изменениях
[Отслеживание изменений](delta-query-overview.md) поддерживаемых ресурсов в национальном облаке Microsoft Graph для государственных организаций США.

### <a name="cloud-communications"></a>Коммуникации из облака
- [Отмените](/graph/api/call-cancelmediaprocessing) любые действия интерактивного голосового ответа (IVR), выполняемые или находящиеся в очереди, которые [воспроизводят звуковой сигнал](/graph/api/call-playprompt) или [записывают ответ](/graph/api/call-record).
- Получите [сведения о расшифровке звонка](/graph/api/resources/calltranscriptioninfo) с помощью свойства **transcription**.

### <a name="teamwork"></a>Командная работа
- Используйте альтернативный способ [создания группы](/graph/api/team-post) без предварительного создания группы.
- Используйте свойство навигации **участники**, чтобы добавить участников в команду с большей надежностью и меньшей задержкой.
- Узнайте, в каком состоянии находится публикация [приложения](/graph/api/resources/teamsapp) Microsoft Teams с помощью свойства **publishingState** [определения приложения](/graph/api/resources/teamsappdefinition). Возможные значения состояния публикации: `submitted`, `published` и `rejected`. См. [пример](/graph/api/teamsapp-list?view=graph-rest-beta&preserve-view=true#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state).
- Воспользуйтесь делегированным разрешением `AppCatalog.Submit`, чтобы позволить пользователю [отправить приложение](/graph/api/teamsapp-publish) и оформить запрос на его проверку администратором. С помощью этого же разрешения пользователь может [отменить](/graph/api/teamsapp-delete) отправленное ранее приложение, которое не было опубликовано. 


## <a name="august-2020-new-in-preview-only"></a>Август 2020 г.: новые возможности только в предварительной версии

### <a name="applications"></a>Приложения
Поддержка единого входа на основе паролей в ресурсах приложения [субъекта-службы](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) и указание таких [параметров](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta&preserve-view=true) в свойстве **passwordSingleSignOnSettings**. Сведения о едином входе на основе паролей в Azure AD см. в статье [Настройка единого входа на основе пароля](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).

### <a name="calendar"></a>Календарь
Улучшенная программная поддержка сценариев, в которых используется повторяющееся [событие](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true):
- надежный поиск экземпляра события в повторяющемся ряду, в том числе измененного или отмененного, с помощью свойства **occurrenceId**;
- поиск любых исключений в ряду повторяющихся экземпляров события с помощью свойства **exceptionOccurrences**;
- поиск любых отмен в ряду повторяющихся экземпляров события с помощью свойства **cancelledOccurrences**.

### <a name="change-notifications"></a>Уведомления об изменениях
- Используйте свойство **includeResourceData** ресурса [subscription](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) для [настройки уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md). Не используйте свойство **includeProperties**.
- Получение [уведомлений об изменениях, доставляемых через концентратор событий](change-notifications-delivery.md).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Предоставление всем пользователям и группам возможности [совместного использования принтера](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) с помощью свойства **allowAllUser**.
- С помощью новых делегированных разрешений и разрешений для приложений можно пользоваться и управлять [печатью документа](/graph/api/resources/printDocument?view=graph-rest-beta&preserve-view=true), [заданием на печать](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true), [принтером](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), [предоставлением общего доступа к принтеру](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) и [определением операции печати](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true). Дополнительные сведения см. в статье об обновлениях в сфере облачной печати [за август](changelog.md#august-2020).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune в бета-версии за [август](changelog.md#august-2020).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Настройка [условий соглашения об использовании](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) для поддержки срока действия и периодичности соглашения с обязательным принятием пользователем соглашения на отдельных устройствах или повторным принятием соглашения с установленной периодичностью. 
- Используйте свойство **file** для перехода к [настраиваемому соглашению](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) условий. Не используйте свойство **files**.
- Добавление, удаление и перечисление внутренних или внешних кураторов, которые могут утверждать запросы от [подключенной организации](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true) на доступ к группе, приложению или сайту SharePoint Online. Дополнительные сведения см. в статье [Управление правами](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Разрешите дальнейшую настройку [политики авторизации](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) для клиента, например разрешите [роли пользователя по умолчанию](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true) создавать приложения или группы безопасности или читать других пользователей, разрешите пользователям возможность подписываться на подписки через электронную почту или присоединяться к клиенту через проверку электронной почты, а также предоставьте пользователям возможность самостоятельного сброса пароля.
- Управляйте [предопределенными, настраиваемыми политиками как пользовательскими потоками в клиенте Azure Active Directory B2C](/graph/api/resources/b2cuserflows?view=graph-rest-beta&preserve-view=true). См. Дополнительные сведения о [пользовательских потоках B2C](/azure/active-directory-b2c/user-flow-overview).
- Включите [возможность самостоятельной регистрации в качестве пользовательских потоков B2X в клиенте Azure Active Directory](/graph/api/resources/b2xuserflows?view=graph-rest-beta&preserve-view=true). См. Дополнительные сведения о [самостоятельной регистрации](/azure/active-directory/external-identities/self-service-sign-up-overview).

### <a name="people-and-workplace-intelligence--profile"></a>Люди и рабочая аналитика | Профиль
Добавление следующих дополнительных свойств пользовательского [профиля](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true) и управление ими. Их можно отображать в общих для пользователей интерфейсах в Microsoft 365 и сторонних приложениях:
- [addresses](/graph/api/resources/itemAddress?view=graph-rest-beta&preserve-view=true)
- [anniversaries](/graph/api/resources/personAnniversary?view=graph-rest-beta&preserve-view=true)
- [awards](/graph/api/resources/personAward?view=graph-rest-beta&preserve-view=true)
- [certifications](/graph/api/resources/personCertification?view=graph-rest-beta&preserve-view=true)
- [notes](/graph/api/resources/personAnnotation?view=graph-rest-beta&preserve-view=true)
- [patents](/graph/api/resources/itemPatent?view=graph-rest-beta&preserve-view=true)
- [publications](/graph/api/resources/itemPublication?view=graph-rest-beta&preserve-view=true)


### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Получение [отчетов об использовании приложений Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta&preserve-view=true), в частности сведений о пользователе, количества пользователей и количества используемых платформ.

### <a name="teamwork"></a>Командная работа
Получение [контента, размещенного в сообщении чата](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true), например изображений или фрагментов кода. См. [пример](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&preserve-view=true&branch=master#example-2-get-hosted-content-bytes-for-an-image), чтобы получить количество байтов содержимого для изображения.

### <a name="to-do-tasks"></a>Задачи To-Do
- Появление нового набора API для [Microsoft To Do](todo-concept-overview.md), позволяющего пользователям приложения упорядочивать и отслеживать личные задачи в клиентских приложениях Microsoft 365. Дополнительные сведения см. в статье [Использование API Microsoft To Do](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true).
- Прекращение поддержки [API задач Outlook](/graph/api/resources/outlooktask?view=graph-rest-beta&preserve-view=true).


## <a name="july-2020-new-and-generally-available"></a>Июль 2020 г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
GA функции, которая позволяет организаторам предлагать альтернативное время собраний, а приглашенным [предлагать новое время для собрания](outlook-calendar-meeting-proposals.md), когда они [предварительно принимают](/graph/api/event-tentativelyaccept?view=graph-rest-1.0&preserve-view=true&preserve-view=true) или[отклоняют](/graph/api/event-decline?view=graph-rest-1.0&preserve-view=true&preserve-view=true) событие.

### <a name="change-notifications"></a>Уведомления об изменениях
Удалено ошибочно реализованное свойство **sequenceNumber** из ресурса [changeNotification](/graph/api/resources/changenotification).

### <a name="groups"></a>Группы
Общая доступность следующих свойств объекта [group](/graph/api/resources/group): **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage** и **theme**.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Удаление пользователя в качестве зарегистрированного владельца или пользователя [устройства](/graph/api/resources/device).
- Отслеживайте изменения в новых, обновленных или удаленных локальных представлениях приложений (представленных ресурсами[servicePrincipals](/graph/api/resources/serviceprincipal)) и делегированных разрешениях (представленных ресурсами [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant)) без полного чтения всей коллекции ресурсов.
- GA [политики обеспечения безопасности по умолчанию](/graph/api/resources/identitysecuritydefaultsenforcementpolicy), которая защищает организации от распространенных атак.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- GA [политик условного доступа](/graph/api/resources/conditionalAccessPolicy), которые являются настраиваемыми правилами, определяющими сценарии доступа.
- GA [именованных расположений](/graph/api/resources/namedLocation), представляющих собой настраиваемые правила, которые определяют сетевые расположения, используемые в политике условного доступа.

### <a name="schema-extensions"></a>Расширения схемы
Функция [расширений схемы](/graph/api/resources/schemaextension) теперь общедоступна в [Microsoft Cloud for US Government](./deployments.md).

### <a name="teamwork"></a>Командная работа
Используйте делегированные разрешения `TeamsAppInstallation.ReadForTeam` или`TeamsAppInstallation.ReadWriteForTeam`, или разрешения приложений `TeamsAppInstallation.ReadForTeam.All` или `TeamsAppInstallation.ReadWriteForTeam.All`, чтобы [составить список приложений, установленных в группе](/graph/api/teamsappinstallation-list).

## <a name="july-2020-new-in-preview-only"></a>Июль 2020 г.: новые возможности только в предварительной версии

### <a name="cloud-communications"></a>Облачные коммуникации
- Использование операции [update](/graph/api/onlinemeeting-update?view=graph-rest-beta&preserve-view=true&preserve-view=true), чтобы обновить свойство **startDateTime**, **endDateTime**, **participants** или **subject** для [собрания по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true&preserve-view=true).
- Подписка на уведомления об изменениях о доступности пользователя в Microsoft Teams, представленной ресурсом [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--call-records"></a>Облачные коммуникации | Записи звонков
- [Получение](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta&preserve-view=true) записей звонков по ТСОП.
- [Получение](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta&preserve-view=true) записей звонков прямой маршрутизации.

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Появление [дел обнаружения электронных данных](/graph/api/resources/ediscoverycase?view=graph-rest-beta&preserve-view=true), которые могут содержать хранителей, удержания, коллекции, наборы для проверки и операции экспорта, доступные для использования в качестве доказательств в судебных делах.
Приложения теперь могут [запрашивать](/graph/api/resources/reviewsetquery?view=graph-rest-beta&preserve-view=true) и вызывать [данные наборов для проверки](/graph/api/resources/reviewset?view=graph-rest-beta&preserve-view=true), собранные для использования в судебных разбирательствах, расследованиях и нормативных запросах. Это добавление входит в состав [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true) Microsoft 365.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Использование разрешения приложений `Printer.ReadWrite.All` и [шифрования Internet Printing Protocol (IPP)](https://tools.ietf.org/html/rfc8010) для [обновления принтера](/graph/api/printer-update?view=graph-rest-beta&preserve-view=true).
- Использование разрешений приложений `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All` или `PrintJob.ReadWrite.All` для [получения задания печати](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true) или [перечисления заданий печати для принтера](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- При [получении задания печати](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true) используйте `$expand` для получения [задач печати](/graph/api/resources/printtask?view=graph-rest-beta&preserve-view=true), выполняемых или выполненных в рамках задания. Задачи печати, [определения задач](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true) и [триггеры задач](/graph/api/resources/printtasktrigger?view=graph-rest-beta&preserve-view=true) используются при [печати по запросу](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).
- [Перенаправление задания печати](/graph/api/printjob-redirect?view=graph-rest-beta&preserve-view=true) на другой принтер в рамках печати по запросу.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [июль](changelog.md#july-2020) в бета-версии.

### <a name="groups"></a>Группы
Используйте свойство **isAssignableToRole** [группы](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) Microsoft 365 и настройте его при создании группы, чтобы указать, можно ли назначить группу для роли Azure AD. Эта [помогает управлять назначениями ролей в Azure AD](/azure/active-directory/users-groups-roles/roles-groups-concept). Например, вместо назначения отдельным пользователям роли Azure AD привилегированный администратор ролей или глобальный администратор может создать группу Microsoft 365 и назначить ее этой роли, чтобы при присоединении пользователей к _группе_ им неявно назначалась нужная роль.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Получите маркер доступа](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta&preserve-view=true) для авторизации службы контроля использования Azure AD для предоставления пользователям доступа к приложению.
- [Получите](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta&preserve-view=true) или[обновите](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta&preserve-view=true)настройки управления правами, которые контролируют доступ к группам, приложениям и сайтам SharePoint Online для пользователей внутри или вне вашей организации. 

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Включение уровней риска пользователя (`low`, `medium`, `high`, `none`) при рассмотрении применения [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- [Использование смены пароля в качестве предоставления управления](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta&preserve-view=true#special-considerations-when-using-passwordchange-as-a-control), чтобы пройти политику условного доступа.
- Использование [поставщика Open ID Connect](/graph/api/resources/openidconnectprovider?view=graph-rest-beta&preserve-view=true) (ODIC) в качестве поставщика удостоверений в клиенте Azure AD и клиенте Azure AD B2C. Его свойство **claimsMapping** позволяет Azure AD [сопоставлять утверждения](/graph/api/resources/claimsmapping?view=graph-rest-beta&preserve-view=true) от поставщика OIDC с утверждениями, которые распознает и использует Azure AD.

### <a name="people-and-workplace-intelligence--insights"></a>Люди и рабочая аналитика | Аналитические сведения
Используйте более [детальное управление конфиденциальностью](insights-customize-item-insights-privacy.md) в отношении доступности и отображения[элементов аналитики](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true) в Microsoft 365. Эти данные представляют собой отношения между пользователем и документами в OneDrive для бизнеса, вычисляемые с использованием передовых методов анализа и машинного обучения. 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>Люди и рабочая аналитика | Настройка карточки профиля
Администраторы могут [настроить свойства, представленные в карточке профиля для своих организаций](add-properties-profilecard.md), используя API-интерфейс для [свойств карточки профиля](/graph/api/resources/profilecardproperty?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Сайты и списки
Доступ к таксономии [банка терминов](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true) SharePoint — иерархии, состоящей из ресурсов [group](/graph/api/resources/termstore-group?view=graph-rest-beta&preserve-view=true), [set](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true) и [term](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true), а также ресурсов [relation](/graph/api/resources/termstore-relation?view=graph-rest-beta&preserve-view=true) для связей между терминами.

### <a name="workbooks-and-charts"></a>Книги и диаграммы
[Получение состояния и любого результата](/graph/api/workbookoperation-get?view=graph-rest-beta&preserve-view=true) длительной [операции](/graph/api/resources/workbookoperation?view=graph-rest-beta&preserve-view=true) в [книге](/graph/api/resources/workbook?view=graph-rest-beta&preserve-view=true).



## <a name="june-2020-new-and-generally-available"></a>Июнь 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
- Использование `Accept-Language` заголовка HTTP при [создании онлайнового собрания](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0&preserve-view=true&preserve-view=true) для предоставления объединенной информации на основе языковой среды.
- Использование [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0&preserve-view=true&preserve-view=true) для возврата онлайнового собрания с указанным значением **externalId** или его создание в случае отсутствия, чтобы упростить внедрение получившегося собрания в стороннем календаре.

### <a name="files"></a>Файлы
- Улучшенная поддержка синхронизации:
  - Использование свойства **pendingOperations** для определения [операций](/graph/api/resources/pendingoperations), которые могут обновить бинарное содержание файла [driveItem](/graph/api/resources/driveitem), ожидающего выполнения.
  - [Восстановление](/graph/api/driveitem-restore) объекта **driveItem**, который был удален и находится в корзине OneDrive персональный.
- Получение или настройка ориентации ресурса [photo](/graph/api/resources/photo). Настройка поддерживается в OneDrive персональный.
- Использование защищенного алгоритма хэширования (SHA-256) для улучшения безопасности и целостности данных ресурса [file](/graph/api/resources/file).
- Использование параметра `deferCommit` для откладывания окончательного создания при [передаче, как правило, большого файла](/graph/api/driveitem-createuploadsession) в OneDrive для бизнеса до тех пор, пока приложение не выполнит запрос на выполнение передачи.
- Использование свойства **fileSize** для предоставления оценки как части параметра **item**, чтобы проверить квоту до [передачи файла](/graph/api/driveitem-createuploadsession) в OneDrive персональный.
- Поиск [storagePlanInformation](/graph/api/resources/storageplaninformation) с помощью свойства **quota** ресурса [drive](/graph/api/resources/drive), чтобы проверить доступность планов с более высокими квотами на хранение.

### <a name="groups"></a>Группы
Использование разрешений приложений `Group.Read.All` и `Group.ReadWrite.All` для получения ресурсов группы [беседа](/graph/api/resources/conversation) и [цепочки беседы](/graph/api/resources/conversationthread).

### <a name="identity-and-access"></a>Удостоверение и доступ 
- Общедоступная версия из двух наборов API для [защиты удостоверения](/graph/api/resources/identityprotectionroot): API [выявления рисков](/graph/api/resources/riskdetection) и [рискованных пользователей](/graph/api/resources/riskyuser).

### <a name="security"></a>Безопасность
- Отслеживание указанного ниже как свойств [оповещения](/graph/api/resources/alert?view=graph-rest-1.0&preserve-view=true&preserve-view=true):
  - Идентификаторы инцидентов, связанных с оповещением.
  - Идентификация [ресурса](/graph/api/resources/securityResource?view=graph-rest-1.0&preserve-view=true#securityresourcetype-values) как атакованного или как связанного ресурса в оповещении.
  - Указание начального и конечного расположений [сетевого подключения](/graph/api/resources/networkconnection?view=graph-rest-1.0&preserve-view=true), связанных с оповещением.

### <a name="sites-and-lists"></a>Сайты и списки
Указание геолокационных данных в [определении столбца](/graph/api/resources/columndefinition) для ресурса [списка](/graph/api/resources/list) SharePoint.

### <a name="teamwork"></a>Командная работа
- Использование делегированного разрешения [AppCatalog.Read.All](./permissions-reference.md#appcatalog-resource-permissions) для перечисления [приложений](/graph/api/resources/teamsapp?view=graph-rest-1.0&preserve-view=true) из каталога приложений Microsoft Teams.
- [Получение информации о папке](/graph/api/channel-get-filesfolder) с сопоставлением вкладки **Файлы** [канала](/graph/api/resources/channel) Teams.
- [Получение канала по умолчанию](/graph/api/team-get-primarychannel) с меткой **Общие** [команды](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Июнь 2020 г.: новые возможности только в предварительной версии

### <a name="calendar"></a>Календарь
Помимо отслеживания инкрементных изменений событий в **calendarView** (коллекции или событий, ограниченных начальными _и_ конечными данными), применяется функция [delta](/graph/api/event-delta?view=graph-rest-beta&preserve-view=true) к событиям в почтовом ящике пользователя или к событиям в календаре определенного пользователя.

### <a name="cloud-communications--presence"></a>Облачные коммуникации | Присутствие
[Получение статуса присутствия](/graph/api/presence-get?view=graph-rest-beta&preserve-view=true) всех пользователей в организации или определенного пользователя организации.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Указание [полей печати](/graph/api/resources/printmargin?view=graph-rest-beta&preserve-view=true) при настройке [документа для печати](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true).
- Поддержка следующих [возможностей принтера](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true):
  - направления подачи;
  - печати диапазонов страниц;
  - разрешение печати в точках на дюйм;
  - максимальный размер очереди заданий печати в байтах;
  - входные лотки;
  - поля;
  - разбор по копиям;
  - масштабирование документов.
- Поддержка разрешения печати (в точках на дюйм) и масштабирование документов как часть [настроек принтера по умолчанию](/graph/api/resources/printerdefaults?view=graph-rest-beta&preserve-view=true).
- Поддержка следующих настроек [конфигурации документов](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta&preserve-view=true):
  - входные лотки;
  - выходные лотки;
  - размеры носителей;
  - поля;
  - типы носителей;
  - финишная обработка, например сшивание или брошюрование;
  - количество страниц на лист;
  - многостраничный макет с указанием направления при размещении страниц на листе;
  - разбор по копиям;
  - масштабирование.
- Расширение документов при [перечислении заданий печати](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- [Регистрация принтера]() и использование ресурса [printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta&preserve-view=true) для отслеживания и проверки регистрации принтера.
- [Получение долгосрочной регистрации принтера](/graph/api/printoperation-get?view=graph-rest-beta&preserve-view=true) для текущего пользователя или клиента приложения.
- Несколько переименований свойств и типов нумерации. Более подробные сведения приведены в обновлениях журнала изменений для облачной печати за [июнь](changelog.md#june-2020).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [июнь](changelog.md#june-2020) в бета-версии.

### <a name="education"></a>Образование
- Возможность использовать делегированные разрешения `EduRoster.ReadBasic` для [получения](/graph/api/educationuser-get?view=graph-rest-beta&preserve-view=true) идентификатора [преподавателя](/graph/api/resources/educationteacher?view=graph-rest-beta&preserve-view=true) или [учащегося](/graph/api/resources/educationstudent?view=graph-rest-beta&preserve-view=true) во внешней исходной программе как свойство **externalId**.
- Использование свойства **externalSource** для отслеживания значения `lms`, если [организация](/graph/api/resources/educationorganization?view=graph-rest-beta&preserve-view=true) или [класс](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) в сфере образования созданы в системе управления обучением (LMS).

### <a name="identity-and-access"></a>Удостоверение и доступ
- ИТ-специалисты могут использовать ресурсы [connector](/graph/api/resources/connector?view=graph-rest-beta&preserve-view=true). Это легкие агенты для подключения к [прокси приложения Azure AD](/azure/active-directory/manage-apps/what-is-application-proxy) и [внешней публикации локальных веб-приложений](/graph/api/resources/onpremisespublishing?view=graph-rest-beta&preserve-view=true), чтобы удаленные пользователи организации могли безопасно получить доступ к этим приложениям.
- Управление [политикой проверки подлинности](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta&preserve-view=true) на уровне клиента для включения или отключения [регистрации с самообслуживанием](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta&preserve-view=true) внешних пользователей.
- [Подготовка учетной записи пользователя по требованию](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta&preserve-view=true) и возможность указывать объекты для выполнения правил подготовки и синхронизации.

### <a name="search"></a>Поиск
- Использование улучшения [свойства](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true) в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true) **isRefinable** для включения фильтрации результатов поиска и более точного управления взаимодействием при поиске, а также **псевдонимов** и **меток** для повышения релевантности.
- Возможность указать до 128 ресурсов **свойства** в **схеме**.
- Использование [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta&preserve-view=true) для диагностики.

### <a name="users"></a>Пользователи
- Использование свойства **userPurpose** [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) для выявления и дифференциации почтового ящика для одного пользователя от общего почтового ящика и почтового ящика оборудования в Exchange Online. 
- Использование [настроек пользователей](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) для [получения](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) или [обновления](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) [предпочитаемых языков и региональных настроек](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta&preserve-view=true).
- Настройки пользователей — это взаимосвязь, доступная через [пользователя](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true), которая обеспечивает единообразное взаимодействие с пользователем в разных приложениях за счет использования профиля Azure AD для применения одних и тех же предпочтений пользователя. См. статью [Чем отличаются пользовательские настройки от настроек почтового ящика](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true#user-preferences-for-languages-and-regional-formats).


## <a name="may-2020-new-and-generally-available"></a>Май 2020 г.: новые и общедоступные возможности

### <a name="calendar--place"></a>Календарь | Место
Общедоступная версия [API мест](/graph/api/resources/place) в версии 1.0. Используйте этот API в производственных приложениях, чтобы получить, обновить или удалить [помещение](/graph/api/resources/room) или [список помещений](/graph/api/resources/roomlist) в клиенте. [Узнайте больше](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) об API мест.

### <a name="change-notifications"></a>Уведомления об изменениях
- Подпишитесь на уведомления об изменениях в Microsoft Cloud для государственных учреждений США.

### <a name="cloud-communications--call-records"></a>Облачные коммуникации | Записи звонков
- Общедоступная версия [API записи звонков](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0&preserve-view=true). Используйте ресурс [callRecord](/graph/api/resources/callrecord?view=graph-rest-1.0&preserve-view=true) для получения метаданных звонков и онлайн-собраний в Microsoft Teams и Skype.
- Подпишитесь на [уведомления об изменениях](./webhooks.md) для отслеживания изменений всех ресурсов **callRecord** в организации.
- [Список сеансов](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true) в **callRecord** и дополнительное [разворачивание каждого сеанса на сегменты списка](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true#example-2-get-session-list-with-segments) в записи звонка.
- Поддержка значений диапазонов на 60 ГГц (`frequency60GHz`) и `unknownFutureValue` WiFi конечной точки мультимедиа в сегменте.
- Поддержка голосовой почты в качестве возможного типа конечной точки на стороне службы в [сегменте](/graph/api/resources/callrecords-segment) связи.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [май](changelog.md#may-2020) в версии 1.0.

### <a name="graph-explorer"></a>Песочница Graph
Используйте множество новых функций [песочницы Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer), которые улучшают обучение и создание прототипов в песочнице. Например:
- Просматривайте фрагменты кода, соответствующие введенному запросу API REST, в C#, Java, JavaScript и Objective C.
- Войдя в систему с помощью клиента, просматривайте и копируйте маркер доступа в свое избранное клиентское приложение для REST.

Дополнительные сведения см. в статье [Новая песочница Graph теперь общедоступная](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/).

### <a name="groups"></a>Группы
- При синхронизации локального каталога с Azure Active Directory с помощью Azure AD Connect теперь возвращаются свойства **onPremisesDomainName**, **onPremisesNetBiosName** и **onPremisesSamAccountName** в составе ресурса [group](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true).
- Подпишитесь на уведомления об изменении для ресурсов [group](/graph/api/resources/group) в службе Microsoft Cloud для Китая, предоставляемой 21Vianet.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Общедоступная версия API субъектов-служб в версии 1.0 Используйте ресурс [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true) в производственных приложениях для программного управления экземплярами приложений и контроля того, что приложение может сделать в рамках вашего клиента. Вы можете управлять тем, кто может использовать приложение, к каким ресурсам у приложения есть доступ, таким как добавление учетных данных, обработка сертификатов с истекающим сроком действия, а также управление делегированными разрешениями и назначениями ролей приложения.
- Общедоступная версия API [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0&preserve-view=true), который регистрирует назначение [appRole](/graph/api/resources/approle?view=graph-rest-1.0&preserve-view=true) (представляющее утверждение `roles` в маркерах идентификатора и маркерах доступа) [пользователю](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), [группе](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) или [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true).
- Используйте Facebook в качестве поставщика удостоверений в Azure Active Directory.
- Используйте делегированное разрешение или разрешение приложения `AppRoleAssignment.ReadWrite.All`, чтобы разрешить приложению управлять предоставлением разрешений для разрешений приложений для любого API (включая Microsoft Graph) и назначений приложений для любого приложения, соответственно, при наличии вошедшего в систему пользователя или без него.


### <a name="microsoft-graph-sdks"></a>Пакеты SDK Microsoft Graph
См. новые рекомендации к SDK в отношении следующего:
- [Разбиение на страницы](./sdks/paging.md)
- [Пакетная обработка](./sdks/batch-requests.md)
- [Отправка больших файлов в OneDrive](./sdks/large-file-upload.md)
- [Настройка клиента службы SDK с помощью компонентов ПО промежуточного слоя для HTTP](./sdks/customize-client.md).

### <a name="teamwork"></a>Командная работа
- Если ваш сценарий предполагает онлайн-собрания в Teams, см. рекомендации [ Как выбрать](choose-online-meeting-api.md) между [API календаря](outlook-calendar-online-meetings.md) и [API облачных средств обмена данными](cloud-communications-online-meetings.md) для создания онлайн-собраний и подключения к ним.
- [Отправка сообщений](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) и [ответ](/graph/api/channel-post-messagereply?view=graph-rest-1.0&preserve-view=true) на сообщения в [канале](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true).
- Получите расположение OneDrive для бизнеса файлов для [канала](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true), используя свойство навигации **fileFolder**.

### <a name="teamwork--shifts"></a>Командная работа | Смены
Общедоступная версия [shifts API](/graph/api/resources/shift?view=graph-rest-1.0&preserve-view=true) в версии 1.0. Используйте этот API в производственных приложениях для создания, обновления и управления расписаниями сотрудников без компьютеров, чтобы обеспечить их взаимодействие и эффективность совместной работы.

### <a name="users"></a>Пользователи
- Подпишитесь на уведомления об изменении для ресурсов [user](/graph/api/resources/user) в службе Microsoft Cloud для Китая, предоставляемой 21Vianet.
- Отслеживайте состояние и дату/время последнего изменения состояния внешнего пользователя, который был [приглашен](/graph/api/invitation-post?view=graph-rest-1.0&preserve-view=true) присоединиться к организации, с помощью свойств **externalUserState** и **externalUserStateChangeDateTime** ресурса **user**.

## <a name="may-2020-new-in-preview-only"></a>Май 2020 г.: новые возможности только в предварительной версии

### <a name="change-notifications"></a>Уведомления об изменениях
- Используйте формально схематизированные типы [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta&preserve-view=true) и [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta&preserve-view=true) для обработки уведомлений об изменении ресурса. 
- Отслеживайте, находится ли уведомление в последовательности или утеряно, используя свойство **sequenceNumber** в ресурсе **changeNotification**.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Ресурсы [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) и [printerShare](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) теперь аналогичны и имеют одинаковые свойства.
- Очищены некоторые имена свойств и типов вокруг общих принтеров:
  - Чтобы получить список общих принтеров, зарегистрированных в клиенте, используйте свойство навигации **shared** в [печати](/graph/api/resources/print?view=graph-rest-beta&preserve-view=true). 
  - Дополнительные сведения см. в журнале изменений за[май](changelog.md#may-2020).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [май](changelog.md#may-2020) в бета-версии.

### <a name="groups"></a>Группы
- [Оцените](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta&preserve-view=true), является ли (может являться) пользователь или устройство членом динамической группы, используя существующее правило для [группы](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) или указанное правило. [Динамическое членство на основе правила](/azure/active-directory/users-groups-roles/groups-dynamic-membership) снижает затраты на администрирование добавления и удаления участников.
- В Microsoft 365 при создании [группы](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) настройте поведение группы, указав варианты поведения в свойстве **resourceBehaviorOptions**. Например, вы можете разрешить участникам публиковать записи, подписывать новых участников в беседы, отключать приветственные сообщения электронной почты и скрывать группу в Outlook.
- Укажите ресурсы для подготовки в свойстве **resourceProvisioningOptions**, которые обычно не входят в объем создания [группы](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) по умолчанию. В настоящее время поддерживается подготовка группы в качестве [команды](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) с возможностями Microsoft Teams.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Применяйте параметры системного запроса OData (`$count`, `$filter`, `$search`) при получении коллекций сущностей, которые являются производными [directoryObject](). Вы можете выполнить [поиск определенных маркеров](./query-parameters.md#using-search-on-directory-object-collections) в свойствах **displayName** и **description** этих сущностей, а также использовать OData cast для обрезки результатов **directoryObject** до определенных производных типов. Подробные сведения приведены в статье [Создание расширенных запросов в Microsoft Graph с использованием атрибутов $count, $filter, $search и $orderby](https://developer.microsoft.com/ru-RU/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/).
- В рамках [API защиты удостоверений](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true) используйте свойство **riskEventType**, чтобы [получить тип определенного риска](/graph/api/riskdetection-get?view=graph-rest-beta&preserve-view=true) или [получить тип риска в журнале пользователя](/graph/api/riskyuser-list-history?view=graph-rest-beta&preserve-view=true). Не используйте свойство **riskType**, поскольку оно устарело.
- Укажите типы клиентского приложения в свойстве **clientAppTypes** [набора свойств](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta&preserve-view=true) для [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Используйте делегированное разрешение `EntitlementManagement.Read.All`, чтобы разрешить приложению считывание пакетов доступа, а также связанных ресурсов по управлению правами от имени пользователя, выполнившего вход.
- Используйте делегированные разрешения или разрешения приложения `Application.Read.All` и `Application.ReadWrite.All`, чтобы [перечислить приложения](/graph/api/application-list?view=graph-rest-beta&preserve-view=true) в организации.
- Управляйте параметрами авторизации в Azure AD с использованием типа ресурса [authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Командная работа
- Приложения Teams, [поддерживающие единый вход (SSO),](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) могут указывать `WebApplicationInfo.id` из манифеста приложения Teams в свойстве **azureADAppId** в [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true).
- Используйте [детализированные разрешения](./permissions-reference.md#teams-resource-specific-consent-permissions) для доступа к ресурсам [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) и [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true).


## <a name="april-2020-new-and-generally-available"></a>Апрель 2020 г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
- [Делитесь календарями или делегируйте их](outlook-share-or-delegate-calendar.md) программным способом, соответствующим пользовательскому интерфейсу Outlook. Поддерживается отслеживание разрешений текущего пользователя и состояния общего доступа к календарю, а также следующие возможности:
  - Для каждого [календаря](/graph/api/resources/calendar?view=graph-rest-1.0&preserve-view=true) теперь можно управлять [разрешениями](/graph/api/resources/calendarpermission?view=graph-rest-1.0&preserve-view=true) каждого пользователя, которому предоставлен доступ к календарю. 
  - Для каждого [почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true) теперь можно указать, кто получает сообщения о собраниях и ответы на эти сообщения: делегат, владелец почтового ящика или и тот, и другой. 
- [Создание или обновление события в виде собрания по сети](outlook-calendar-online-meetings.md):
  - В каждом **календаре** можно указать разрешенных и используемых по умолчанию поставщиков собраний по сети.
  - Можно создать или обновить [мероприятие](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), доступное по сети, и предоставить участникам сведения для присоединения к собранию по сети. 
  - В частности, можно использовать **onlineMeetingProvider** и **onlineMeeting** — это новые свойства **мероприятий**, с помощью которых можно задать или указать Microsoft Teams в качестве поставщика собраний по сети. Это временное решение [известной проблемы](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) со свойством **onlineMeetingUrl**.
- Добавление [файловых вложений до 150 МБ](outlook-large-attachments.md) в [событие](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Файлы
- [Извлекайте](/graph/api/driveitem-checkout?view=graph-rest-1.0&preserve-view=true) и [возвращайте](/graph/api/driveitem-checkin?view=graph-rest-1.0&preserve-view=true) файлы в OneDrive, чтобы управлять их обновлением и делать обновления доступными для других пользователей.
- Применяйте необязательный пароль и дату/время истечения срока действия в качестве параметров действий[пригласить](/graph/api/driveitem-invite?view=graph-rest-1.0&preserve-view=true) и [создать ссылку совместного доступа](/graph/api/driveitem-createlink?view=graph-rest-1.0&preserve-view=true) для совместного доступа к [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).
- Получите или задайте пароль и дату/время истечения срока действия [разрешения](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true), а также отслеживайте [identitySet](/graph/api/resources/identityset?view=graph-rest-1.0&preserve-view=true) пользователей, которым предоставлено разрешение на совместный доступ к **driveItem**.
- Получите [разрешение](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true) для [общего элемента диска](/graph/api/resources/shareddriveitem?view=graph-rest-1.0&preserve-view=true), используя свойство навигации **permission**.
- Ограничьте действия пользователей со [ссылкой совместного доступа](/graph/api/resources/sharinglink?view=graph-rest-1.0&preserve-view=true) только просмотром без возможности скачивания содержимого общего элемента **driveItem** в OneDrive для бизнеса или в SharePoint.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Чтобы управлять ролями и назначать доступ к ресурсам в провайдерах управления доступом на основе ролей (RBAC), таких как Microsoft Intune, используйте [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0&preserve-view=true). Ресурс **unifiedRoleAssignmentMultiple** поддерживает определение одной роли в массиве областей и назначение роли для нескольких субъектов (например, пользователей).
- Получите доступ к определенным типам [политик для организации](/graph/api/resources/policy-overview?view=graph-rest-1.0&preserve-view=true), используя `/policies`сегмент URL и указав тип политики. Например, организация может применить политику для автоматического выхода пользователя из веб-сеанса после периода бездействия; см. операции CRUD для экземпляров [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0&preserve-view=true). Это [серьезное изменение](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/), упрощающее обнаружение всех политик путем группировки всех типизированных политик в сегменте `/policies`. Доступ к другим типизированным политикам осуществляется аналогичным образом: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0&preserve-view=true) и [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0&preserve-view=true). 

### <a name="mail"></a>Почта
Добавление [файловых вложений до 150 МБ](outlook-large-attachments.md) в [сообщение](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true).

### <a name="sites-and-lists"></a>Сайты и списки
- [Список сайтов](/graph/api/sites-list-followed?view=graph-rest-1.0&preserve-view=true), на которые подписан пользователь.
- Определите географическую область [семейства веб-сайтов](/graph/api/resources/sitecollection?view=graph-rest-1.0&preserve-view=true) с помощью свойства **dataLocationCode**.
- Определите клиента файла, папки или другого элемента в SharePoint, путем доступа к свойству **tenantId**, которое является частью **sharepointIds** в [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).

## <a name="april-2020-new-in-preview-only"></a>Апрель 2020 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать

Назначьте разрешенным пользователям и группам доступ к определенным [общим принтерам](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) Универсальной печати — облачной инфраструктуры печати Microsoft 365. Чтобы воспользоваться возможностями надежного централизованного управления печатью и предложить пользователям простой, но полнофункциональный и безопасный интерфейс печати, ознакомьтесь с [объявлением Универсальной печати](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775) и присоединитесь к программе по ознакомлению с предварительной версией.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [апрель](changelog.md#april-2020).

### <a name="groups"></a>Группы
Определите, какое приложение создало [группу](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true), по идентификатору приложения.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Отслеживание изменений](/graph/api/administrativeunit-delta?view=graph-rest-beta&preserve-view=true), касающихся [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true).
- [Отслеживание изменений](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta&preserve-view=true), касающихся [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta&preserve-view=true).
- [Управление](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) пользовательскими [методами проверки подлинности](/graph/api/resources/authenticationmethod?view=graph-rest-beta&preserve-view=true), среди которых [пароль](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta&preserve-view=true) или [телефон](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta&preserve-view=true). Например, [сброс пароля пользователя](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta&preserve-view=true) и [получение состояния сброса](/graph/api/authenticationoperation-get?view=graph-rest-beta&preserve-view=true) или [добавление номера телефона](/graph/api/authentication-post-phonemethods?view=graph-rest-beta&preserve-view=true) пользователя для проверки подлинности с помощью SMS или голосового вызова, если для этого пользователя включена соответствующая политика.

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
[Список](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta&preserve-view=true) [проверяющих сторон](/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts), настроенных в службах федерации Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Просмотр данных о **созданных собраниях** и **действиях с уведомлениями о собраниях** в отчетах CSV, включающих [счетчики действий с электронной почтой](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta&preserve-view=true), [счетчики пользователей, совершающих действия с электронной почтой](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta&preserve-view=true) и [данные о действиях пользователей с электронной почтой](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta&preserve-view=true).


## <a name="march-2020-new-and-generally-available"></a>Март 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачные коммуникации
- Получите функцию маршрутизации вызовов и контекст входящих [вызовов](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true).
- [Обновите состояние записи](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0&preserve-view=true) звонка.
- Укажите информацию о записи для [участника](/graph/api/resources/participant?view=graph-rest-1.0&preserve-view=true), включая инициатора и состояние записи.
- Для уникальной идентификации участников конференции или [звонка](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) от участника к участнику используйте свойство **callChainId**.
- Определите как часть [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0&preserve-view=true) код страны и тип конечной точки (например, Skype для бизнеса или Skype для бизнеса VoIP) участника.
- Сторонние партнеры в области устройств видеоконференцсвязи (VTC) могут регистрировать и предоставлять сведения о качестве связи для своих устройств через бот Cloud Video Interop (CVI) с помощью функции [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0&preserve-view=true). Качество связи определяется данными открытого типа о [звуке](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0&preserve-view=true), [видео](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0&preserve-view=true) и [демонстрации экрана](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Файлы
- [Удаленные элементы](/graph/api/resources/remoteitem?view=graph-rest-1.0&preserve-view=true), к которым пользователю предоставлен общий доступ, добавленные в хранилище OneDrive пользователя или возвращенные как результаты поиска, могут содержать метаданные для изображения или видео.
- [Отслеживайте](/graph/api/driveitem-follow?view=graph-rest-1.0&preserve-view=true) объект [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true) для удобного доступа или упрощения таких действий, как перемещение, копирование и сохранение в определенном формате. Используйте [отмену отслеживания](/graph/api/driveitem-unfollow?view=graph-rest-1.0&preserve-view=true), чтобы прекратить отслеживание элемента диска.
- [Предоставьте](/graph/api/permission-grant?view=graph-rest-1.0&preserve-view=true) пользователям разрешение на доступ к ссылке для общего доступа, чтобы поделиться соответствующим элементом диска.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Отслеживайте изменения](/graph/api/orgcontact-delta?view=graph-rest-1.0&preserve-view=true) в [контактах организации](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true).
- Используйте свойство **riskEventTypes_v2**, чтобы получить типы событий риска, связанные с [входом](/graph/api/resources/signin?view=graph-rest-1.0&preserve-view=true).
- Используйте делегированное разрешение `User.ManageIdentities.All`, чтобы разрешить приложению считывать, обновлять и удалять удостоверения, связанные с учетной записью пользователя, к которой имеет доступ зарегистрированный пользователь. Используйте это разрешение на уровне приложения без зарегистрированного пользователя. Это позволяет приложению [определить](/graph/api/user-update?view=graph-rest-1.0&preserve-view=true), с помощью каких удостоверений пользователь может войти.

### <a name="reports"></a>Отчеты
Используйте Администратор службы Teams и Администратор связи Teams в качестве принятых ролей пользователя, чтобы приложения могли читать отчеты об использовании службы Microsoft 365 от имени пользователя в качестве [форм делегированной пользователем авторизации](reportroot-authorization.md). 

### <a name="sites"></a>Сайты
- Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-1.0&preserve-view=true) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-1.0&preserve-view=true) сайтов SharePoint. 
- [Подпишитесь на уведомления об изменениях](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) в [списке](/graph/api/resources/list?view=graph-rest-1.0&preserve-view=true) SharePoint.

## <a name="march-2020-new-in-preview-only"></a>Март 2020: Новое только в превью

### <a name="calendar"></a>Календарь
- Используйте свойство **calendarGroupId**, чтобы получить группу [календаря](/graph/api/resources/calendargroup?view=graph-rest-beta&preserve-view=true), в которой создан [календарь](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true).
- Используйте свойство **в черновике**, чтобы идентифицировать [событие](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) как собрание, которое пользователь обновил в Outlook, но не отправил для обновления участников.

### <a name="cloud-communications"></a>Облачные коммуникации
- Используйте [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta&preserve-view=true), чтобы получить экземпляр [онлайн-собрания](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) с помощью внешнего настраиваемого идентификатора или создать его, если он еще не существует.
- Вы можете использовать свойство **externalId**, чтобы определить онлайн-собрание с помощью внешнего настраиваемого идентификатора.
- Используйте необязательный заголовок HTTP-запроса `Accept-Language`, чтобы [создать](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true) или [получить](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) экземпляр онлайн-собрания. При успешном выполнении операции отображается содержимое свойства **joinInformation** на указанном языке и вариант локали.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [март](changelog.md#march-2020).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте разрешение `Auditlogs.Read.All` для списка [действий входа](/graph/api/resources/signinactivity?view=graph-rest-beta&preserve-view=true) [пользователя](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).
- Используйте разрешение на уровне приложения `PrivilegedAccess.Read.AzureResources` для [управления привилегированными удостоверениями (PIM) ресурсов Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true), чтобы настроить рабочий процесс доступа «точно в срок» для ролей инфраструктуры Azure на уровне группы управления, подписки, группы ресурсов или ресурса.
- Используйте объект [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta&preserve-view=true), чтобы [получить](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta&preserve-view=true) или [обновить](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta&preserve-view=true) предварительно настроенные параметры безопасности по умолчанию, которые защищают организации от распространенных атак.
- Используйте сегмент `identity` при вызове API условного доступа. Например, чтобы [получить](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta&preserve-view=true) [политику условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true): `GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`.
- Используйте свойство **authenticationRequirement**, чтобы получить наивысший уровень проверки подлинности, необходимый для успешного выполнения всех действий [входа](/graph/api/resources/signin?view=graph-rest-beta&preserve-view=true).
- Используйте разбивку на страницы при [перечислении событий подготовки](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta&preserve-view=true) в вашем клиенте.

### <a name="search"></a>Поиск
- Чтобы добавить данные в файле к результатам поиска, просто индексируйте данные как [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true). Тип **externalFile** не рекомендуется.
- [Обновите](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) [элемент в индексе](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true), обновив представление элемента в виде обычного текста (представленное свойством **content**) или контейнер свойств элемента (представленный свойством **properties**). При обновлении любого свойства в контейнере свойств перезаписывается весь контейнер свойств, поэтому убедитесь, что все свойства элемента явным образом включены в обновление.
- Проверьте наличие `HTTP 429` и заголовка ответа `Retry-After` после вызова операции [создания](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true), [обновления](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) или [удаления](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) элемента **externalItem**. Самый быстрый способ выполнить восстановление после [регулирования](throttling.md#best-practices-to-handle-throttling) — отложить запросы с помощью задержки `Retry-After`.

### <a name="teamwork"></a>Командная работа
Используйте разрешение на уровне приложения `ChannelMessage.Read.All` для чтения экземпляров [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) в каналах без зарегистрированного пользователя.

### <a name="universal-print"></a>Универсальная печать
Появление [API универсальной печати](universal-print-concept-overview.md), позволяющего пользователям печатать в Интернете или из приложения. API позволяет ИТ-администраторам управлять доступом пользователей и групп к принтерам в облаке Microsoft 365, а также удаленным общим доступом к принтерам для поддерживания доступности, отслеживать состояние принтеров и создавать отчеты о заархивированных заданиях печати и использовании. 

Обратите внимание, что с марта 2020 г. _служба_ универсальной печати доступна в закрытой предварительной версии. Дополнительные сведения об участии см. в статье [Представляем универсальную печать: облачное решение для печати](https://aka.ms/announcinguniversalprint).


## <a name="february-2020-new-and-generally-available"></a>2020 февраля: новая и общедоступная

### <a name="calendar"></a>Календарь
Просмотрите пример [создания события в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md), а также действия и свойства, доступные для делегата, приглашенных и владельца календаря во время этого процесса.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Чтобы повысить безопасность при подписке на [уведомления об изменениях пользовательских данных](webhooks.md), [установите Transport Layer Security (TLS) 1.2](/configmgr/core/plan-design/security/enable-tls-1-2) или выше на клиентах и серверах сайтов, используемых в процессе уведомления. Новое требование вводится поэтапно, начиная с 15 февраля 2020 года. К 15 мая 2020 года все конечные точки уведомления должны соответствовать новому требованию TLS. [Узнайте о стадиях развертывания](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) и при необходимости воспользуйтесь новым свойством **latestSupportedTlsVersion** в качестве временного решения, чтобы избежать сбоев подписки до выполнения обновления TLS.
- Используйте соответствующие типы [запроса оценки угроз](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0&preserve-view=true) для отслеживания угроз от [почты](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0&preserve-view=true), [файла сообщения электронной почты](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (. EML-файл), [файлов вложений электронной почты](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (текстовых файлов, файлов Word и двоичных файлов) и [URL-адреса](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0&preserve-view=true).

### <a name="users"></a>Пользователи
[Повторная обработка](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0&preserve-view=true) всех назначений лицензий на основе группы для [пользователя](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).


## <a name="february-2020-new-in-preview-only"></a>Февраль 2020: новое только в предварительном просмотре

### <a name="calendar"></a>Календарь
Просмотрите [задачи, поддерживаемые API-интерфейсами предварительного просмотра, которые управляют совместным использованием и делегированием календаря](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Коммуникации из облака

- Используйте новую [запись вызова ](/graph/api/resources/callrecord?view=graph-rest-beta&preserve-view=true) ресурс, чтобы получить метаданные звонков и собрания по сети в Microsoft Teams и Skype для бизнеса в Организации.
- Для участника собрания используйте свойство **инициатора**, чтобы получить идентификационную информацию инициатора [записи](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true), если таковая имеется.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [Февраль](changelog.md#february-2020)

### <a name="groups"></a>Группы
Используйте метод [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true), чтобы назначить лицензии для продуктов, таких как Microsoft 365 или Enterprise Mobility + Security, группе. Поскольку Azure AD обеспечивает назначение лицензий членам группы, для участников, вступающих в группу или покидающих ее, больше не требуется управление лицензиями на индивидуальном уровне.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Установите параметры запроса, утверждения и проверки при создании [политики назначения пакетов доступа](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true).
- Получите доступ к определенным типам [политик для организации](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true), используя `/policies`сегмент URL и указав тип политики. Например, организация может применить политику для автоматического выхода пользователя из веб-сеанса после периода бездействия; см. операции CRUD для экземпляров [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta&preserve-view=true). Это [серьезное изменение](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/), упрощающее обнаружение всех политик путем группировки всех типизированных политик в сегменте `/policies`. Доступ к другим типизированным политикам осуществляется аналогичным образом: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta&preserve-view=true) и [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta&preserve-view=true). 
- Используйте уровень приложения и делегированное `Policy.ReadWrite.ApplicationConfiguration`разрешение для операций чтения и записи в [политиках](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) конфигурации приложений, упомянутых в предыдущем пункте.

### <a name="teamwork"></a>Командная работа
- Используйте [уведомления об изменениях,](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true) всех сообщений канала или всех сообщений в Организации.
- [Отклоните](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta&preserve-view=true) [запрос на замену смен](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta&preserve-view=true) другим пользователем в [группе](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).

## <a name="january-2020-new-and-generally-available"></a>Январь 2020 г.: новые и общедоступные возможности

### <a name="security"></a>Безопасность
В рамках управления оповещениями используйте метод [обновления оповещений](/graph/api/alert-update?view=graph-rest-1.0&preserve-view=true) и обновляйте поле **комментариев** как `Closed in IPC` или `Closed in MCAS`.

### <a name="teamwork"></a>Командная работа
Используйте свойство навигации **primaryChannel** [группы](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) для доступа к каналу по умолчанию **General**.

### <a name="users"></a>Пользователи
Чтобы получить доступ к одному или нескольким удостоверениям, которые [пользователь](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true) может использовать для входа в учетную запись пользователя Azure AD, используйте свойство **удостоверения**. Удостоверения могут предоставляться поставщиками услуг Майкрософт, организаций или социальных удостоверений, таких как Facebook, Google или Microsoft. Это свойство позволяет пользователю входить в учетную запись пользователя с помощью любого из этих удостоверений.

## <a name="january-2020-new-in-preview"></a>Январь 2020: Новое в предварительной версии

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [Январь](changelog.md#january-2020).


## <a name="december-2019-new-and-generally-available"></a>Декабрь 2019 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Коммуникации из облака
API коммуникаций из облака имеет общедоступное состояние, API ресурсов [call](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) и [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-1.0&preserve-view=true) [доступны в версии 1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0&preserve-view=true).

### <a name="education"></a>Образование
Используйте свойство **classSettings**, чтобы управлять параметрами для конкретного класса, например включением отправки еженедельных дайджестов заданий.  Это свойство доступно в ресурсе [team](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true), когда команда представляет собой [группу обучения](/graph/api/resources/educationclass?view=graph-rest-1.0&preserve-view=true).

### <a name="identity-and-access"></a>Удостоверение и доступ 
[При попытке получить объекты-контейнеры с ограниченными разрешениями часть данных возвращается](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects). В качестве примера можно привести экземпляр [группы](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true), связанный с [пользователем](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), другую **группу** и [устройство](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true). Приложение, у которого есть только разрешения User.Read.All и Group.Read.All, при попытке получить доступ к этому экземпляру **группы** получит объекты **user** и **group**, а также ограниченные данные для объекта **device** (только тип данных и ИД объекта), не включающие значения свойств.

### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика
API аналитики имеет общедоступное состояние. Используйте этот API в рабочих приложениях для определения наиболее релевантных документов, которые:

- [касаются](/graph/api/insights-list-trending?view=graph-rest-1.0&preserve-view=true) пользователя;
- [используются](/graph/api/insights-list-used?view=graph-rest-1.0&preserve-view=true) пользователем;
- [к которым предоставлен доступ](/graph/api/insights-list-shared?view=graph-rest-1.0&preserve-view=true) пользователю или пользователем.

### <a name="reports"></a>Отчеты
Чтобы получать отчеты об использовании Microsoft 365 с помощью разрешений, делегированных пользователем, администраторам необходимо назначить пользователю роль администратора Azure AD с ограниченными правами. Это может быть одна из следующих ролей: администратор организации, администратор Exchange, администратор SharePoint, администратор Lync, глобальный читатель или читатель отчетов. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](reportroot-authorization.md).

### <a name="toolkit"></a>Набор средств
Выпущен набор средств Microsoft Graph версии 1.1. Список улучшений и исправлений ошибок см. в [разделе за декабрь 2019 г.](changelog.md#december-2019) журнала изменений.

## <a name="december-2019-new-in-preview"></a>Декабрь 2019 г.: новые возможности в предварительной версии

### <a name="cloud-communications"></a>Коммуникации из облака
- Чтобы получить сведения о доступности и текущей активности одного или нескольких пользователей, используйте новый ресурс [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true).
- [Удалите](/graph/api/onlinemeeting-delete?view=graph-rest-beta&preserve-view=true) экземпляр [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).
- Ознакомьтесь с [разделом за декабрь 2019 г.](changelog.md#december-2019) журнала изменений, чтобы переименовать или удалить несколько элементов ресурсов [call](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) и [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) и обеспечить соответствие версии v1 этих ресурсов.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [декабрь](changelog.md#december-2019)

### <a name="identity-and-access"></a>Удостоверение и доступ 
- Исправлено поведение отношений **appRoleAssignments** и **appRoleAssignedTo** в [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Используйте [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true) в [функции управления правами в Azure AD](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) для запроса добавления ресурса к [каталогу](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true), чтобы роли этого ресурса можно было использовать в [пакете для доступа](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true).
- Используйте [API оценки угроз](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta&preserve-view=true), чтобы дать администраторам возможность сообщать о подозрительной почте, URL-адресах фишинга, вложениях электронной почты и других файлах. Вывод, сделанный при сканировании потока, может побудить их изменить политику организации соответствующим образом.

### <a name="teamwork"></a>Командная работа
- [Настройка уведомлений об изменениях, включающих данные](webhooks-with-resource-data.md) для ресурсов [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) в каналах и чатах Microsoft Teams.
- [Подписка на уведомления](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) о новых и измененных [сообщениях канала или чата](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true).
- Используйте ресурс [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta&preserve-view=true), чтобы включить указание доступности пользователя для назначения смен в [графике](/graph/api/resources/schedule?view=graph-rest-beta&preserve-view=true). Настройте эту возможность в [параметрах](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) пользователя.


## <a name="november-2019-new-and-generally-available"></a>Ноябрь 2019 г.: новые и общедоступные возможности

### <a name="groups"></a>Группы
- Использование разрешений приложения или делегированных разрешений GroupMember.Read.All и GroupMember.ReadWrite.All для перечисления групп, чтения основных свойств групп, считывания (и обновления при наличии разрешения на чтение и запись) сведений об участии в группах, к которым у приложения есть доступ.
- Использование разрешения приложения Group.Create для создания групп без необходимости входа пользователя.
- Для указанной [группы](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) [проверка участия](/graph/api/group-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) в других группах или ролях каталога.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Регистрация [приложений](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true), проходящих проверку подлинности в Azure Active Directory (Azure AD). Используйте делегированные [разрешения](./permissions-reference.md#application-resource-permissions), Application.Read.All и Application.ReadWrite.All, или разрешение приложения, Application.Read.All.
- Для указанного [устройства](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true) [проверка участия](/graph/api/device-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) в других группах или ролях каталога.

### <a name="mail"></a>Почта
- Использование свойства **conversationIndex** для получения положения сообщения в беседе электронной почты Outlook.
- Использование делегированного разрешения Mail.ReadBasic и разрешения приложения Mail.ReadBasic.All, чтобы получить ресурсы [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) или [mail folder](/graph/api/resources/mailfolder?view=graph-rest-1.0&preserve-view=true), отслеживать их изменения, а также управлять [подпиской](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) на уведомления об изменениях сообщений.

### <a name="users"></a>Пользователи
- [Проверка участия в группах](/graph/api/user-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) для определенного [пользователя](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).
- Использование свойства **creationType**, чтобы узнать, как была создана учетная запись пользователя, например была ли она создана в качестве обычной учебной или рабочей учетной записи либо в качестве внешней учетной записи и т. д.

## <a name="november-2019-new-in-preview"></a>Ноябрь 2019 г.: новые возможности в предварительной версии

### <a name="calendar"></a>Календарь
- [Организация и посещение собраний по сети с помощью Outlook](outlook-calendar-online-meetings.md).
- [Настройка свойств](/graph/api/place-update?view=graph-rest-beta&preserve-view=true) для расширенных типов расположений [комната](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) и [список комнат](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communication"></a>Облачное взаимодействие
Тип ресурса [call](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) поддерживает следующие дополнительные функции:

- [Контекст входящего звонка](/graph/api/resources/incomingcontext?view=graph-rest-beta&preserve-view=true)
- Тип конечной точки для участника, например голосовая почта или Skype для бизнеса
- Возможность [обновления](/graph/api/call-updaterecordingstatus?view=graph-rest-beta&preserve-view=true) [сведений о записи](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true) для [участника](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true)

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [ноябрь](changelog.md#november-2019)

### <a name="education"></a>Образование
Администраторы могут включать параметры на уровне класса с помощью свойства **classSettings** [команды](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), связанной с [классом](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true). В настоящее время существует параметр для уведомления опекунов о еженедельных заданиях.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Использование разрешения приложения Policy.Read.All для чтения всех политик условного доступа и именованных расположений организации без необходимости входа пользователя.
- Поддержка для [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) состояния только для отчета `enabledForReportingButNotEnforced`.
- Использование делегированного разрешения ThreatAssessment.ReadWrite.All или разрешения приложения ThreatAssessment.Read.All для чтения (или создания при наличии разрешения на чтение и запись) запросов на оценку угроз в организации.

### <a name="mail"></a>Почта
Использование делегированного разрешения Mail.ReadBasic и разрешения приложения Mail.ReadBasic.All, чтобы управлять [подписками](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) на уведомления об изменениях в ресурсе [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true).

### <a name="notifications"></a>Уведомления
Можно использовать новые компактные [веб-SDK](https://aka.ms/GNSDK) уведомлений вместо [SDK Project Rome](https://github.com/Microsoft/project-rome), чтобы воспользоваться улучшенной моделью проверки подлинности и поддержкой веб-приложений с push-уведомлениями. 

### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика
Первое появление ресурса [профиль](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true), который является расширенным представлением нового поколения записей людей в службах Майкрософт. Этот ресурс связан с распространенными и удобными атрибутами людей, включая информацию о всех важных датах, таких как [годовщины](/graph/api/resources/personanniversary?view=graph-rest-beta&preserve-view=true), а также об [образовании](/graph/api/resources/educationalactivity?view=graph-rest-beta&preserve-view=true), [должностях](/graph/api/resources/workposition?view=graph-rest-beta&preserve-view=true) и [интересах](/graph/api/resources/personinterest?view=graph-rest-beta&preserve-view=true), уровнях владения [языками](/graph/api/resources/languageproficiency?view=graph-rest-beta&preserve-view=true) и [навыками](/graph/api/resources/skillproficiency?view=graph-rest-beta&preserve-view=true), об [участии в проектах](/graph/api/resources/projectparticipation?view=graph-rest-beta&preserve-view=true) и [связи с веб-сайтами](/graph/api/resources/personwebsite?view=graph-rest-beta&preserve-view=true), а также прочие сведения об [учетной записи](/graph/api/resources/useraccountinformation?view=graph-rest-beta&preserve-view=true) и контактные данные.

### <a name="search"></a>Поиск
Первое появление [API Microsoft Search](search-concept-overview.md), с помощью которого пользователи приложений могут получать индивидуально адаптированные, более актуальные и релевантные результаты поиска с использованием возможностей Microsoft Graph. Можно использовать функцию [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true), которая по умолчанию выполняет поиск в сообщениях и событиях Outlook, а также в файлах OneDrive и SharePoint в облаке Майкрософт. Можно использовать [соединители](/microsoftsearch/connectors-overview), доступные в [коллекции соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы задействовать поисковые данные за пределами облака Майкрософт. Также можно [создавать собственные соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), индексировать внешние настраиваемые элементы и файлы, а также отправлять запросы к определенным внешним источникам данных.

### <a name="teamwork"></a>Командная работа
Получение ресурсов [file](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true), связанных с [командой](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) и [каналом](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), с помощью следующего синтаксиса HTTP-запроса:

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>Пользователи
Использование свойства **creationType**, чтобы узнать, как была создана учетная запись пользователя, например была ли она создана в качестве обычной учебной или рабочей учетной записи либо в качестве внешней учетной записи и т. д.


## <a name="october-2019-new-and-generally-available"></a>Октябрь 2019 г.: новые и общедоступные возможности

### <a name="identity-and-access"></a>Идентификация и доступ
- Использование [контактов организации](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true) в рабочих приложениях. Контакты организации находятся под управлением администраторов организации и синхронизируются из локальной службы каталогов Active Directory или из Exchange Online.
- Настройка [проверки подлинности на основе сертификатов](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) в [организации](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true).
- Добавление и удаление [учетных данных с паролем](/graph/api/resources/passwordcredential?view=graph-rest-1.0&preserve-view=true) для [приложений](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true).

### <a name="mail"></a>Почта
Использование нового параметра **message** для обновления любых записываемых свойств [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) при [ответе](/graph/api/message-reply?view=graph-rest-1.0&preserve-view=true) на сообщение, например [для добавления получателя в ответ](/graph/api/message-reply#example?view=graph-rest-1.0&preserve-view=true).

### <a name="microsoft-graph-data-connect"></a>Подключение к данным Microsoft Graph
Разработчики и исследователи данных теперь могут использовать [инструменты для преобразования данных Office 365 в формат общей модели данных](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md). В этом случае обеспечивается согласование схемы данных с другими наборами данных, совместимыми с Open Data Initiative (ODI). 


### <a name="microsoft-graph-sdks"></a>Пакеты SDK Microsoft Graph
- Использование обработчиков хаоса в SDK JavaScript для проверки устойчивости приложения к сбоям серверов, возникающим в трудновоспроизводимых условиях.
- Прочтите о [создании вызовов API с помощью пакетов SDK](./sdks/create-requests.md).

### <a name="users"></a>Пользователи
- [Получение](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0&preserve-view=true) или [настройка](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0&preserve-view=true) параметров предпочитаемого пользователем формата даты и времени [для почтового ящика пользователя](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true). 
- Отслеживание даты и времени последнего изменения пароля [пользователя](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).

## <a name="october-2019-new-in-preview"></a>Октябрь 2019 г.: новые возможности в предварительной версии

### <a name="calendar"></a>Календарь
- Организаторы собраний могут [разрешить приглашенным предлагать другое время собраний](outlook-calendar-meeting-proposals.md). При получении ответа на приглашение, содержащего предложение другого времени, организатор может принять предложение и [обновить](/graph/api/event-update?view=graph-rest-beta&preserve-view=true) время собрания.
- Программное предоставление доступа к календарю с более тесным взаимодействием с использованием пользовательского интерфейса Outlook. Поддерживается отслеживание разрешений текущего пользователя и состояния общего доступа к календарю, а также следующие возможности:
  - Для каждого [календаря](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true) теперь можно управлять [разрешениями](/graph/api/resources/calendarpermission?view=graph-rest-beta&preserve-view=true) каждого пользователя, которому предоставлен доступ к календарю. 
  - Для каждого [почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) теперь можно указать, кто получает сообщения о собраниях и ответы на эти сообщения: делегат, владелец почтового ящика или и тот, и другой. 
- Дополнительная поддержка собраний по сети:
  - В каждом **календаре** можно указать разрешенных и используемых по умолчанию поставщиков собраний по сети.
  - Можно создать или обновить [мероприятие](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true), доступное по сети, и предоставить участникам сведения для присоединения к собранию по сети. 
  - В частности, можно использовать **onlineMeetingProvider** и **onlineMeeting** — это новые свойства **мероприятий**, с помощью которых можно задать или указать Microsoft Teams в качестве поставщика собраний по сети. Это временное решение [известной проблемы](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) со свойством **onlineMeetingUrl**.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [октябрь](changelog.md#october-2019)

### <a name="graph-explorer"></a>Песочница Graph
Попробуйте [следующую версию песочницы Graph](https://developer.microsoft.com/graph/graph-explorer/preview) и воспользуйтесь полезной контекстной информацией, включая разрешения, маркеры доступа и фрагменты кода SDK, на новых вкладках **Разрешения**, **Проверка подлинности** и **Фрагменты кода**. С помощью ползунка **просмотра** можно переключаться между [рабочей](https://developer.microsoft.com/graph/graph-explorer) и новой предварительной версией песочницы Graph.

### <a name="groups"></a>Группы
- Управление видимостью [групп](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) в определенных частях пользовательского интерфейса Outlook или в клиенте Outlook с помощью свойств **hideFromAddressLists** и **hideFromOutlookClients**.
- [Назначение](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) и удаление лицензий пользователям в [группе](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Идентификация и доступ
- Использование [политик условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) для настройки правил доступа для организации. Эти правила учитывают сигналы о пользователях или об удостоверениях устройств, включая членство пользователей или групп, расположение IP-адреса, а также поведение, включая попытки доступа к определенным приложениям и опасное поведение при входе.
- [Управление правами](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) можно использовать для управления доступом к группам, приложениям и сайтам SharePoint Online для пользователей внутри организации и вне ее.
- Добавление и удаление [учетных данных с паролем](/graph/api/resources/passwordcredential?view=graph-rest-beta&preserve-view=true) для [приложений](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) и [субъектов-служб](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Управление [ключами политики инфраструктуры доверия](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta&preserve-view=true) Azure AD B2C.
- Можно определить политики [пользовательского процесса](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true) Azure AD B2C для входа, регистрации, объединенной процедуры регистрации и входа, сброса пароля и обновления профиля.
- Настройка [меток защиты информации](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta&preserve-view=true), чтобы классифицировать конфиденциальность данных для пользователя или клиента.
- Существующие приложения, использующие API для [событий с риском для идентификации](/graph/api/resources/identityriskevent?view=graph-rest-beta&preserve-view=true), должны перейти на использование функций [обнаружения риска](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) в службе защиты идентификации Azure AD. Дополнительные сведения и график прекращения использования прежнего решения см. в [публикации в блоге](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/).


### <a name="mail"></a>Почта
[Вложение больших файлов размером до 150 МБ](outlook-large-attachments.md) в экземпляр [сообщения](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) путем создания [сеанса отправки](/graph/api/resources/uploadsession?view=graph-rest-beta&preserve-view=true) и итерационной отправки диапазонов файла, пока не отправятся все байты файла. 

### <a name="microsoft-graph-security-api"></a>Microsoft Graph Security API
- Предварительная версия интеграции с RSA NetWitness, ServiceNow и Splunk для сопоставления и синхронизации [оповещений](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#alerts), улучшения защиты от угроз и реагирования.
- Новые переключатели добавлены в [соединитель безопасности Microsoft Graph](/connectors/microsoftgraphsecurity/) и в [сборники схем](/azure/security-center/security-center-playbooks) для логических приложений и потоков. См. [примеры сборников схем](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Поддержка отправки [индикаторов угроз](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#threat-indicators-preview) в Microsoft Defender ATP для блокирования или отправки оповещений об угрозах с использованием собственных источников аналитики. Интеграция с партнерами, такими как ThreatConnect, дает заказчикам возможность отправлять индикаторы непосредственно из решений аналитики угроз и автоматизации. 

### <a name="notifications"></a>Уведомления
- [Создание и отправка уведомлений](/graph/api/user-post-notifications?view=graph-rest-beta&preserve-view=true) всем клиентам приложения во всех конечных точках устройств, где пользователи могли войти в систему, без необходимости управлять разрешениями, делегированными пользователями.
- [Целевые конечные точки политики](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta&preserve-view=true) в [уведомлениях](/graph/api/resources/notification?view=graph-rest-beta&preserve-view=true) пользователей позволяют целенаправленно управлять уведомлениями на платформах Windows, iOS, Android или WebPush.
- Можно указать [политику отката](/graph/api/resources/fallbackpolicy?view=graph-rest-beta&preserve-view=true) для уведомлений для конечных точек iOS, чтобы отправлять высокоприоритетные необработанные уведомления, доставка которых на устройства другими способами может быть невозможной из-за ограничений, действующих для конкретной платформы, например, из-за использования режима экономии заряда аккумулятора.

 
### <a name="powershell-sdk"></a>Пакет SDK для PowerShell 
Разработчики и ИТ-специалисты могут обратить внимание на выпуск [пакета SDK Microsoft Graph для Powershell](https://github.com/microsoftgraph/msgraph-sdk-powershell). Этот пакет будет формировать модули, содержащие командлеты для создания запросов API REST Microsoft.

## <a name="september-2019-new-and-generally-available"></a>Сентябрь 2019 г.: новые и общедоступные возможности

### <a name="calendar-mail-and-group"></a>Календарь, почта и группа
[Получение необработанного содержимого файла или содержимого MIME элемента](/graph/api/attachment-get?view=graph-rest-1.0&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment), добавленного в качестве [вложения](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true) в [событие](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), [сообщение](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) или [запись](/graph/api/resources/post?view=graph-rest-1.0&preserve-view=true) группы.

### <a name="calendar-mail-outlook-task-personal-contact"></a>Календарь, почта, задача Outlook, личный контакт
Преобразование идентификатора элемента Outlook в поддерживаемые [форматы](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true#exchangeidformat-values), включая стандартный и неизменяемый формат идентификаторов Microsoft Graph, с помощью функции [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true). 

Преобразование формата идентификатора поддерживают следующие ресурсы:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true)
- [contact](/graph/api/resources/contact?view=graph-rest-1.0&preserve-view=true)
- [event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0&preserve-view=true)
- [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0&preserve-view=true)

### <a name="mail"></a>Почта
[Получение содержимого MIME сообщения](outlook-get-mime-message.md)

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
Использование [набора средств Microsoft Graph](toolkit/overview.md) с целью разработки приложений для рабочей среды, обеспечивающих согласованный внешний вид и функции Microsoft 365, и экономии времени при проверке подлинности и доступе к данным из Microsoft Graph.

## <a name="september-2019-new-in-preview"></a>Сентябрь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [сентябрь](changelog.md#september-2019)

### <a name="files"></a>Файлы
- Улучшенная поддержка синхронизации:

  - Определение операций, которые могут влиять на двоичное содержимое объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true), с помощью нового свойства **pendingOperations**.
  - [Восстановление](/graph/api/driveitem-restore?view=graph-rest-beta&preserve-view=true) удаленного объекта **driveItem**. 
- Использование защищенного алгоритма хэширования (SHA-256) для улучшения безопасности и целостности данных ресурса [file](/graph/api/resources/file?view=graph-rest-beta&preserve-view=true).
- Получение или настройка ориентации ресурса [photo](/graph/api/resources/photo?view=graph-rest-beta&preserve-view=true). Настройка поддерживается в OneDrive персональный.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Использование нового свойства **identities** и получение удостоверений, которые может применять [пользователь](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) для входа в учетную запись. Удостоверения могут предоставляться организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт.
- Добавочные улучшения для [синхронизации удостоверений](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) в облачном приложении для клиента:

  - Сохранение параметров для [задания синхронизации](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta&preserve-view=true)
  - Указание причины применения [карантина](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta&preserve-view=true) для задания синхронизации

### <a name="teamwork"></a>Командная работа
Использование канала **Общий** в [команде](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) или настройка [параметров участников](/graph/api/resources/teammembersettings?view=graph-rest-beta&preserve-view=true), чтобы разрешить участникам команд создавать закрытые каналы в **команде**.

### <a name="users"></a>Пользователи
- Получение или обновление удостоверений, с помощью которых [пользователь](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) может войти в учетную запись. Эти удостоверения могут предоставляться бизнес-организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт.
- Получение или обновление параметров предпочитаемого пользователем формата даты и времени [для почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true).


## <a name="august-2019-new-and-generally-available"></a>Август 2019 г.: новые и общедоступные возможности 

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0&preserve-view=true) касательно числа и размера удаленных элементов.
- Отслеживайте идентификаторы групп Microsoft 365 при [получении сведений о действиях групп](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0&preserve-view=true).
- Отслеживайте имя субъекта-владельца при получении [сведений об использовании хранилища OneDrive учетной записью](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0&preserve-view=true) и [сведений об использовании сайта SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0&preserve-view=true).
- Узнайте число активных и неактивных пользователей в Microsoft 365 при [получении отчета о количестве пользователей в отдельных службах Microsoft 365](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0&preserve-view=true).

### <a name="security"></a>Безопасность
- Используйте новую [надстройку Microsoft Graph Security API для Splunk](https://aka.ms/graphsecuritysplunkaddon), чтобы передавать оповещения системы безопасности и аналитику из различных продуктов партнеров в Splunk, облегчая сопоставление их данных по безопасности в режиме реального времени. Дополнительные сведения см. в [объявлении](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972). 
- [Ознакомьтесь со списком других решений и соединителей](security-integration.md), разработанных корпорацией Майкрософт или партнерами Майкрософт, которые подключаются к API безопасности и позволяют работать с данными в едином формате.


## <a name="august-2019-new-in-preview"></a>Август 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [август](changelog.md#august-2019)

### <a name="education"></a>Образование
- Свяжите [преподавателя](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true) или [задание](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) с [рубрикой оценивания](/graph/api/resources/educationrubric?view=graph-rest-beta&preserve-view=true), чтобы задать определенные показатели качества и уровни заданий. К примерам показателей качеств относятся орфография и грамматика, а к примерам уровней — "хорошо" и "неудовлетворительно". Кроме того, вы можете связать с рубрикой баллы и веса. Дополнительные сведения см. в [обзоре образовательных рубрик](education-rubric-overview.md).
- Оцените задание и представьте результаты в виде [отзыва](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta&preserve-view=true), [числовой оценки](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta&preserve-view=true) или [рубрики](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta&preserve-view=true).

### <a name="files"></a>Файлы
До этого момента вы могли [отслеживать](/graph/api/driveitem-follow?view=graph-rest-beta&preserve-view=true) объект [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) для удобного доступа или упрощения таких действий, как перемещение, копирование и сохранение в определенном формате. Теперь вы можете использовать действие [отмены отслеживания](/graph/api/driveitem-unfollow?view=graph-rest-beta&preserve-view=true), чтобы прекратить отслеживание таких элементов диска.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Поставщики управления доступом на основе ролей (RBAC) могут [управлять ролями](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) в Azure Active Directory, [определяя действия ролей](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true), которые могут выполняться с определенными ресурсами, и [назначая роли](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta&preserve-view=true) пользователям в соответствии с этими определениями, чтобы предоставить им доступ к этим ресурсам.
- Администраторы могут [просматривать обзоры доступа](/graph/api/accessreview-list?view=graph-rest-beta&preserve-view=true), чтобы эффективно проверять членство в группах, доступ к корпоративным приложениям и назначения ролей. Регулярные проверки доступа позволяют гарантировать, что только уполномоченные люди получают постоянный доступ к ресурсам определенными способами.

### <a name="social-and-workplace-intelligence"></a>Социальная и рабочая аналитика
Пользователи могли использовать приложение [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) Microsoft 365 для получения аналитических сведений о распределении рабочего времени, совместной работе и балансе между трудовой и личной жизнью. Теперь с помощью [API аналитики](/graph/api/resources/social-overview?view=graph-rest-beta&preserve-view=true#help-users-gain-insights-into-their-work-patterns) можно интегрировать данные о времени, потраченном на рабочие задачи (например, звонки, чаты и электронную почту), чтобы повысить продуктивность пользователя и улучшить его самочувствие. 


## <a name="july-2019-new-and-generally-available"></a>Июль 2019 г.: новые и общедоступные возможности 

### <a name="example-code-snippets"></a>Примеры фрагментов кода
Теперь имеются фрагменты кода Objective-C для всех статей по API в справочных материалах для версии 1.0 и бета-версии. См. пример Objective-C для [получения события](/graph/api/event-get?view=graph-rest-1.0&preserve-view=true&tabs=objective-c#example).

### <a name="group"></a>Группа
- Используйте функцию [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0&preserve-view=true), чтобы отображаемое имя или почтовый псевдоним существующей группы Microsoft 365 соответствовали политикам именования.
- Кроме того, перед созданием группы вы можете использовать функцию [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0&preserve-view=true) для объекта [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0&preserve-view=true), чтобы сначала проверить имена.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-1.0&preserve-view=true).
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#role-management-permissions) _RoleManagement.Read.Directory_ и _RoleManagement.ReadWrite.Directory_ для управления доступом на основе ролей (RBAC) в каталоге компании:

  - Используйте разрешение на чтение и запись, чтобы сначала [активировать](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0&preserve-view=true) роль каталога. 
  - Если роль активирована, вы можете использовать разрешение на чтение для [чтения ролей каталога](/graph/api/directoryrole-list?view=graph-rest-1.0&preserve-view=true), [перечисления участников ролей](/graph/api/directoryrole-list-members?view=graph-rest-1.0&preserve-view=true) и [перечисления шаблонов для ролей каталогов](/graph/api/directoryroletemplate-list?view=graph-rest-1.0&preserve-view=true). 
  - Вы также можете использовать разрешение на чтение и запись для [добавления](/graph/api/directoryrole-post-members?view=graph-rest-1.0&preserve-view=true) и [удаления](/graph/api/directoryrole-delete-member?view=graph-rest-1.0&preserve-view=true) участников ролей.


## <a name="july-2019-new-in-preview"></a>Июль 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="calendar"></a>Календарь 
Используйте новый [API мест](/graph/api/resources/place?view=graph-rest-beta&preserve-view=true), чтобы применять различные типы расположений, например [помещения](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) и [список помещений](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true), настроенные администраторами Exchange Online.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [июль](changelog.md#july-2019)

### <a name="files"></a>Файлы 
Применяйте дату и время окончания срока действия или пароль при [создании ссылки для общего доступа](/graph/api/driveitem-createlink?view=graph-rest-beta&preserve-view=true) к файлу, папке или другому объекту [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новое разрешение приложений](./permissions-reference.md#access-reviews-permissions) _AccessReview.ReadWrite.Membership_ для операций CRUD при [проверках доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true). 
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#administrative-units-permissions) _AdministrativeUnit.Read.All_ и _AdministrativeUnit.ReadWrite.All_ для чтения и записи (включая создание, обновление и удаление участников, а также управление ими) ресурсов [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true) соответственно.
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-beta&preserve-view=true).
- Используйте новую функцию [обнаружения](/graph/api/directorydefinition-discover?view=graph-rest-beta&preserve-view=true) для поиска последней [схемы синхронизации](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta&preserve-view=true) каталога, чтобы синхронизировать объекты каталога, атрибуты и их типы с приложением.
- Используйте [политику развертывания функций](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta&preserve-view=true), чтобы помочь администраторам клиента выполнить пилотное развертывание функций для определенных групп перед включением их для всей организации.

### <a name="mail"></a>Почта
Используйте более детализированное разрешение приложений _Mail.ReadBasic.All_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Теперь его можно применять в [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) и [отслеживании изменений](delta-query-overview.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) и объекта **mailFolder**.

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta&preserve-view=true) касательно числа и размера удаленных элементов.

### <a name="teamwork"></a>Командная работа
- [Устанавливайте](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [удаляйте](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [обновляйте](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta&preserve-view=true) и [перечисляйте установленные приложения Microsoft Teams](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta&preserve-view=true) для пользователя.
- Используйте доступ только для приложения, чтобы читать сообщения канала, а также отвечать на сообщения в каналах и беседах. [Запросите и получите утверждение](teams-protected-apis.md) для такого доступа.

## <a name="may---june-2019-new-and-generally-available"></a>Май–июнь 2019 г.: новые и общедоступные возможности

### <a name="calendar-mail-and-personal-contacts"></a>Календарь, почта и личные контакты
Администраторы Exchange могут предоставлять приложению разрешения приложения и [ограничить доступ приложения только к подмножеству почтовых ящиков](auth-limit-mailbox-access.md) вместо доступа ко всем почтовым ящикам в организации, используемого по умолчанию. Такое ограничение доступа будет применено ко всем разрешениям приложения, предоставленным приложению для [календарей](permissions-reference.md#calendars-permissions), [контактов](permissions-reference.md#contacts-permissions), а также [параметров почты и почтового ящика](permissions-reference.md#mail-permissions). См. связанное [объявление в блоге](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/).

### <a name="mail"></a>Почта
Используйте API [папок поиска почты](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0&preserve-view=true) для поиска сообщений и доступа к результатам поиска по электронной почте Outlook. См. связанное [объявление в блоге](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/).

### <a name="postman"></a>Postman
В качестве альтернативы песочнице Graph используйте API Microsoft Graph в [коллекции Postman Microsoft Graph](use-postman.md), чтобы изучить поведение API и ускорить разработку приложения.

### <a name="tutorials"></a>Учебники
Воспользуйтесь новым [руководством для создания консольного приложения Java](/graph/tutorials/java), чтобы получить информацию о календаре пользователя.

### <a name="user"></a>Пользователь
Администраторы и пользователи могут [отзывать](/graph/api/user-revokesigninsessions?view=graph-rest-1.0&preserve-view=true) все выданные маркеры обновления для пользователя. Обычно это используется для того, чтобы запретить доступ к данным организации для приложений на потерянных и украденных устройствах.


## <a name="may---june-2019-new-in-preview"></a>Май–июнь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [май](changelog.md#may-2019) 
- Обновления Intune за [июнь](changelog.md#june-2019)

### <a name="education"></a>Образование
- Разностный запрос для [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta&preserve-view=true).
- Разностный запрос и добавления свойств для [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) и [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true).

### <a name="group"></a>Группа
Получите [метки конфиденциальности](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true), чтобы обеспечить защиту конфиденциальных данных группы Microsoft 365 и выполнение политик в отношении соответствия требованиям. Эти метки являются объектами [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true), опубликованными администраторами в Центре безопасности и соответствия требованиям Microsoft 365, в рамках возможностей Microsoft Information Protection. 

### <a name="identity-and-access"></a>Удостоверения и доступ
- Получите экземпляр [приложения](/graph/api/resources/applicationtemplate?view=graph-rest-beta&preserve-view=true) или добавьте экземпляр из коллекции приложений Azure AD в ваш каталог в качестве шаблона.
- Получите журнал всех [событий подготовки](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta&preserve-view=true) каталога в клиенте.
- Получите сведения об [обнаруженном пользователе или рисках входа в систему](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) в среде Azure AD. Эта функциональность обнаружения рисков является частью Azure AD Identity Protection (Защиты идентификации Azure AD).

### <a name="mail"></a>Почта
Используйте более детализированное делегированное разрешение _Mail.ReadBasic_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Доступно для методов чтения [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) и [отслеживания изменений](delta-query-overview.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) и объекта **mailFolder**.

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
[Набор средств Microsoft Graph](./toolkit/overview.md) — это набор не зависящих от платформы веб-компонентов и помощников, обеспечивающий удобную проверку подлинности и доступ к данным в Microsoft Graph.  Так как набор средств Microsoft Graph находится в состоянии предварительной версии, используйте компоненты и поставщиков наборов средств только для тех приложений, которые не предназначены для рабочей среды.

### <a name="reports"></a>Отчеты
- Получайте [отчеты о методах проверки подлинности](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta&preserve-view=true), используемых пользователями в организации, таких как самостоятельное хранение пароля и многофакторная проверка подлинности (MFA).

### <a name="sites"></a>Сайты
Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-beta&preserve-view=true) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-beta&preserve-view=true) сайтов SharePoint. 

### <a name="teamwork"></a>Командная работа
- Размещайте [изображения](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta&preserve-view=true) в [сообщениях в чатах](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) Microsoft Teams.
- Поддерживайте [настройку](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta&preserve-view=true) способа обнаружения закрытой команды.


## <a name="january---april-2019-new-and-generally-available"></a>Январь–апрель 2019 г.: новые и общедоступные возможности

[Подключение к данным Microsoft Graph](data-connect-concept-overview.md)

### <a name="calendar"></a>Календарь
[Получение сведений о доступности](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>Удостоверения и доступ
[Поставщики удостоверений](/graph/api/resources/identityprovider?view=graph-rest-1.0&preserve-view=true)
[Руководство по улучшенной проверке подлинности](./auth/index.yml)
[Миграция приложений из Azure AD Graph в Microsoft Graph](migrate-azure-ad-graph-planning-checklist.md)

### <a name="sdks"></a>Пакеты SDK
[Руководство по пакетам SDK](/sdks/sdks-overview.md) Фрагменты API ([пример](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true&tabs=cs#sdk-sample-code))

### <a name="security"></a>Система безопасности
[Оценка безопасности клиента](/graph/api/resources/securescore?view=graph-rest-1.0&preserve-view=true)

## <a name="january---april-2019-new-in-preview"></a>Январь–апрель 2019 г.: новые возможности в предварительной версии

### <a name="calendar-group-mail-to-do-tasks"></a>Календарь, группа, почта, задачи To-Do
[Получение необработанного контента или содержимого MIME вложений](/graph/api/attachment-get?view=graph-rest-beta&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment) для события, сообщения, задачи Outlook или записи в группе

### <a name="change-notifications"></a>Уведомления об изменениях
[Уменьшение количества пропущенных уведомлений об изменениях](webhooks-lifecycle.md)

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [январь](changelog.md#january-2019) 
- Обновления Intune за [февраль](changelog.md#february-2019)
- Обновления Intune за [март](changelog.md#march-2019)
- Обновления Intune за [апрель](changelog.md#april-2019)

### <a name="files"></a>Файлы
[Приглашение к совместному использованию](/graph/api/driveitem-invite?view=graph-rest-beta&preserve-view=true) включает истечение срока его действия и пароль

### <a name="financials"></a>Финансовые показатели
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>Удостоверения и доступ
[Проверки доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) поддерживают разрешения для приложений [Журналы аудита и входа](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta&preserve-view=true)
[Настраиваемые вход и регистрация в Azure AD B2C](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta&preserve-view=true)
[Рискованный пользователь](/graph/api/resources/riskyuser?view=graph-rest-beta&preserve-view=true) и [журнал](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta&preserve-view=true)

### <a name="mail"></a>Почта
[Получение содержимого MIME сообщений](outlook-get-mime-message.md)

### <a name="reports"></a>Отчеты
[Отчеты о входе в приложение](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta&preserve-view=true)

### <a name="security"></a>Система безопасности
[Действия по обеспечению безопасности](/graph/api/resources/securityaction?view=graph-rest-beta&preserve-view=true)
[Индикаторы угроз](/graph/api/resources/tiindicator?view=graph-rest-beta&preserve-view=true)

### <a name="teamwork"></a>Командная работа
[Личные чаты](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)
[Управление сменами](/graph/api/resources/shift?view=graph-rest-beta&preserve-view=true)

## <a name="see-also"></a>См. также
- Ознакомьтесь [с текущими новыми возможностями](whats-new-overview.md) в Microsoft Graph.
- Периодически просматривайте [блог разработчика, посвященный Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).