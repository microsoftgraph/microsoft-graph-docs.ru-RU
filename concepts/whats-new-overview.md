---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: f9fb8834895c7b61745dab084c2b1807ef6143dd
ms.sourcegitcommit: 8f156a80b2f76cefa271a536c238721aff6931bf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883405"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="january-2021-new-in-preview-only"></a>Январь 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications"></a>Облачные коммуникации
- Организация трансляций как ресурсов [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). См. [пример](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token). 
- Получение потока содержимого в виде [отчета об участниках](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event), [записи](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event) или альтернативной записи трансляции.
- Получение статуса [присутствия](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) пользователя, которого [нет на месте](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true), а также любого сообщения, заданного в качестве этого статуса.

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- [Обновление пароля домена Active Directory](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) для успешного [локального сетевого подключения](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true).
- [Запуск проверок работоспособности локального сетевого подключения](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) теперь может выявлять 5 дополнительных типов ошибок в ресурсе [проверки работоспособности локального подключения](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true). Дополнительные сведения о типах ошибок см. в [журнале изменений](https://developer.microsoft.com/graph/changelog) за январь 2021 г.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
Использование делегированных разрешений в приложениях от имени вошедшего пользователя:
- `PrinterShare.ReadBasic.All` для чтения основных сведений об общих принтерах, кроме сведений об управлении доступом.
- `PrintConnector.Read.All` для чтения соединителей печати.
- `PrintConnector.ReadWrite.All` для чтения и записи соединителей печати.
- `PrintJob.Create` для создания заданий печати и отправки содержимого в задания печати.
- `PrintSettings.Read.All` для чтения параметров печати на уровне клиента.
- `PrintSettings.ReadWrite.All` для чтения или записи параметров печати на уровне клиента.
- `Reports.Read.All` для чтения сводки об использовании печати для определенного пользователя или принтера.

### <a name="groups"></a>Группы
Получение состояния обработки динамической группы на основе правил с помощью свойства **membershipRuleProcessingStatus**. Это удобно, когда изменяется атрибут пользователя, участие пользователя в [группе Microsoft 365](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) на основе правил подвергается повторной оценке в соответствии с правилами участия в группе, настроенными в организации. 

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Приложения могут использовать делегированные разрешения, чтобы пользователи могли вызывать API для управления собственными [способами проверки подлинности](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true), или использовать разрешения приложений, чтобы позволить администраторам управлять способами проверки подлинности для других пользователей.
- Поддержка [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) в качестве способа проверки подлинности пользователя для входа или многофакторной проверки подлинности в Azure AD.
- Использование [политики Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true), чтобы определить параметры конфигурации, а также пользователей или группы, которым разрешено применять Microsoft Authenticator в качестве способа проверки подлинности. Использование политики Microsoft Authenticator вместо [политики входа по телефону без пароля с помощью Microsoft Authenticator](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true), поддержка которой прекращена. 
- Поддержка [Windows Hello для бизнеса](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true) в качестве способа проверки подлинности пользователя при входе на устройствах с Windows без применения пароля.

## <a name="december-2020-new-and-generally-available"></a>Декабрь 2020 г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
- Организаторы собраний могут использовать свойство **hideAttendees** ресурса [event](/graph/api/resources/event), чтобы управлять возможностью участников видеть друг друга в списке собрания **Отслеживание**.
- Общая доступность свойства **isDraft** и метода [cancel](/graph/api/event-cancel), которые доступны для организаторов, а также доступность метода [forward](/graph/api/event-forward) для организаторов и участников, чтобы лучше управлять ресурсами [event](/graph/api/resources/event) в календаре.
- Общая доступность свойств **hexColor** и **isDefault** ресурса [calendar](/graph/api/resources/calendar), чтобы улучшить управление календарями.

### <a name="cloud-communications"></a>Облачные коммуникации
Общая доступность ресурса [presence](/graph/api/resources/presence), позволяющего получать сведения о присутствии одного или нескольких пользователей, например их доступность и действия.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Воспользуйтесь новым [учебником](tutorial-riskdetection-api.md), чтобы узнать, как использовать [API защиты удостоверения](/graph/api/resources/identityprotectionroot) для идентификации риска и настройки рабочего процесса для подтверждения компрометации или включения исправления.

### <a name="teamwork"></a>Командная работа
- Общая доступность [API для управления установкой приложения Teams](/graph/api/resources/teamsappinstallation), в том числе управления установкой приложений, а также добавления, удаления или обновления приложения в команде или в личной области пользователя.
- [Получение чата между пользователем и приложением Teams](/graph/api/userscopeteamsappinstallation-get-chat).

### <a name="use-the-toolkit"></a>Использование набора средств
Общая доступность набора средств Microsoft Graph Toolkit 2.0. Этот выпуск включает новый [компонент для задач Microsoft Graph To-Do](./toolkit/components/todo.md), отличающийся от [компонента задач Планировщика](./toolkit/components/tasks.md), и улучшенный [компонент карточки контакта](./toolkit/components/person-card.md). Дополнительные сведения см. в соответствующей [записи блога](https://developer.microsoft.com/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/).


## <a name="december-2020-new-in-preview-only"></a>Декабрь 2020 г.: новые возможности только в предварительной версии

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Продолжением реализации конвейера [API соответствия требованиям Microsoft 365](/graph/api/resources/ediscoveryapioverview?view=graph-rest-beta&preserve-view=true) является ресурс [custodian](/graph/api/resources/custodian?view=graph-rest-beta&preserve-view=true) и связанные с ним операции и методы для [выпуска](/graph/api/custodian-release?view=graph-rest-beta&preserve-view=true) или [активации](/graph/api/custodian-activate?view=graph-rest-beta&preserve-view=true) хранителя. Используйте ресурс **custodian** для доступа к данным хранителя ([userSource](/graph/api/resources/userSource?view=graph-rest-beta&preserve-view=true)) в почтовом ящике Exchange Online, OneDrive для бизнеса, сайтах SharePoint ([siteSource](/graph/api/resources/siteSource?view=graph-rest-beta&preserve-view=true)) и группах Microsoft 365 ([unifiedGroupSource](/graph/api/resources/unifiedGroupSource?view=graph-rest-beta&preserve-view=true)).

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
Определение состояния сбоя виртуального рабочего стола с облачным управлением в целом как `failed` в свойстве **status** ресурса [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- [Обновление](/graph/api/printjob-update-configuration?view=graph-rest-beta&preserve-view=true) [конфигурации](/graph/api/resources/printjobconfiguration?view=graph-rest-beta&preserve-view=true) [задания печати](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Сведения о переименовании нескольких свойств и изменении типа связей см. в разделе Декабрь 2020 г. [журнала изменений API](https://developer.microsoft.com/graph/changelog/).

### <a name="education"></a>Образование
- Если учащиеся добавляются после публикации задания, преподаватели могут управлять действием задания, используя свойство **addedStudentAction** ресурса [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true).
- Преподаватели могут размещать уведомление о публикации задания с помощью свойства **notificationChannelUrl** ресурса **educationAssignment**.

### <a name="identity-and-access"></a>Удостоверение и доступ
Получение или настройка метаданных версии и создания для [соглашения](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) [об условиях использования](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true), [файла соглашения](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) и отношения [agreementfilelocalization](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true) в Azure AD.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
В рамках [управления правами](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) Azure Active Directory, когда пользователи хотят получить доступ к группам или приложениям либо сайты SharePoint Online запрашивают назначение для [пакета доступа](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true), они теперь могут отвечать на [вопросы](/graph/api/resources/accesspackagequestion?view=graph-rest-beta&preserve-view=true), представленные [локализованном содержимом](/graph/api/resources/accesspackagelocalizedcontent?view=graph-rest-beta&preserve-view=true) [запросa на назначение пакета доступа](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Администраторы могут связывать пользовательские потоки с приложениями, общий доступ к которым предоставлен внешним пользователям, и включить [самостоятельную регистрацию](/azure/active-directory/external-identities/self-service-sign-up-overview) в этих приложениях. Они могут настраивать пользовательские потоки самостоятельной регистрации и создавать персонализированные интерфейсы регистрации. В частности, они могут создать [прослушивателя для события начала регистрации, чтобы вызывать настраиваемый пользовательский поток](/graph/api/resources/invokeuserflowlistener?view=graph-rest-beta&preserve-view=true). После связи приложения с пользовательским потоком пользователи, переходящие в это приложение, смогут запускать поток регистрации, предоставляющий гостевую учетную запись.
- В [пользовательском потоке Azure Active Directory](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true) или [пользовательском потоке клиента Azure Active Directory B2C](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true) вы можете управлять стандартными языковыми параметрами и [настраивать языки и строки, отображаемые для пользователей в пользовательском потоке](/graph/api/resources/userflowlanguageconfiguration?view=graph-rest-beta&preserve-view=true).
- Использование [соединителя API](/graph/api/resources/identityapiconnector?view=graph-rest-beta&preserve-view=true) в пользовательских потоках для самостоятельной регистрации Azure AD и регистрации Azure AD B2C, чтобы вызывать API на определенном шаге для воздействия на выполнение пользовательского потока.
- Определение [политики способов проверки подлинности OTP электронной почты](/graph/api/resources/emailauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) для клиента.

### <a name="teamwork"></a>Командная работа
- Новые возможности для ресурса [member](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true) в контексте [команды](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), [канала](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) или [чата](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true):
  - Выделение участника, который является [пользователем Azure AD](/graph/api/resources/aaduserconversationmember?view=graph-rest-beta&preserve-view=true), с указанием ИД пользователя, адреса электронной почты и ИД клиента Azure AD. 
  - [Добавление нескольких пользователей в качестве участников команды](/graph/api/conversationmembers-add?view=graph-rest-beta&preserve-view=true).
- Для ресурса [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true):
  - [Получение всех сообщений в чатах, в которых принимал участие определенный пользователь](/graph/api/chats-getallmessages?view=graph-rest-beta&preserve-view=true), включая приватные чаты, групповые чаты и чаты собраний.
  - Использование всех возможностей для перечисления, получения, добавления, удаления и обновления [приложения](/graph/api/resources/teamsappinstallation?view=graph-rest-beta&preserve-view=true) или [вкладки](/graph/api/resources/teamstab?view=graph-rest-beta&preserve-view=true) в чате.
  - Использование свойства **chatType**, чтобы отличать приватный чат от группового чата или от чата, связанного с собранием по сети.
  - [Создание](/graph/api/chat-post?view=graph-rest-beta&preserve-view=true) или [обновление](/graph/api/chat-patch?view=graph-rest-beta&preserve-view=true) чата.
  - Для участника в контексте чата используйте свойство **visibleHistoryStartDateTime**, чтобы настроить или получить метку времени, указывающую, с какого момента в прошлом участнику предоставлен журнал беседы.
  - [Создание](/graph/api/chat-post-members?view=graph-rest-beta&preserve-view=true) или [удаление](/graph/api/chat-delete-members?view=graph-rest-beta&preserve-view=true) участника из указанного чата. 
- Для ресурса [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true):
  - [Получение всех сообщений из всех каналов в команде](/graph/api/channels-getallmessages?view=graph-rest-beta&preserve-view=true).
  - Владельцы команд могут включить [модерацию для канала](/graph/api/resources/channelmoderationsettings?view=graph-rest-beta&preserve-view=true), чтобы контролировать, кто может создавать новые сообщения или отвечать на сообщения в канале, используя свойство **moderationSettings** канала.
- В рамках [определения приложения Teams](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true) используйте связь **bot**, чтобы подключаться к [боту командной работы](/graph/api/resources/teamworkbot?view=graph-rest-beta&preserve-view=true).

### <a name="to-do-tasks"></a>Задачи To-Do
Подписывайтесь на [уведомления об изменениях](webhooks.md) [задачи To Do](/graph/api/resources/todoTask?view=graph-rest-beta&preserve-view=true).

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
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](https://developer.microsoft.com/graph/changelog/).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).