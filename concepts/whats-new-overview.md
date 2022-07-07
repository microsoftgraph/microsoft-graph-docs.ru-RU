---
title: Новые возможности Microsoft Graph
description: Прочитайте о самых важных новых возможностях Microsoft Graph за последние два месяца, о том, что было добавлено в более ранних выпусках, и о том, как делиться идеями.
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: e08c148c1898633f07412a94bf94b11e0d650f98
ms.sourcegitcommit: 005e9d483d03ed048611ffd180a92930afff4e42
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66646135"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.

## <a name="july-2022-new-in-preview-only"></a>Июль 2022 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--call"></a>Облачные коммуникации | Вызов
[Присоединение к запланированному вызову](/graph/api/application-post-calls?view=graph-rest-beta&preserve-view=true) с помощью идентификатора или секретного кода для присоединения к собранию.

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
[Создание](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-4-create-an-online-meeting-that-requires-a-passcode) [собрания по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true), для которого требуется секретный код.

### <a name="users"></a>Пользователи
[Получение](/graph/api/user-get?view=graph-rest-beta&preserve-view=true) идентификатора безопасности (SID) пользователя в сценариях Windows.

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

### <a name="compliance--records-management"></a>Соответствие требованиям | Управление записями
Использование дебютного [API управления записями Microsoft Purview](/graph/api/resources/security-recordsmanagement-overview?view=graph-rest-beta&preserve-view=true), чтобы помочь организациям управлять хранением и удалением данных в соответствии с юридическими обязательствами и нормативами соответствия требованиям.

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

### <a name="teamwork"></a>Teamwork
- Получение сведений о [закреплении](/graph/api/resources/messagePinnedEventMessageDetail?view=graph-rest-beta&preserve-view=true) или [откреплении](/graph/api/resources/messageUnpinnedEventMessageDetail?view=graph-rest-beta&preserve-view=true) [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) в [чате](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) или [канале](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true). 
- Благодаря поддержке сценариев экспорта содержимого Teams вы можете [перечислить](/graph/api/teamwork-list-deletedteams?view=graph-rest-beta&preserve-view=true) команды, которые были удалены, и [получить](/graph/api/deletedteam-getallmessages?view=graph-rest-beta&preserve-view=true) приватные чаты, групповые чаты, чаты собраний и сообщения каналов [удаленной команды](/graph/api/resources/deletedTeam?view=graph-rest-beta&preserve-view=true). Дополнительные сведения см. в статье [Экспорт контента с помощью API экспорта Microsoft Teams](/microsoftteams/export-teams-content).


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
