---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 873e6fa03fd02470eb520657573556266de6f2a7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443209"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.

## <a name="july-2021-new-and-generally-available"></a>Июль 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
Поддержка ограничения емкости для количества участников, которое приложение может обрабатывать при [ответе](/graph/api/call-answer) на [вызов](/graph/api/resources/call), в организациях, внедряющих [запись звонков на основе политики Teams](/microsoftteams/teams-recording-policy).

### <a name="users"></a>Пользователи
Позвольте пользователям [менять собственный пароль](/graph/api/user-changepassword) без роли администратора.


## <a name="july-2021-new-in-preview-only"></a>Июль 2021 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
Локальное подключение [проверки работоспособности ](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) может выявлять больше возможных типов ошибок проверки работоспособности.
- Учетная запись облачного ПК не найдена в подразделении (`adJoinCheckComputerObjectAlreadyExists`).
- Объект облачного ПК не найден в Azure AD (`azureAdDeviceSyncCheckDeviceNotFound`).
- Превышено время ожидания с момента проверки синхронизации объекта облачного ПК с Azure AD (`azureAdDeviceSyncCheckLongSyncCircle`). 

Подробные сведения и рекомендуемые действия по исправлению см. в [справочных материалах](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values).

### <a name="devices-and-apps--multi-tenant-management"></a>Устройства и приложения | Управление несколькими клиентами
Дебютный выпуск [Microsoft 365 Lighthouse API](managedtenants-concept-overview.md), который позволяет поставщикам управляемых служб удаленно управлять несколькими пользовательскими клиентами в масштабе для обеспечения соответствия требованиям и обнаружения угроз, а также обеспечивать работоспособное и безопасное состояние устройств клиента.

### <a name="search"></a>Поиск
Используйте [API Поиска (Майкрософт) для получения сведений о людях](search-concept-person.md), наиболее релевантных для пользователя. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. 

### <a name="teamwork"></a>Командная работа
- [Подпишитесь на уведомления об изменениях в ресурсе чата](teams-changenotifications-chat.md).
- [Подпишитесь на уведомления об изменениях пользователей в чате](teams-changenotifications-chatmembership.md), в [канале](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) или в [группе](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) (например, ресурсы [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true)).

## <a name="june-2021-new-and-generally-available"></a>Июнь 2021 г.: новые и общедоступные возможности

### <a name="applications"></a>Приложения
Получение или задание состояния [application](/graph/api/resources/application) или [servicePrincipal](/graph/api/resources/serviceprincipal) с целью указать с помощью свойства **disabledByMicrosoftStatus**, отключила ли корпорация Майкрософт приложение. Среди возможных причин отключения подозрительные, оскорбительные или вредоносные действия, а также нарушение соглашения об использовании служб Майкрософт.

### <a name="change-notifications"></a>Уведомления об изменениях
Продлен максимальный срок подписки до его истечения для следующих ресурсов:
- OneDrive [driveItem](/graph/api/resources/driveitem) и SharePoint [list](/graph/api/resources/list) с 3 до 30 дней.
- [group](/graph/api/resources/group), [user](/graph/api/resources/user) или других ресурсов каталога — с 3 до 29 дней.

### <a name="change-tracking"></a>Отслеживание изменений
Устранено ограничение на отслеживание изменений в некорневых папках в OneDrive для бизнеса и SharePoint.

### <a name="education"></a>Образование
API-интерфейсы для [службы заданий](/graph/api/resources/educationassignment) в образовании теперь общедоступны. 

### <a name="identity-and-access--governance"></a>Удостоверения и доступ | Управление
GA интерфейса API [просмотра доступа](/graph/api/resources/accessreviewsv2-root). Ознакомьтесь с [обзором](accessreviews-overview.md) и инструкциями по [просмотру доступа в группы безопасности](tutorial-accessreviews-securitygroup.md) и [доступа в группы Microsoft 365](tutorial-accessreviews-m365group.md). Обратите внимание на то, что поддержка [предыдущего API просмотра доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) прекращается, и он перестанет возвращать данные в мае 2023 г.


## <a name="june-2021-new-in-preview-only"></a>Июнь 2021 года: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meetings"></a>Облачная коммуникация | Онлайн-собрания
Настройка управления звуком и видео в [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) посредством включения и выключения для участников собрания возможности включать свои камеры и микрофоны с помощью **allowAttendeeToEnableCamera** и **allowAttendeeToEnableMic** соответственно.

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- [Назначение](/graph/api/cloudpcusersetting-assign?view=graph-rest-beta&preserve-view=true) и управление [cloudPcUserSetting](/graph/api/resources/cloudpcusersetting?view=graph-rest-beta&preserve-view=true) для включения параметра локального администратора или самообслуживания для пользователя на облачном ПК. В настоящее время назначения можно осуществлять на уровне группы (пользователи, относящиеся к группе Microsoft 365 или к группе безопасности).
- [Получение](/graph/api/cloudpc-get?view=graph-rest-beta&preserve-view=true) нескольких новых свойств [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true): имен политики подготовки и локального соединения, которое использовалось во время подготовки, а также даты и времени окончания периода отсрочки, до которого производится повторная подготовка или отмена подготовки.
- Поддержка расширенного набора типов состояния и ошибок для [проверки работоспособности](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) или [локальной связи](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true).

