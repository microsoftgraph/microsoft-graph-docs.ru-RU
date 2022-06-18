---
title: Новые возможности Microsoft Graph
description: Прочитайте о самых важных новых возможностях Microsoft Graph за последние два месяца, о том, что было добавлено в более ранних выпусках, и о том, как делиться идеями.
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 33d64635297761f0ac625c4a460e36abba34795e
ms.sourcegitcommit: 8f54d85e8e8b0a1f72d4557d2bb7749b972dd3e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2022
ms.locfileid: "66141618"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.


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

## <a name="april-2022-new-and-generally-available"></a>Апрель 2022 г.: новое и общедоступное

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Использование службы [Privileged Identity Management (PIM)](/graph/api/resources/privilegedidentitymanagementv3-overview) в рабочих приложениях, чтобы контролировать и отслеживать доступ к важным ресурсам в пределах организации, а также управлять им. Доступ предоставляется через привилегированные роли и управление доступом на основе ролей (RBAC). Он может предоставляться пользователям, группам или субъектам-службам. Ресурсы могут находиться в Azure AD, Azure и других облачных службах Майкрософт, таких как Microsoft 365 или Microsoft Intune.

### <a name="search--index"></a>Поиск | Индекс
- Используйте разрешения приложения `ExternalConnection.Read.All` и `ExternalConnection.ReadWrite.All` для чтения и записи всех внешних подключений без присутствия вошедшего в систему пользователя.
- Используйте разрешение приложения `ExternalItem.Read.All` для чтения всех внешних элементов без присутствия вошедшего в систему пользователя.
- Используйте делегированную авторизацию `ExternalConnection.ReadWrite.OwnedBy` для чтения и записи внешних подключений от имени вошедшего в систему пользователя, которому разрешено ваше приложение.
- Используйте делегирование разрешения `ExternalConnection.Read.All` или `ExternalConnection.ReadWrite.All` для чтения или записи всех внешних подключений от имени вошедшего пользователя.
- Используйте делегирование разрешений `ExternalItem.ReadWrite.OwnedBy` для чтения и записи внешних элементов от имени вошедшего в систему пользователя, которому разрешено ваше приложение.
- Используйте делегирование разрешения `ExternalItem.Read.All` или `ExternalItem.ReadWrite.All` для чтения или записи всех внешних элементов от имени вошедшего пользователя.


## <a name="april-2022-new-in-preview-only"></a>Апрель 2022 г.: новые возможности только в предварительной версии

### <a name="customer-bookings"></a>Резервирование для пользователей
- [Получение сведений о доступности](/graph/api/bookingbusiness-getstaffavailability?view=graph-rest-beta&preserve-view=true) ресурсов [staff member](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) в [организации](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true).
- Использование разрешения приложений `Bookings.Read.All` в операциях чтения для ресурсов [business](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true), [staff member](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true), [service](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true), [customer](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true) и [appointment](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true).
- Использование разрешения приложений `BookingsAppointment.ReadWrite.All` для операций чтения и записи ресурсов клиентов и встреч.

### <a name="device-and-app-management--cloud-pc"></a>Управление устройствами и приложениями | Облачный компьютер
- Указание [параметров Windows](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) в составе [ параметров организации облачного компьютера](/graph/api/resources/cloudPcOrganizationSettings?view=graph-rest-beta&preserve-view=true) для клиента.
- [Получите](/graph/api/user-list-cloudpcs?view=graph-rest-beta&preserve-view=true) облачные компьютерные устройства, связанные с вошедшим пользователем.
- [Задать сведения для запуска облачного компьютерного устройства](/graph/api/cloudpc-getcloudpclaunchinfo?view=graph-rest-beta&preserve-view=true) для вошедшего пользователя.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Настройка [параметров федерации](/graph/api/resources/internalDomainFederation?view=graph-rest-beta&preserve-view=true) федеративных доменов в Azure Active Directory.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
[Получение назначений](/graph/api/accesspackageassignment-additionalaccess?view=graph-rest-beta&preserve-view=true), для которых у соответствующего пользователя есть несовместимые пакеты доступа. 

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
Подтверждение того, что событие является [высокорискованным и скомпрометированным](/graph/api/signin-confirmCompromised?view=graph-rest-beta&preserve-view=true) или [безопасным](/graph/api/signin-confirmSafe?view=graph-rest-beta&preserve-view=true) путем его маркировки в соответствующих журналах входа Azure Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
- [Получение общего отчета о распределении](/graph/api/reportroot-getTeamsUserActivityTotalDistributionCounts?view=graph-rest-beta&preserve-view=true) для количества определенных действий Teams за указанный период. Количество действий Teams, включая сообщения чата команды, звонки, собрания, длительность звукового фрагмента, публикацию сообщений и т. д.
- Получение дополнительных типов действий в отчетах, которые [получают сведения о пользователе](/graph/api/reportroot-getTeamsUserActivityUserDetail?view=graph-rest-beta&preserve-view=true), [получают количество действий](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta&preserve-view=true) и [получают общее количество действий](/graph/api/reportroot-getteamsuseractivitytotalcounts?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Командная работа
Предоставление общего доступа к каналу одной или нескольким командам:
- [Перечисление только каналов, к которым предоставлен общий доступ в команде](/graph/api/team-list-incomingchannels?view=graph-rest-beta&preserve-view=true).
- [Перечисление всех каналов в команде](/graph/api/team-list-allchannels?view=graph-rest-beta&preserve-view=true), включая каналы, размещенные в команде, и команды, к которым предоставлен общий доступ в команде.
- [Перечисление участников команды, у которых есть доступ к указанному общему каналу](/graph/api/sharedwithchannelteaminfo-list-allowedmembers?view=graph-rest-beta&preserve-view=true).
- [Удаление канала, к которому предоставлен общий доступ в команде](/graph/api/team-delete-incomingchannel?view=graph-rest-beta&preserve-view=true).
- [Перечисление команд, которым предоставлен общий доступ к указанному каналу](/graph/api/sharedwithchannelteaminfo-list?view=graph-rest-beta&preserve-view=true).
- [Отмена общего доступа к каналу для команды](/graph/api/sharedwithchannelteaminfo-delete?view=graph-rest-beta&preserve-view=true).


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
