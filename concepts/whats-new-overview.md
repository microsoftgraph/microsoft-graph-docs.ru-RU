---
title: Новые возможности Microsoft Graph
description: Прочитайте о самых важных новых возможностях Microsoft Graph за последние два месяца, о том, что было добавлено в более ранних выпусках, и о том, как делиться идеями.
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 57e86b50b14c87a00341a296af38f22669c3651b
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645240"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.

## <a name="june-2022-new-and-generally-available"></a>Июнь 2022 г.: новые и общедоступные возможности

### <a name="cloud-communications--call-records"></a>Облачные коммуникации | Записи звонков
Получение сведений об аудиокодеке, видеокодеке. сетевом транспортном протоколе и прыжках маршрута трассировки для [потока мультимедиа](/graph/api/resources/callrecords-mediastream) при [получении записи звонка](/graph/api/callrecords-callrecord-get) и развертывании каждого [сегмента](/graph/api/resources/callrecords-segment) [сеанса](/graph/api/resources/callrecords-session).

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- [Перечисление административных единиц](/graph/api/device-list-memberOf), в состав которых входит [устройство](/graph/api/resources/device).
- Управление устройствами в качестве участников [административной единицы](/graph/api/resources/administrativeunit): [перечисление участников](/graph/api/administrativeunit-list-members), включая устройства; [получение](/graph/api/administrativeunit-get-members), [добавление](/graph/api/administrativeunit-post-members) и [удаление](/graph/api/administrativeunit-delete-members) устройства в качестве участника. 
- [Получите](/graph/api/application-get) статус и другие сведения о [безопасности и сертификации](/graph/api/resources/certification) [приложения](/graph/api/resources/application) для защиты данных клиентов. Дополнительные сведения см. в разделе [Сертификация Microsoft 365](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).
- Настройка [параметров федерации с Azure AD](/graph/api/resources/internalDomainFederation).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Настройка [параметров политики методов проверки подлинности с временным паролем доступа](/graph/api/resources/temporaryAccessPassAuthenticationMethodConfiguration) в вашем клиенте и управление этими параметрами.
- Получение [базовой политики в каталоге для параметров межтенантного доступа](/graph/api/resources/crosstenantaccesspolicy), [конфигурации по умолчанию](/graph/api/resources/crosstenantaccesspolicyconfigurationdefault) для взаимодействия организации с внешними организациями Azure Active Directory и [конфигурации партнеров](/graph/api/resources/crosstenantaccesspolicyconfigurationpartner) для внешних организаций Azure Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Поиск новых столбцов в отчетах Teams, созданных следующими методами:
  - [getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts);
  - [getTeamsUserActivityUserDetail](/graph/api/reportroot-getTeamsUserActivityUserDetail);
  - [getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getTeamsDeviceUsageUserDetail);
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts);
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts).
- Столбец Windows Phone упразднен в отчетах Teams, созданных следующими методами:
  - [getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts);
  - [getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getTeamsDeviceUsageDistributionUserCounts).