### <a name="education"></a>Образование
- Теперь преподаватели при публикации заданий могут выбирать действия календаря по умолчанию. Преподаватели могут управлять действиями календаря заданий с помощью свойства **addToCalendarAction** ресурса [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- Теперь преподаватели при публикации заданий также могут настраивать действия календаря по умолчанию. Преподаватели могут управлять действиями календаря заданий по умолчанию с помощью свойства **addToCalendarAction** ресурса [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true).

### <a name="groups"></a>Группы
Разрешение назначения роли Azure AD [группе](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) при ее создании путем настройки свойства **isAssignableToRole**. Если это свойство настроено, оно обеспечивает удобное управление ролями пользователей. Вместо назначения роли каждому пользователю соответствующим пользователям разрешается присоединиться к группе, и назначение роли группе будет по умолчанию означать присвоение этой роли каждому новому пользователю в ней. 

### <a name="identity-and-access--governance"></a>Удостоверения и доступ | Управление
Настройка уведомлений пользователей или участников группы о ходе выполнения [проверки доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) с помощью свойства **additionalNotificationRecipients** [определения расписания](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверения и доступ | Удостоверения и вход
Добавление фильтра для динамического включения и исключения устройств с использованием свойства **deviceFilter** ресурса [conditionalAccessDevices](/graph/api/resources/conditionalAccessDevices?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Сайты и списки
Создание или получение существующей ссылки [sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta&preserve-view=true) для [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) путем вызова [createLink](/graph/api/listitem-createlink?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Командная работа
- [Получение](/graph/api/chat-get?view=graph-rest-beta&preserve-view=true) непрозрачного URL-адреса для ресурса [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) через свойство **webUrl**.
- [Подписка на уведомления об изменениях ](/graph/webhooks?view=graph-rest-beta&preserve-view=true) ресурса [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) или [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).
- Использование разрешений [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) с API для ресурса [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true), [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-beta&preserve-view=true), [chatMessageHostedContent](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true) или [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).
- Получение списка [выданных разрешений для конкретных ресурсов](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true) для ресурса [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), в котором указаны приложения этой команды и предоставленные этим приложениям разрешения для конкретных ресурсов.
- [Получение](/graph/api/teamsasyncoperation-get?view=graph-rest-beta&preserve-view=true) конкретной [асинхронной операции](/graph/api/resources/teamsasyncoperation?view=graph-rest-beta&preserve-view=true) или [списка](/graph/api/chat-list-operations?view=graph-rest-beta&preserve-view=true) всех асинхронных операций, запущенных для ресурса [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- Можно указать [приложение Teams](/graph/api/resources/teamsapp?view=graph-rest-beta&preserve-view=true) при [создании чата](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true).
- Использование единого действия [provisionEmail](/graph/api/channel-provisionemail?view=graph-rest-beta&preserve-view=true) для получения адреса электронной почты ресурса [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), если таковой существует, или его создания. Использование действия [removeEmail](/graph/api/channel-removeemail?view=graph-rest-beta&preserve-view=true) для удаления адреса электронной почты.

### <a name="teamwork--shifts"></a>Командная работа | Смены
- Поддержка сущностей [offerShiftRequest](/graph/api/resources/offershiftrequest?view=graph-rest-beta&preserve-view=true), [timeOff](/graph/api/resources/timeoff?view=graph-rest-beta&preserve-view=true), [timeOffReason](/graph/api/resources/timeoffreason?view=graph-rest-beta&preserve-view=true) и [timeOffRequest](/graph/api/resources/timeoffrequest?view=graph-rest-beta&preserve-view=true) для синхронных уведомлений об изменениях.
- Поддержка управления ресурсами и распространенными функциями [карточки времени](/graph/api/resources/timecard?view=graph-rest-beta&preserve-view=true), такими как [clock in](/graph/api/timecard-clockin?view=graph-rest-beta&preserve-view=true), [clock out](/graph/api/timecard-clockout?view=graph-rest-beta&preserve-view=true), [start break](/graph/api/timecard-startbreak?view=graph-rest-beta&preserve-view=true), [end break](/graph/api/timecard-endbreak?view=graph-rest-beta&preserve-view=true), [confirm](/graph/api/timecard-confirm?view=graph-rest-beta&preserve-view=true) и [replace](/graph/api/timecard-replace?view=graph-rest-beta&preserve-view=true).


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на сайте [сообщества Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Впервые в состоянии **_предварительной версии_**. Все связанные обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](https://developer.microsoft.com/graph/changelog/).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
