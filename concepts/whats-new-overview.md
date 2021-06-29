---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 42beebafd90b752548e6be81963c8c7bc484de39
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162205"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.

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
Настройте уведомление пользователей или участников группы о ходе выполнения [просмотра доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) с помощью свойства **additionalNotificationRecipients** [определения расписания](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

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

## <a name="may-2021-new-and-generally-available"></a>Март 2021 г.: новые и общедоступные возможности

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
Узнайте, когда принтер в последний раз взаимодействовал с функцией универсальной печати, с помощью свойства **lastSeenDateTime** объекта [printer](/graph/api/resources/printer).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверения и доступ | Удостоверения и вход
Получение и обновление ролей гостевых пользователей с помощью свойства **guestUserRoleId** объекта [authorizationPolicy](/graph/api/resources/authorizationpolicy).

### <a name="mail"></a>Почта
- [Создавайте черновики и отправляйте сообщения Outlook в формате MIME](outlook-send-mime-message.md), прикрепляйте цифровые подписи S/MIME и шифруйте содержимое сообщений в S/MIME.
- Создайте [mailFolder](/graph/api/resources/mailfolder) как [скрытую папку](/graph/api/resources/mailfolder#hidden-mail-folders), [задав свойство isHidden](/graph/api/user-post-mailfolders#example).

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph Toolkit
Попробуйте следующие новые функции в Microsoft Graph Toolkit 2.2:
- Компоненты [Файл](/graph/toolkit/components/file) и [Список файлов](/graph/toolkit/components/file-list)
- [Поставщик проверки подлинности MSAL 2.0](/graph/toolkit/providers/msal2)
- [Библиотека SharePoint Framework](/graph/toolkit/get-started/mgt-spfx)

### <a name="reports--azure-ad-activity-reports"></a>Отчеты | Отчеты о действиях Azure AD
Общая доступность API отчетов для [отображения списка](/graph/api/provisioningobjectsummary-list) действий, выполненных службой подготовки Azure AD, и связанных с ней свойств. Предыдущая бета-версия согласована с версией API 1.0.

## <a name="may-2021-new-in-preview-only"></a>Март 2021 г.: новые возможности только в предварительной версии

### <a name="connecting-external-content"></a>Подключение внешнего контента
- При разработке соединителей учитывайте ограничения, связанные с [реализацией и работой](connecting-external-content-api-limits.md).
- Попробуйте [API соединителей с Postman](connecting-external-content-connectors-api-postman.md).

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
Запрос разрешений приложений с минимальными правами, `CloudPC.Read.All` или `CloudPC.ReadWrite.All`, для доступа к методам следующих ресурсов:
  - Операции чтения и записи, а также метод [reprovision](/graph/api/cloudpc-reprovision?view=graph-rest-beta&preserve-view=true) ресурса [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).
  - Операции чтения и записи, а также метод [getSourceImages](/graph/api/cloudpcdeviceimage-getsourceimages?view=graph-rest-beta&preserve-view=true) ресурса [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true).
  - Операции чтения и записи, а также метод [updateAdDomainPassword](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) ресурса [cloudPcOnPremisesConnection](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true).
  - Операции чтения и записи, а также метод [assign](/graph/api/cloudpcprovisioningpolicy-assign?view=graph-rest-beta&preserve-view=true) ресурса [cloudPcProvisioningPolicy](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune за сентябрь для бета-версии. Установите фильтр **Дата** в значение "июнь 2021" и выполните поиск раздела с таким заголовком.

### <a name="education"></a>Образование
- [Настройте папку ресурсов SharePoint](/graph/api/educationAssignment-setupresourcesfolder?view=graph-rest-beta&preserve-view=true) для загрузки и хранения всех файловых ресурсов в одном месте для [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- [Настройте папку ресурсов SharePoint](/graph/api/educationsubmission-setupresourcesfolder?view=graph-rest-beta&preserve-view=true) для загрузки и хранения всех файловых ресурсов, таких как файл Word или Excel, в одном месте для [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Удостоверения и доступ | Управление
- Получите коллекцию ресурсов [accessPackageAssignment](/graph/api/resources/accessPackageAssignment?view=graph-rest-beta&preserve-view=true) путем [фильтрации по пользователю, вошедшему в систему](/graph/api/accesspackageassignment-filterbycurrentuser?view=graph-rest-beta&preserve-view=true).
- Получите коллекцию ресурсов [accessPackageAssignmentRequest](/graph/api/resources/accessPackageAssignmentRequest?view=graph-rest-beta&preserve-view=true) путем [фильтрации по пользователю, вошедшему в систему](/graph/api/accesspackageassignmentrequest-filterbycurrentuser?view=graph-rest-beta&preserve-view=true).

### <a name="use-sdks"></a>Использование пакетов SDK
Попробуйте предварительную версию [пакета SDK Microsoft Graph .NET версии 4](https://www.nuget.org/packages/Microsoft.Graph/4.0.0-preview.4) и воспользуйтесь следующими улучшениями:
- Использование одного API для проверки подлинности в клиентах Microsoft Graph и Azure .NET.
- Новая поддержка сериализации и десериализации JSON.
- Удобный доступ к сведениям откликов.
- Более удобные возможности обновления зависимостей.


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
