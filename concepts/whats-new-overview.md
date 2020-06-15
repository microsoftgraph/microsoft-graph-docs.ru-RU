---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: c6c41527ea5b52e4d683cb2d14594c088f080142
ms.sourcegitcommit: d6374f42bee4de11fd7a3d0d8c2a7f8c4e7739bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2020
ms.locfileid: "44710603"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API [можно](changelog.md#may-2020) найти в разделах и [июньах](changelog.md#june-2020) , а также в разделах журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.


## <a name="june-2020-new-and-generally-available"></a>Июнь 2020: новый и обычно доступный

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
- Используйте `Accept-Language` заголовок HTTP при [создании собрания по сети](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0) для предоставления сведений о соединении на основе языкового стандарта.
- Используйте [креатеоржет](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0) , чтобы вернуть собрание по сети, которое содержит указанное значение **екстерналид** , или создайте его, если он уже существует, для упрощения внедрения результирующего собрания в сторонний календарь.

### <a name="security"></a>Безопасность
- Отслеживайте следующие свойства [оповещения](/graph/api/resources/alert?view=graph-rest-1.0):
  - Идентификаторы инцидентов, связанных с оповещением.
  - Определите [ресурс](/graph/api/resources/securityResource?view=graph-rest-1.0#securityresourcetype-values) как атаковать или как связанный ресурс в оповещении.
  - Укажите расположение источника и назначения для [сетевого подключения](/graph/api/resources/networkconnection?view=graph-rest-1.0) , связанного с оповещением.

### <a name="teamwork"></a>Командная работа
Используйте делегированное разрешение [CamlQuery. Read. ALL](/graph/permissions-reference#appcatalog-resource-permissions) , чтобы перечислить [приложения](/graph/api/resources/teamsapp?view=graph-rest-1.0) из каталога приложений Microsoft Teams.


## <a name="june-2020-new-in-preview-only"></a>Июнь 2020: Новая версия только для предварительного просмотра
### <a name="cloud-communications--presence"></a>Взаимодействие с облаком | Знак
[Получение сведений о присутствии](/graph/api/presence-get?view=graph-rest-beta) всех пользователей в организации или определенного пользователя в Организации.

### <a name="identity-and-access"></a>Удостоверение и доступ
- ИТ-специалисты могут использовать ресурсы [соединителей](/graph/api/resources/connector?view=graph-rest-beta) , которые являются упрощенными агентами для подключения к [прокси-серверу приложений Azure AD](/azure/active-directory/manage-apps/what-is-application-proxy), и [публикации локальных приложений веб-приложений извне](/graph/api/resources/onpremisespublishing?view=graph-rest-beta), чтобы удаленные пользователи их организаций могли безопасно получать доступ к этим приложениям.
- Управление [политикой проверки подлинности](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta) на уровне клиента для включения или отключения [самостоятельной регистрации](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta) внешних пользователей.

## <a name="may-2020-new-and-generally-available"></a>Май 2020: новый и обычно доступный

### <a name="calendar--place"></a>Календарь | Место
GA API для почтовых [мест](/graph/api/resources/place) в версии 1.0 используйте этот API в производственных приложениях для получения, обновления или удаления [комнаты](/graph/api/resources/room) или [списка помещений](/graph/api/resources/roomlist) в клиенте. [Узнайте больше](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) об API мест.

### <a name="change-notifications"></a>Уведомления об изменениях
- Подпишитесь на уведомления об изменениях в Microsoft Cloud для государственных организаций США.

### <a name="cloud-communications--call-records"></a>Облачные коммуникации | Записи звонков
- GA в [API записей вызовов](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0) — используйте ресурс [каллрекорд](/graph/api/resources/callrecord?view=graph-rest-1.0) для получения метаданных звонков и собраний по сети в Microsoft Teams и Skype.
- Подпишитесь на [уведомления об изменении](/graph/webhooks) всех ресурсов **каллрекорд** в Организации.
- [Перечислите сеансы](/graph/api/callrecords-session-list?view=graph-rest-1.0) в **каллрекорд**и при необходимости [разверните каждый сеанс, чтобы отобразить сегменты](/graph/api/callrecords-session-list?view=graph-rest-1.0#example-2-get-session-list-with-segments) в записи вызова.
- Поддержка значений диапазона 60 ГГц ( `frequency60GHz` ) и `unknownFutureValue` диапазона Wi-Fi для конечной точки мультимедиа в сегменте.
- Поддержка голосовой почты в качестве возможного типа конечной точки на стороне службы в [сегменте](/graph/api/resources/callrecords-segment)связи.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Intune [можно](changelog.md#may-2020) обновить в версии 1.0.

### <a name="graph-explorer"></a>Песочница Graph
Используйте многие новые возможности [проводника Graph](https://developer.microsoft.com/en-us/graph/graph-explorer) , которые улучшают обучение и создание прототипов в песочнице. Пример:
- Просмотрите фрагменты кода, соответствующие введенному запросу REST API, в C#, Java, JavaScript и целевом языке C.
- Войти в систему с помощью клиента, просмотреть и скопировать маркер доступа в ваше клиентское приложение REST.

Для получения дополнительных сведений см. [новый проводник Graph](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/) .

### <a name="groups"></a>Группы
- Синхронизация локального каталога с Azure Active Directory через Azure AD Connect теперь возвращает свойства **onPremisesDomainName**, **онпремисеснетбиоснаме** и **onPremisesSamAccountName** как часть ресурса [Group](/graph/api/resources/group?view=graph-rest-1.0) .
- Подпишитесь на уведомления об изменении ресурсов [группы](/graph/api/resources/group) в Microsoft Cloud Китая под управлением 21vianet.

### <a name="identity-and-access"></a>Удостоверение и доступ
- GA API-интерфейса субъектов-служб в версии 1.0 используйте ресурс [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) в производственных приложениях для программного управления экземплярами приложений и управления действиями, которые может выполнять приложение в клиенте. Можно контролировать, кто может использовать приложение, ресурсы, к которым приложение имеет доступ, например, добавлять учетные данные пароля, пошаговые сертификаты с истекшим сроком действия и управлять назначениями ролей приложений.
- GA API [аппролеассигнмент](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0) , который записывает назначение [аппроле](/graph/api/resources/approle?view=graph-rest-1.0) (представляющее `roles` утверждения в маркерах ID и маркерах доступа) [пользователю](/graph/api/resources/user?view=graph-rest-1.0), [группе](/graph/api/resources/group?view=graph-rest-1.0)или [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0).
- Использование Facebook в качестве поставщика удостоверений в Azure Active Directory.
- Используйте делегированное разрешение или разрешение приложения, `AppRoleAssignment.ReadWrite.All` чтобы разрешить приложению управлять предоставлением разрешений на приложения любому API (включая Microsoft Graph) и назначениям приложений для любого приложения, соответственно или без пользователя, выполнившего вход в систему.


### <a name="microsoft-graph-sdks"></a>Пакеты SDK Microsoft Graph
Ознакомьтесь с новыми рекомендациями SDK по следующим вопросам:
- [Разбиение на страницы](/graph/sdks/paging)
- [Пакетная обработка](/graph/sdks/batch-requests)
- [Отправка больших файлов в OneDrive](/graph/sdks/large-file-upload)
- [Настройка клиента службы SDK с помощью компонентов промежуточного слоя HTTP](/graph/sdks/customize-client).

### <a name="teamwork"></a>Командная работа
- Если ваш сценарий включает собрания по сети в Teams, ознакомьтесь с разделом новые рекомендации по [выбору](choose-online-meeting-api.md) между [API календаря](outlook-calendar-online-meetings.md) и [API облачных коммуникаций](cloud-communications-online-meetings.md) для создания собраний по сети и присоединения к ним.
- [Отправка](/graph/api/channel-post-messages?view=graph-rest-1.0) сообщений и [ответ на них](/graph/api/channel-post-messagereply?view=graph-rest-1.0) в [канале](/graph/api/resources/channel?view=graph-rest-1.0).
- Получение расположения OneDrive для бизнеса файлов для [канала](/graph/api/resources/channel?view=graph-rest-1.0)с помощью свойства навигации **филефолдер** .

### <a name="teamwork--shifts"></a>Командная работа | Смены
Конец [API смен](/graph/api/resources/shift?view=graph-rest-1.0) в версии 1.0: Используйте этот API в производственных приложениях для создания, обновления и управления расписаниями рабочих процессов задействование, чтобы обеспечить их эффективное общение и сотрудничество.

### <a name="users"></a>Пользователи
- Подпишитесь на уведомления об изменении [пользовательских](/graph/api/resources/user) ресурсов в Microsoft Cloud Китая под управлением 21vianet.
- Отслеживайте состояние и дату и время последнего изменения состояния внешнего пользователя, который был [приглашен](/graph/api/invitation-post?view=graph-rest-1.0) на присоединение к Организации с помощью свойств **свойства** и **екстерналусерстатечанжедатетиме** ресурса **User** .

## <a name="may-2020-new-in-preview-only"></a>Май 2020: новый только предварительный просмотр

### <a name="change-notifications"></a>Уведомления об изменениях
- Используйте в формальном схематизированные типы [чанженотификатион](/graph/api/resources/changenotification?view=graph-rest-beta) и [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) для обработки уведомлений об изменении ресурсов. 
- Отслеживайте, находятся ли уведомления в последовательности, или если отсутствует уведомление с помощью свойства **SequenceNumber** ресурса **чанженотификатион** .

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Ресурсы [принтера](/graph/api/resources/printer?view=graph-rest-beta) и [принтершаре](/graph/api/resources/printershare?view=graph-rest-beta) теперь хранятся в четном виде и имеют одинаковые свойства.
- Некоторые свойства и имена типов очищаются в общих папках принтера:
  - Используйте свойство **Shared** навигации для [Print](/graph/api/resources/print?view=graph-rest-beta) , чтобы получить список общих папок принтера, зарегистрированных в клиенте. 
  - Подробные сведения [можно](changelog.md#may-2020) найти в журнале изменений в журнале.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Intune [может](changelog.md#may-2020) обновляться в бета-версии.

### <a name="groups"></a>Группы
- [Оценка](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta) того, является ли пользователь или устройство участником динамической группы, с помощью существующего правила для [группы](/graph/api/resources/group?view=graph-rest-beta) или указанного правила. [Динамическое членство на основе правил](/azure/active-directory/users-groups-roles/groups-dynamic-membership) снижает затраты на администрирование добавления и удаления участников.
- При создании [группы](/graph/api/resources/group?view=graph-rest-beta)Office 365 настройте поведение группы, указав ее в свойстве **ресаурцебехавиороптионс** . Например, разрешите участникам отправлять, подписываться на беседу, отключать приветственные сообщения и скрывать группу в Outlook.
- Укажите ресурсы для подготовки в свойстве **ресаурцепровисионингоптионс** , которые обычно не входят в создание [группы](/graph/api/resources/group?view=graph-rest-beta) по умолчанию. В настоящее время поддерживается предоставление [группы в качестве группы с возможностями](/graph/api/resources/team?view=graph-rest-beta) Microsoft Teams.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Применяйте системные параметры запросов OData ( `$count` , `$filter` , `$search` ) при извлечении коллекций сущностей, являющихся производными от [directoryObject](). Можно [выполнить поиск определенных маркеров](/graph/query-parameters?#using-search-on-directory-object-collections) в свойствах **DisplayName** и **Description** для этих сущностей и использовать приведение OData для обрезки результатов **directoryObject** до определенных производных типов. Более подробную информацию можно найти в [статье Создание расширенных запросов в Microsoft Graph с помощью $Count, $Filter, $Search и $OrderBy](https://developer.microsoft.com/en-us/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/).
- В рамках [API защиты удостоверений](/graph/api/resources/identityprotection-root?view=graph-rest-beta)используйте свойство **рискевенттипе** , чтобы [получить тип обнаруженного риска](/graph/api/riskdetection-get?view=graph-rest-beta), или [Получите тип риска в журнале пользователя](/graph/api/riskyuser-list-history?view=graph-rest-beta). Не используйте свойство **рисктипе** , так как оно является устаревшим.
- Укажите типы клиентских приложений в свойстве **клиентапптипес** [набора условий](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta) для [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta).
- Используйте делегированное разрешение, `EntitlementManagement.Read.All` чтобы разрешить приложению считывать пакеты доступа и связанные ресурсы управления обслуживанием от имени пользователя, выполнившего вход в систему.
- Используйте делегированные разрешения или разрешения приложения `Application.Read.All` , а `Application.ReadWrite.All` также [перечислите приложения](/graph/api/application-list?view=graph-rest-beta) в Организации.
- Управление параметрами авторизации в Azure AD с помощью типа ресурса [аусоризатионполици](/graph/api/resources/authorizationpolicy?view=graph-rest-beta) .

### <a name="teamwork"></a>Командная работа
- Приложения Teams, [поддерживающие единый вход (SSO)](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) , могут указывать значение `WebApplicationInfo.id` из манифеста приложения Teams в свойстве **азуреадаппид** объекта [теамсаппдефинитион](/graph/api/resources/teamsappdefinition?view=graph-rest-beta).
- Используйте [детально детализированные разрешения](/graph/permissions-reference#teams-resource-specific-consent-permissions) для доступа к ресурсам [Team](/graph/api/resources/team?view=graph-rest-beta) и [Channel](/graph/api/resources/channel?view=graph-rest-beta) .




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