### <a name="teamwork"></a>Teamwork
Подпишитесь на уведомления об изменениях для следующих элементов в Teams:
- [команда и канал](teams-changenotifications-team-and-channel.md)
- [участие в командах и каналах](teams-changenotifications-teammembership.md)
- [chat](teams-changenotifications-chat.md)
- [участие в чате](teams-changenotifications-chatmembership.md)
- [сообщения во всех чатах](/graph/teams-changenotifications-chatmessage#subscribe-to-changes-at-the-user-level), в которых участвует конкретный пользователь.

## <a name="june-2022-new-in-preview-only"></a>Июнь 2022 г.: новые возможности только в предварительной версии

### <a name="applications"></a>Приложения
Указание [связанных объектов](/graph/api/resources/synchronization-synchronizationLinkedObjects?view=graph-rest-beta&preserve-view=true), которые можно [подготовить во время подготовки по запросу](/graph/api/resources/synchronization-synchronizationJobSubject?view=graph-rest-beta&preserve-view=true), включая такие субъекты, как руководитель, участники и владельцы.

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Доступ к [API обнаружения электронных данных](/graph/api/resources/security-ediscoverycase?view=graph-rest-beta&preserve-view=true) теперь осуществляется из пространства имен [security](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true) вместо пространства имен "compliance".

### <a name="customer-booking"></a>Резервирование для пользователей
- Управление языком страницы самостоятельного резервирования [компании](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true) или [службы](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true), предоставляемой компанией.
- Указание в [сведениях клиента](/graph/api/resources/bookingCustomerInformation?view=graph-rest-beta&preserve-view=true), включены ли SMS-уведомления для [встречи](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true) клиента.
- Указание, включено ли анонимное присоединение для [службы](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true) и нужно ли создавать URL-адрес анонимного присоединения для встречи с целью обслуживания.
- Разграничение роли [сотрудника](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) в качестве планировщика или участника.
- Указание, следует ли уведомлять [сотрудника](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) по электронной почте при назначении или обновлении резервирования для участника.

### <a name="device-and-app-management--cloud-pc"></a>Управление устройствами и приложениями | Облачный компьютер
Получение следующих сведений о [политике подготовки](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true) облачных компьютеров.
- Имя группы, в которой находятся облачные компьютеры.
- Количество часов ожидания перед повторной подготовкой или отменой подготовки.
- Включен ли локальный администратор (например, конечный пользователь облачного компьютера).
- Служба, управляющая сетевым подключением Azure, которой в настоящее время является Windows 365 или Пространство для разработки Microsoft.

### <a name="device-and-app-management--multi-tenant-management"></a>Управление устройствами и приложениями | Управление несколькими клиентами
[Получите](/graph/api/managedtenants-managedtenant-list-myroles?view=graph-rest-beta&preserve-view=true) набор [ролей, назначенных пользователю, вошедшему в ](/graph/api/resources/managedtenants-myRole?view=graph-rest-beta&preserve-view=true)[управляемый клиент](/graph/api/resources/managedtenants-managedTenant?view=graph-rest-beta&preserve-view=true).

### <a name="education"></a>Образование
- [Создание](/graph/api/educationassignment-setupfeedbackresourcesfolder?view=graph-rest-beta&preserve-view=true) папки SharePoint для [задания](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) для отправки документов с отзывами.
- [Создание](/graph/api/educationfeedbackresourceoutcome-post-outcomes?view=graph-rest-beta&preserve-view=true) [документа с отзывами](/graph/api/resources/educationFeedbackResourceOutcome?view=graph-rest-beta&preserve-view=true) для [отправки](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) в папке отзывов, связанной с заданием.

### <a name="groups"></a>Группы
Указание того, настроена ли [группа](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) для [обратной записи](/graph/api/resources/groupWritebackConfiguration?view=graph-rest-beta&preserve-view=true) свойств объекта группы в локальную службу Active Directory.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- [Повышение](/graph/api/domain-promote?view=graph-rest-beta&preserve-view=true) уровня проверенного поддомена до корневого домена.
- [Получите](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) URL-адрес метаданных SAML для объединения одноклиентского [приложения](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Скрытие ссылок самостоятельного сброса пароля (SSPR) в [параметрах видимости текста страницы входа](/graph/api/resources/loginpagetextvisibilitysettings?view=graph-rest-beta&preserve-view=true) для страницы входа клиента.

### <a name="compliance--records-management"></a>Соответствие требованиям | Управление записями
Использование дебютного [API управления записями Microsoft Purview](/graph/api/resources/security-recordsmanagement-overview?view=graph-rest-beta&preserve-view=true), чтобы помочь организациям управлять хранением и удалением данных в соответствии с юридическими обязательствами и нормативами соответствия требованиям.

### <a name="teamwork"></a>Teamwork
Получение сведений о [закреплении](/graph/api/resources/messagePinnedEventMessageDetail?view=graph-rest-beta&preserve-view=true) или [откреплении](/graph/api/resources/messageUnpinnedEventMessageDetail?view=graph-rest-beta&preserve-view=true) [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) в [чате](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) или [канале](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true). 

## <a name="may-2022-new-and-generally-available"></a>Май 2022 г.: новые и общедоступные возможности

### <a name="education"></a>Образование
- [Отслеживание изменений в ресурсах назначения](/graph/api/educationassignment-delta).
- [Отслеживание изменений в ресурсах категории назначения](/graph/api/educationcategory-delta).

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
[Приложение](/graph/api/resources/application), зарегистрированное в Azure Active Directory (Azure AD), может указывать контактные данные приложения или службы из базы данных управления службой или ресурсами.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Разрешите клиенту Azure Active Directory (Azure AD) настроить [федерацию с другой организацией, поставщик удостоверений (IdP) которой поддерживает протокол SAML или WS-Fed](/graph/api/resources/samlOrWsFedExternalDomainFederation). Это позволит клиенту Azure AD предоставить доступ к своим ресурсам гостевым пользователям.

### <a name="search"></a>Поиск
Для [поискового запроса](/graph/api/resources/searchrequest) можно указать до 1000 результатов поиска на странице.

### <a name="sites-and-lists"></a>Сайты и списки
- Получите коллекцию совместимых ресурсов [типа контента](/graph/api/resources/contentType) из концентратора типов контента, совместимых с помощью действия [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes). 
- Добавьте или синхронизируйте тип контента из концентратора типов контента на [сайт](/graph/api/resources/site) или в [список](/graph/api/resources/list) с помощью действия [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub). Это делает тип контента или его обновление доступными для определенного сайта или списка, где это необходимо. Это улучшение по сравнению с устаревшей инфраструктурой синхронизации, которая распространяет тип контента на все сайты в организации, сокращая время ожидания распространения публикации. 
- Получение одной или нескольких [многофункциональных длительных операций](/graph/api/resources/richlongrunningoperation), выполняемых на сайте или в списке, что может происходить при синхронном добавлении типа контента.

### <a name="tasks-and-plans"></a>Задачи и планы
- [Получение](/graph/api/plannerplandetails-get) и [обновление](/graph/api/plannerplandetails-update) описаний категорий в [рамках сведений](/graph/api/resources/plannerplandetails) о [плане](/graph/api/resources/plannerplan).
- Вместо свойства **владельца** **плана** используйте свойство **type** [контейнера плана](/graph/api/resources/plannerplancontainer), чтобы указать правила авторизации и время существования **плана**.
- Получение приоритета [задачи](/graph/api/resources/plannerTask).

### <a name="teamwork"></a>Teamwork
[Получение сообщений в канале](/graph/api/channel-list-messages) и [включение всех ответов](/graph/api/channel-list-messages#example-3-request-with-top-and-expand-query-options-on-replies) в сообщение.

### <a name="to-do-tasks"></a>Задачи To-Do
- Разделите сложную [задачу](/graph/api/resources/todotask) на более выполнимые, маленькие задачи, каждая из которых является [элементом контрольного списка](/graph/api/resources/checklistitem).
- Пометьте задачу [категорией](/graph/api/resources/outlookcategory), определенной пользователем для группирования контактов, событий, сообщений, записей групп и задач Outlook.


## <a name="may-2022-new-in-preview-only"></a>Май 2022 г.: новые возможности только в предварительной версии

### <a name="application"></a>Приложение
При настройке прокси приложения Azure AD для локальных приложений с целью безопасного удаленного доступа используйте свойство **isStateSessionEnabled** в ресурсе [onPremisesPublishing](/graph/api/resources/onPremisesPublishing?view=graph-rest-beta&preserve-view=true), чтобы указать, следует ли проверять параметр состояния, если приложение использует поток предоставления кода авторизации OAuth 2.0. Установка этого свойства помогает администраторам защитить приложение от подделки межсайтовых запросов (CSRF).

### <a name="compliance--subject-rights-requests"></a>Соответствие требованиям | Запросы прав субъектов
- Указание и получение расположений, в которых должен выполняться поиск при [запросе прав субъекта](/graph/api/resources/subjectRightsRequest?view=graph-rest-beta&preserve-view=true), например [почтовые ящики](/graph/api/resources/subjectRightsRequestAllMailboxLocation?view=graph-rest-beta&preserve-view=true), [каналы SharePoint, OneDrive и Teams](/graph/api/resources/subjectRightsRequestAllSiteLocation?view=graph-rest-beta&preserve-view=true).
- Указание и получение запроса KQL контента, который должен использоваться для поиска при запросе прав субъекта.

### <a name="device-and-app-management--cloud-pc"></a>Управление устройствами и приложениями | Облачный компьютер
- Получение четко определенного [результата](/graph/api/resources/cloudpcbulkremoteactionresult?view=graph-rest-beta&preserve-view=true) при [массовой повторной подготовке облачных компьютеров](/graph/api/manageddevice-bulkReprovisionCloudPc?view=graph-rest-beta&preserve-view=true).
- [Получение](/graph/api/manageddevice-getcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true) и [указание](/graph/api/manageddevice-setcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true) [состояния проверки облачного компьютера](/graph/api/resources/cloudpcreviewstatus?view=graph-rest-beta&preserve-view=true) и [массовое задание состояния проверки облачных компьютеров](/graph/api/manageddevice-bulksetcloudpcreviewstatus?view=graph-rest-beta&preserve-view=true) для нескольких устройств.

### <a name="device-and-app-management--multi-tenant-management"></a>Управление устройствами и приложениями | Управление несколькими клиентами
[Получение](/graph/api/managedtenants-managedtenant-list-tenantusage?view=graph-rest-beta&preserve-view=true) количества ежемесячных активных пользователей для каждой службы в управляемом клиенте.

### <a name="education"></a>Образование
Использование ресурса [Teams](/graph/api/resources/educationteamsappresource?view=graph-rest-beta&preserve-view=true), соответствующего установленному приложению Microsoft Teams, чтобы разрешить пользователям образовательных служб создавать задания и делиться заданиями во внедренных приложениях Teams, таких как YouTube или FlipGrid.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Активация службы [для организации](/graph/api/organization-activateService?view=graph-rest-beta&preserve-view=true) и [пользователя](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) устарела и перестанет возвращать данные 30 июня 2022 г.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
В области [роли пользователя по умолчанию](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true) [политики авторизации](/graph/api/resources/authorizationPolicy?view=graph-rest-beta&preserve-view=true) укажите, может ли зарегистрированный владелец устройства считывать собственные ключи восстановления BitLocker.

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
Получите [отчет об использовании зарегистрированных методов проверки подлинности пользователя](/graph/api/resources/userregistrationdetails?view=graph-rest-beta&preserve-view=true), который включает метод многофакторной проверки подлинности по умолчанию.

### <a name="search--index"></a>Поиск | Индекс
[Получение](/graph/api/externalconnectors-connectionquota-get?view=graph-rest-beta&preserve-view=true) [сведений о квоте](/graph/api/resources/externalconnectors-connectionQuota?view=graph-rest-beta&preserve-view=true) для [подключения](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true). Эти сведения включают количество элементов, которые можно принять в подключение, учитывая элементы, остающиеся в подключении, и остающуюся квоту на уровне клиента для всех подключений.

### <a name="sites-and-lists"></a>Сайты и списки
[Отслеживание изменений в ресурсах элементов списка SharePoint](/graph/api/listitem-delta?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Командная работа
- Использование разрешений приложений для [получения всех чатов](/graph/api/chat-list?view=graph-rest-beta&preserve-view=true), в которых участвует указанный пользователь, без необходимости присутствия пользователя.
- [Массовая отправка уведомлений в веб-канале действий нескольким пользователям](/graph/api/teamwork-sendActivityNotificationToRecipients?view=graph-rest-beta&preserve-view=true) (до 100 пользователей одновременно).

### <a name="to-do-tasks"></a>Задачи To-Do
С 31 мая 2022 г. [набор API задач, созданный на основе baseTask](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true), является устаревшим. Этот набор API прекратит возвращать данные 31 августа 2022 г. Вместо этого используйте [набор API задач, созданный на основе todoTask](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true).


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на сайте [сообщества Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/m365-dev-call) к еженедельной видеоконференции сообщества платформы Microsoft 365.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](https://developer.microsoft.com/graph/changelog/).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
