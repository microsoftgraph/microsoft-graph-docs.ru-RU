---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 6eb661e4a7a84ea9dc1757db75d23e8169066988
ms.sourcegitcommit: 4da3cf28f252c974fb00894d21b6e04eccbeffbe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/21/2020
ms.locfileid: "49722497"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](changelog.md). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

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
Общая доступность набора средств Microsoft Graph Toolkit 2.0. Этот выпуск включает новый [компонент для задач Microsoft Graph To-Do](/graph/toolkit/components/todo), отличающийся от [компонента задач Планировщика](/graph/toolkit/components/tasks), и улучшенный [компонент карточки контакта](/graph/toolkit/components/person-card). Дополнительные сведения см. в соответствующей [записи блога](https://developer.microsoft.com/ru-RU/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/).

## <a name="december-2020-new-in-preview-only"></a>Декабрь 2020 г.: новые возможности только в предварительной версии

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Продолжением реализации конвейера [API соответствия требованиям Microsoft 365](/graph/api/resources/ediscoveryapioverview?view=graph-rest-beta&preserve-view=true) является ресурс [custodian](/graph/api/resources/custodian?view=graph-rest-beta&preserve-view=true) и связанные с ним операции и методы для [выпуска](/graph/api/custodian-release?view=graph-rest-beta&preserve-view=true) или [активации](/graph/api/custodian-activate?view=graph-rest-beta&preserve-view=true) хранителя. Используйте ресурс **custodian** для доступа к данным хранителя ([userSource](/graph/api/resources/userSource?view=graph-rest-beta&preserve-view=true)) в почтовом ящике Exchange Online, OneDrive для бизнеса, сайтах SharePoint ([siteSource](/graph/api/resources/siteSource?view=graph-rest-beta&preserve-view=true)) и группах Microsoft 365 ([unifiedGroupSource](/graph/api/resources/unifiedGroupSource?view=graph-rest-beta&preserve-view=true)).

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
Определение состояния сбоя виртуального рабочего стола с облачным управлением в целом как `failed` в свойстве **status** ресурса [cloudPC](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- [Обновление](/graph/api/printjob-update-configuration?view=graph-rest-beta&preserve-view=true) [конфигурации](/graph/api/resources/printjobconfiguration?view=graph-rest-beta&preserve-view=true) [задания печати](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Сведения о переименовании нескольких свойств и изменении типа связей см. в разделе [Декабрь 2020 г.](changelog.md#december-2020) [журнала изменений API](changelog.md).

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
- Определение [политики методов проверки подлинности OTP электронной почты](/graph/api/resources/emailauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) для клиента.

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

## <a name="november-2020-new-and-generally-available"></a>Ноябрь 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачная коммуникация
- Общая доступность свойства **роль** типа [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo), разделяющего участников [виртуального собрания](/graph/api/resources/onlinemeeting) на участников и докладчиков.
- Общая доступность свойства **lobbyBypassSettings** и его [значений](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) для допуска пользователей к виртуальному собранию.
- Общая доступность свойства **isEntryExitAnnounced** для настройки параметров объявления пользователей, присоединяющихся к виртуальному собранию или покидающих его.
- Общая доступность свойства **allowedPresenters** для разрешения отдельным пользователям выступать на собрании.

### <a name="search"></a>Поиск
- Общая доступность [API запросов](/graph/api/resources/search-api-overview) Поиска (Майкрософт), поддерживающих поиск данных следующих типов:
  - [Сообщения Outlook](/graph/search-concept-messages)
  - [События календаря Outlook](/graph/search-concept-events)
  - [Ресурсы OneDrive и SharePoint](/graph/search-concept-files).

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
