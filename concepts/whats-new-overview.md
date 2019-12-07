---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ae0ec1d070a163cbb093dfabfb36edf2b034f441
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895495"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API см. в [декабрьском](changelog.md#december-2019) и [ноябрьском](changelog.md#november-2019) разделах журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.


## <a name="december-2019-new-in-preview"></a>Декабрь 2019 г.: новые возможности в предварительной версии

### <a name="teamwork"></a>Командная работа
- [Настройка уведомлений об изменениях, включающих данные](webhooks-with-resource-data.md) для ресурсов [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) в каналах и чатах Microsoft Teams.
- [Подписка на уведомления](/graph/api/resources/subscription?view=graph-rest-beta) о новых и измененных [сообщениях канала или чата](/graph/api/resources/chatmessage?view=graph-rest-beta).

## <a name="november-2019-new-and-generally-available"></a>Ноябрь 2019 г.: новые и общедоступные возможности

### <a name="groups"></a>Группы
- Использование разрешений приложения или делегированных разрешений GroupMember.Read.All и GroupMember.ReadWrite.All для перечисления групп, чтения основных свойств групп, считывания (и обновления при наличии разрешения на чтение и запись) сведений об участии в группах, к которым у приложения есть доступ.
- Использование разрешения приложения Group.Create для создания групп без необходимости входа пользователя.
- Для указанной [группы](/graph/api/resources/group?view=graph-rest-1.0) [проверка участия](/graph/api/group-checkmemberobjects?view=graph-rest-1.0) в других группах или ролях каталога.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Регистрация [приложений](/graph/api/resources/application?view=graph-rest-1.0), проходящих проверку подлинности в Azure Active Directory (Azure AD). Используйте делегированные [разрешения](/graph/permissions-reference#application-resource-permissions), Application.Read.All и Application.ReadWrite.All, или разрешение приложения, Application.Read.All.
- Для указанного [устройства](/graph/api/resources/device?view=graph-rest-1.0) [проверка участия](/graph/api/device-checkmemberobjects?view=graph-rest-1.0) в других группах или ролях каталога.

### <a name="mail"></a>Почта
- Использование свойства **conversationIndex** для получения положения сообщения в беседе электронной почты Outlook.
- Использование делегированного разрешения Mail.ReadBasic и разрешения приложения Mail.ReadBasic.All, чтобы получить ресурсы [message](/graph/api/resources/message?view=graph-rest-1.0) или [mail folder](/graph/api/resources/mailfolder?view=graph-rest-1.0), отслеживать их изменения, а также управлять [подпиской](/graph/api/resources/subscription?view=graph-rest-1.0) на уведомления об изменениях сообщений.

### <a name="users"></a>Пользователи
- [Проверка участия в группах](/graph/api/user-checkmemberobjects?view=graph-rest-1.0) для определенного [пользователя](/graph/api/resources/user?view=graph-rest-1.0).
- Использование свойства **creationType**, чтобы узнать, как была создана учетная запись пользователя, например была ли она создана в качестве обычной учебной или рабочей учетной записи либо в качестве внешней учетной записи и т. д.

## <a name="november-2019-new-in-preview"></a>Ноябрь 2019 г.: новые возможности в предварительной версии

### <a name="calendar"></a>Календарь
- [Организация и посещение собраний по сети с помощью Outlook](outlook-calendar-online-meetings.md).
- [Настройка свойств](/graph/api/place-update?view=graph-rest-beta) для расширенных типов расположений [комната](/graph/api/resources/room?view=graph-rest-beta) и [список комнат](/graph/api/resources/roomlist?view=graph-rest-beta).

### <a name="cloud-communication"></a>Облачное взаимодействие
Тип ресурса [call](/graph/api/resources/call?view=graph-rest-beta) поддерживает следующие дополнительные функции:

- [Контекст входящего звонка](/graph/api/resources/incomingcontext?view=graph-rest-beta)
- Тип конечной точки для участника, например голосовая почта или Skype для бизнеса
- Возможность [обновления](/graph/api/call-updaterecordingstatus?view=graph-rest-beta) [сведений о записи](/graph/api/resources/recordinginfo?view=graph-rest-beta) для [участника](/graph/api/resources/participant?view=graph-rest-beta)

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [ноябрь](changelog.md#november-2019)

### <a name="education"></a>Образование
Администраторы могут включать параметры на уровне класса с помощью свойства **classSettings** [команды](/graph/api/resources/team?view=graph-rest-beta), связанной с [классом](/graph/api/resources/educationclass?view=graph-rest-beta). В настоящее время существует параметр для уведомления опекунов о еженедельных заданиях.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Использование разрешения приложения Policy.Read.All для чтения всех политик условного доступа и именованных расположений организации без необходимости входа пользователя.
- Поддержка для [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) состояния только для отчета `enabledForReportingButNotEnforced`.
- Использование делегированного разрешения ThreatAssessment.ReadWrite.All или разрешения приложения ThreatAssessment.Read.All для чтения (или создания при наличии разрешения на чтение и запись) запросов на оценку угроз в организации.

### <a name="mail"></a>Почта
Использование делегированного разрешения Mail.ReadBasic и разрешения приложения Mail.ReadBasic.All, чтобы управлять [подписками](/graph/api/resources/subscription?view=graph-rest-beta) на уведомления об изменениях в ресурсе [message](/graph/api/resources/message?view=graph-rest-beta).

### <a name="notifications"></a>Уведомления
Можно использовать новые компактные [веб-SDK](https://aka.ms/GNSDK) уведомлений вместо [SDK Project Rome](https://github.com/Microsoft/project-rome), чтобы воспользоваться улучшенной моделью проверки подлинности и поддержкой веб-приложений с push-уведомлениями. 

### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика
Первое появление ресурса [профиль](/graph/api/resources/profile?view=graph-rest-beta), который является расширенным представлением нового поколения записей людей в службах Майкрософт. Этот ресурс связан с распространенными и удобными атрибутами людей, включая информацию о всех важных датах, таких как [годовщины](/graph/api/resources/personanniversary?view=graph-rest-beta), а также об [образовании](/graph/api/resources/educationalactivity?view=graph-rest-beta), [должностях](/graph/api/resources/workposition?view=graph-rest-beta) и [интересах](/graph/api/resources/personinterest?view=graph-rest-beta), уровнях владения [языками](/graph/api/resources/languageproficiency?view=graph-rest-beta) и [навыками](/graph/api/resources/skillproficiency?view=graph-rest-beta), об [участии в проектах](/graph/api/resources/projectparticipation?view=graph-rest-beta) и [связи с веб-сайтами](/graph/api/resources/personwebsite?view=graph-rest-beta), а также прочие сведения об [учетной записи](/graph/api/resources/useraccountinformation?view=graph-rest-beta) и контактные данные.

### <a name="search"></a>Поиск
Первое появление [API Microsoft Search](search-concept-overview.md), с помощью которого пользователи приложений могут получать индивидуально адаптированные, более актуальные и релевантные результаты поиска с использованием возможностей Microsoft Graph. Можно использовать функцию [запроса](/graph/api/search-query?view=graph-rest-beta), которая по умолчанию выполняет поиск в сообщениях и событиях Outlook, а также в файлах OneDrive и SharePoint в облаке Майкрософт. Можно использовать [соединители](/microsoftsearch/connectors-overview), доступные в [коллекции соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы задействовать поисковые данные за пределами облака Майкрософт. Также можно [создавать собственные соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), индексировать внешние настраиваемые элементы и файлы, а также отправлять запросы к определенным внешним источникам данных.

### <a name="teamwork"></a>Командная работа
Получение ресурсов [file](/graph/api/resources/driveitem?view=graph-rest-beta), связанных с [командой](/graph/api/resources/team?view=graph-rest-beta) и [каналом](/graph/api/resources/channel?view=graph-rest-beta), с помощью следующего синтаксиса HTTP-запроса:

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>Пользователи
Использование свойства **creationType**, чтобы узнать, как была создана учетная запись пользователя, например была ли она создана в качестве обычной учебной или рабочей учетной записи либо в качестве внешней учетной записи и т. д.

## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Office 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Office 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

