---
title: Обзор предыдущих выпусков Microsoft Graph
description: Новые возможности в предыдущих выпусках Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: f9d62486ba64e0ee597872276f1f62f869d8a632
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038641"
---
# <a name="highlights-of-earlier-releases"></a>Обзор предыдущих выпусков

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
Используйте многие новые возможности [проводника Graph](https://developer.microsoft.com/en-us/graph/graph-explorer) , которые улучшают обучение и создание прототипов в песочнице. Например,
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
- При создании [группы](/graph/api/resources/group?view=graph-rest-beta)Microsoft 365 настройте поведение группы, указав ее в свойстве **ресаурцебехавиороптионс** . Например, разрешите участникам отправлять, подписываться на беседу, отключать приветственные сообщения и скрывать группу в Outlook.
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


## <a name="april-2020-new-and-generally-available"></a>Апрель 2020 г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
- [Делитесь календарями или делегируйте их](outlook-share-or-delegate-calendar.md) программным способом, соответствующим пользовательскому интерфейсу Outlook. Поддерживается отслеживание разрешений текущего пользователя и состояния общего доступа к календарю, а также следующие возможности:
  - Для каждого [календаря](/graph/api/resources/calendar?view=graph-rest-1.0) теперь можно управлять [разрешениями](/graph/api/resources/calendarpermission?view=graph-rest-1.0) каждого пользователя, которому предоставлен доступ к календарю. 
  - Для каждого [почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-1.0) теперь можно указать, кто получает сообщения о собраниях и ответы на эти сообщения: делегат, владелец почтового ящика или и тот, и другой. 
- [Создание или обновление события в виде собрания по сети](outlook-calendar-online-meetings.md):
  - В каждом **календаре** можно указать разрешенных и используемых по умолчанию поставщиков собраний по сети.
  - Можно создать или обновить [мероприятие](/graph/api/resources/event?view=graph-rest-1.0), доступное по сети, и предоставить участникам сведения для присоединения к собранию по сети. 
  - В частности, можно использовать **onlineMeetingProvider** и **onlineMeeting** — это новые свойства **мероприятий**, с помощью которых можно задать или указать Microsoft Teams в качестве поставщика собраний по сети. Это временное решение [известной проблемы](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) со свойством **onlineMeetingUrl**.
- Добавление [файловых вложений до 150 МБ](outlook-large-attachments.md) в [событие](/graph/api/resources/event?view=graph-rest-1.0).

### <a name="files"></a>Файлы
- [Извлекайте](/graph/api/driveitem-checkout?view=graph-rest-1.0) и [возвращайте](/graph/api/driveitem-checkin?view=graph-rest-1.0) файлы в OneDrive, чтобы управлять их обновлением и делать обновления доступными для других пользователей.
- Применение необязательных параметров и даты истечения срока действия к ссылке " [пригласить](/graph/api/driveitem-invite?view=graph-rest-1.0) " и " [Создание ссылки для совместного доступа](/graph/api/driveitem-createlink?view=graph-rest-1.0) " для предоставления общего доступа к [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0).
- Получение или установка пароля и даты истечения срока действия [разрешения](/graph/api/resources/permission?view=graph-rest-1.0), а также отслеживание [набора удостоверений](/graph/api/resources/identityset?view=graph-rest-1.0) пользователей, которым предоставлено разрешение на общий доступ к **driveItem**.
- Получение [разрешения](/graph/api/resources/permission?view=graph-rest-1.0) для [элемента общего диска](/graph/api/resources/shareddriveitem?view=graph-rest-1.0) с помощью свойства навигации **разрешений** .
- Ограничьте для пользователей, имеющих [ссылку для совместного доступа](/graph/api/resources/sharinglink?view=graph-rest-1.0) , только просматривать и загружать содержимое общих**driveItem** в OneDrive для бизнеса или SharePoint.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Чтобы управлять ролями и назначать доступ к ресурсам в провайдерах управления доступом на основе ролей (RBAC), таких как Microsoft Intune, используйте [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0). Ресурс **unifiedRoleAssignmentMultiple** поддерживает определение одной роли в массиве областей и назначение роли для нескольких субъектов (например, пользователей).
- Получите доступ к определенным типам [политик для организации](/graph/api/resources/policy-overview?view=graph-rest-1.0), используя `/policies`сегмент URL и указав тип политики. Например, организация может применить политику для автоматического выхода пользователя из веб-сеанса после периода бездействия; см. операции CRUD для экземпляров [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0). Это [серьезное изменение](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/), упрощающее обнаружение всех политик путем группировки всех типизированных политик в сегменте `/policies`. Доступ к другим типизированным политикам осуществляется аналогичным образом: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0) и [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0). 

### <a name="mail"></a>Почта
Добавление [файловых вложений до 150 МБ](outlook-large-attachments.md) в [сообщение](/graph/api/resources/message?view=graph-rest-1.0).

### <a name="sites-and-lists"></a>Сайты и списки
- [Список сайтов](/graph/api/sites-list-followed?view=graph-rest-1.0), на которые подписан пользователь.
- Определите географический регион [семейства веб-сайтов](/graph/api/resources/sitecollection?view=graph-rest-1.0) с помощью свойства **даталокатионкоде** .
- Определите клиент для файла, папки или другого элемента в SharePoint, обратившись к свойству **tenantId** , которое является частью **sharepointIds** [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0).

## <a name="april-2020-new-in-preview-only"></a>Апрель 2020 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать

Назначьте разрешенным пользователям и группам доступ к определенным [общим принтерам](/graph/api/resources/printershare?view=graph-rest-beta) Универсальной печати — облачной инфраструктуры печати Microsoft 365. Чтобы воспользоваться возможностями надежного централизованного управления печатью и предложить пользователям простой, но полнофункциональный и безопасный интерфейс печати, ознакомьтесь с [объявлением Универсальной печати](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775) и присоединитесь к программе по ознакомлению с предварительной версией.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [апрель](changelog.md#april-2020).

### <a name="groups"></a>Группы
Определите, какое приложение создало [группу](/graph/api/resources/group?view=graph-rest-beta), по идентификатору приложения.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Отслеживание изменений](/graph/api/administrativeunit-delta?view=graph-rest-beta), касающихся [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta).
- [Отслеживание изменений](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta), касающихся [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta).
- [Управление](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta) пользовательскими [методами проверки подлинности](/graph/api/resources/authenticationmethod?view=graph-rest-beta), среди которых [пароль](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta) или [телефон](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta). Например, [сброс пароля пользователя](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta) и [получение состояния сброса](/graph/api/authenticationoperation-get?view=graph-rest-beta) или [добавление номера телефона](/graph/api/authentication-post-phonemethods?view=graph-rest-beta) пользователя для проверки подлинности с помощью SMS или голосового вызова, если для этого пользователя включена соответствующая политика.

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
[Список](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta) [проверяющих сторон](https://docs.microsoft.com/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts), настроенных в службах федерации Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Просмотр данных о **созданных собраниях** и **действиях с уведомлениями о собраниях** в отчетах CSV, включающих [счетчики действий с электронной почтой](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta), [счетчики пользователей, совершающих действия с электронной почтой](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) и [данные о действиях пользователей с электронной почтой](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta).


## <a name="march-2020-new-and-generally-available"></a>Март 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачные коммуникации
- Получите функцию маршрутизации вызовов и контекст входящих [вызовов](/graph/api/resources/call?view=graph-rest-1.0).
- [Обновите состояние записи](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0) звонка.
- Укажите информацию о записи для [участника](/graph/api/resources/participant?view=graph-rest-1.0), включая инициатора и состояние записи.
- Для уникальной идентификации участников конференции или [звонка](/graph/api/resources/call?view=graph-rest-1.0) от участника к участнику используйте свойство **callChainId**.
- Определите как часть [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0) код страны и тип конечной точки (например, Skype для бизнеса или Skype для бизнеса VoIP) участника.
- Сторонние партнеры в области устройств видеоконференцсвязи (VTC) могут регистрировать и предоставлять сведения о качестве связи для своих устройств через бот Cloud Video Interop (CVI) с помощью функции [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0). Качество связи определяется данными открытого типа о [звуке](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0), [видео](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0) и [демонстрации экрана](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0).

### <a name="files"></a>Файлы
- [Удаленные элементы](/graph/api/resources/remoteitem?view=graph-rest-1.0), к которым пользователю предоставлен общий доступ, добавленные в хранилище OneDrive пользователя или возвращенные как результаты поиска, могут содержать метаданные для изображения или видео.
- [Отслеживайте](/graph/api/driveitem-follow?view=graph-rest-1.0) объект [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) для удобного доступа или упрощения таких действий, как перемещение, копирование и сохранение в определенном формате. Используйте [отмену отслеживания](/graph/api/driveitem-unfollow?view=graph-rest-1.0), чтобы прекратить отслеживание элемента диска.
- [Предоставьте](/graph/api/permission-grant?view=graph-rest-1.0) пользователям разрешение на доступ к ссылке для общего доступа, чтобы поделиться соответствующим элементом диска.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Отслеживайте изменения](/graph/api/orgcontact-delta?view=graph-rest-1.0) в [контактах организации](/graph/api/resources/orgcontact?view=graph-rest-1.0).
- Используйте свойство **riskEventTypes_v2**, чтобы получить типы событий риска, связанные с [входом](/graph/api/resources/signin?view=graph-rest-1.0).
- Используйте делегированное разрешение `User.ManageIdentities.All`, чтобы разрешить приложению считывать, обновлять и удалять удостоверения, связанные с учетной записью пользователя, к которой имеет доступ зарегистрированный пользователь. Используйте это разрешение на уровне приложения без зарегистрированного пользователя. Это позволяет приложению [определить](/graph/api/user-update?view=graph-rest-1.0), с помощью каких удостоверений пользователь может войти.

### <a name="reports"></a>Отчеты
Использование администратора службы Teams и администратора служб Teams в качестве обслуживаемых ролей пользователей позволяет приложениям читать отчеты об использовании служб Microsoft 365 от имени пользователя, а также [формы авторизации, делегированные пользователю](reportroot-authorization.md). 

### <a name="sites"></a>Сайты
- Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-1.0) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-1.0) сайтов SharePoint. 
- [Подпишитесь на уведомления об изменениях](/graph/api/resources/subscription?view=graph-rest-1.0) в [списке](/graph/api/resources/list?view=graph-rest-1.0) SharePoint.

## <a name="march-2020-new-in-preview-only"></a>Март 2020: Новое только в превью

### <a name="calendar"></a>Календарь
- Используйте свойство **calendarGroupId**, чтобы получить группу [календаря](/graph/api/resources/calendargroup?view=graph-rest-beta), в которой создан [календарь](/graph/api/resources/calendar?view=graph-rest-beta).
- Используйте свойство **в черновике**, чтобы идентифицировать [событие](/graph/api/resources/event?view=graph-rest-beta) как собрание, которое пользователь обновил в Outlook, но не отправил для обновления участников.

### <a name="cloud-communications"></a>Облачные коммуникации
- Используйте [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta), чтобы получить экземпляр [онлайн-собрания](/graph/api/resources/onlinemeeting?view=graph-rest-beta) с помощью внешнего настраиваемого идентификатора или создать его, если он еще не существует.
- Вы можете использовать свойство **externalId**, чтобы определить онлайн-собрание с помощью внешнего настраиваемого идентификатора.
- Используйте необязательный заголовок HTTP-запроса `Accept-Language`, чтобы [создать](/graph/api/application-post-onlinemeetings?view=graph-rest-beta) или [получить](/graph/api/onlinemeeting-get?view=graph-rest-beta) экземпляр онлайн-собрания. При успешном выполнении операции отображается содержимое свойства **joinInformation** на указанном языке и вариант локали.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [март](changelog.md#march-2020).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте разрешение `Auditlogs.Read.All` для списка [действий входа](/graph/api/resources/signinactivity?view=graph-rest-beta) [пользователя](/graph/api/resources/user?view=graph-rest-beta).
- Используйте разрешение на уровне приложения `PrivilegedAccess.Read.AzureResources` для [управления привилегированными удостоверениями (PIM) ресурсов Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta), чтобы настроить рабочий процесс доступа «точно в срок» для ролей инфраструктуры Azure на уровне группы управления, подписки, группы ресурсов или ресурса.
- Используйте объект [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta), чтобы [получить](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta) или [обновить](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta) предварительно настроенные параметры безопасности по умолчанию, которые защищают организации от распространенных атак.
- Используйте сегмент `identity` при вызове API условного доступа. Например, чтобы [получить](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta) [политику условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta): `GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`.
- Используйте свойство **authenticationRequirement**, чтобы получить наивысший уровень проверки подлинности, необходимый для успешного выполнения всех действий [входа](/graph/api/resources/signin?view=graph-rest-beta).
- Используйте разбивку на страницы при [перечислении событий подготовки](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta) в вашем клиенте.

### <a name="search"></a>Поиск
- Чтобы добавить данные в файле к результатам поиска, просто индексируйте данные как [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta). Тип **externalFile** не рекомендуется.
- [Обновите](/graph/api/externalitem-update?view=graph-rest-beta) [элемент в индексе](/graph/api/resources/externalitem?view=graph-rest-beta), обновив представление элемента в виде обычного текста (представленное свойством **content**) или контейнер свойств элемента (представленный свойством **properties**). При обновлении любого свойства в контейнере свойств перезаписывается весь контейнер свойств, поэтому убедитесь, что все свойства элемента явным образом включены в обновление.
- Проверьте наличие `HTTP 429` и заголовка ответа `Retry-After` после вызова операции [создания](/graph/api/externalconnection-put-items?view=graph-rest-beta), [обновления](/graph/api/externalitem-update?view=graph-rest-beta) или [удаления](/graph/api/externalitem-delete?view=graph-rest-beta) элемента **externalItem**. Самый быстрый способ выполнить восстановление после [регулирования](throttling.md#best-practices-to-handle-throttling) — отложить запросы с помощью задержки `Retry-After`.

### <a name="teamwork"></a>Командная работа
Используйте разрешение на уровне приложения `ChannelMessage.Read.All` для чтения экземпляров [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) в каналах без зарегистрированного пользователя.

### <a name="universal-print"></a>Универсальная печать
Появление [API универсальной печати](universal-print-concept-overview.md), позволяющего пользователям печатать в Интернете или из приложения. API позволяет ИТ-администраторам управлять доступом пользователей и групп к принтерам в облаке Microsoft 365, а также удаленным общим доступом к принтерам для поддерживания доступности, отслеживать состояние принтеров и создавать отчеты о заархивированных заданиях печати и использовании. 

Обратите внимание, что с марта 2020 г. _служба_ универсальной печати доступна в закрытой предварительной версии. Дополнительные сведения об участии см. в статье [Представляем универсальную печать: облачное решение для печати](https://aka.ms/announcinguniversalprint).


## <a name="february-2020-new-and-generally-available"></a>2020 февраля: новая и общедоступная

### <a name="calendar"></a>Календарь
Просмотрите пример [создания события в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md), а также действия и свойства, доступные для делегата, приглашенных и владельца календаря во время этого процесса.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Чтобы повысить безопасность при подписке на [уведомления об изменениях пользовательских данных](webhooks.md), [установите Transport Layer Security (TLS) 1.2](https://docs.microsoft.com/configmgr/core/plan-design/security/enable-tls-1-2) или выше на клиентах и серверах сайтов, используемых в процессе уведомления. Новое требование вводится поэтапно, начиная с 15 февраля 2020 года. К 15 мая 2020 года все конечные точки уведомления должны соответствовать новому требованию TLS. [Узнайте о стадиях развертывания](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) и при необходимости воспользуйтесь новым свойством **latestSupportedTlsVersion** в качестве временного решения, чтобы избежать сбоев подписки до выполнения обновления TLS.
- Используйте соответствующие типы [запроса оценки угроз](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0) для отслеживания угроз от [почты](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0), [файла сообщения электронной почты](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0) (. EML-файл), [файлов вложений электронной почты](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0) (текстовых файлов, файлов Word и двоичных файлов) и [URL-адреса](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0).

### <a name="users"></a>Пользователи
[Повторная обработка](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0) всех назначений лицензий на основе группы для [пользователя](/graph/api/resources/user?view=graph-rest-1.0).


## <a name="february-2020-new-in-preview-only"></a>Февраль 2020: новое только в предварительном просмотре

### <a name="calendar"></a>Календарь
Просмотрите [задачи, поддерживаемые API-интерфейсами предварительного просмотра, которые управляют совместным использованием и делегированием календаря](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Коммуникации из облака

- Используйте новую [запись вызова ](/graph/api/resources/callrecord?view=graph-rest-beta) ресурс, чтобы получить метаданные звонков и собрания по сети в Microsoft Teams и Skype для бизнеса в Организации.
- Для участника собрания используйте свойство **инициатора**, чтобы получить идентификационную информацию инициатора [записи](/graph/api/resources/recordinginfo?view=graph-rest-beta), если таковая имеется.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [Февраль](changelog.md#february-2020)

### <a name="groups"></a>Группы
Используйте метод [ассигнлиценсе](/graph/api/group-assignlicense?view=graph-rest-beta) для назначения лицензий на продукты, такие как Microsoft 365 или Enterprise Mobility + Security, в группу. Поскольку Azure AD обеспечивает назначение лицензий членам группы, для участников, вступающих в группу или покидающих ее, больше не требуется управление лицензиями на индивидуальном уровне.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Установите параметры запроса, утверждения и проверки при создании [политики назначения пакетов доступа](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta).
- Получите доступ к определенным типам [политик для организации](/graph/api/resources/policy-overview?view=graph-rest-beta), используя `/policies`сегмент URL и указав тип политики. Например, организация может применить политику для автоматического выхода пользователя из веб-сеанса после периода бездействия; см. операции CRUD для экземпляров [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta). Это [серьезное изменение](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/), упрощающее обнаружение всех политик путем группировки всех типизированных политик в сегменте `/policies`. Доступ к другим типизированным политикам осуществляется аналогичным образом: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta) и [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta). 
- Используйте уровень приложения и делегированное `Policy.ReadWrite.ApplicationConfiguration`разрешение для операций чтения и записи в [политиках](/graph/api/resources/policy-overview?view=graph-rest-beta) конфигурации приложений, упомянутых в предыдущем пункте.

### <a name="teamwork"></a>Командная работа
- Используйте [уведомления об изменениях,](/graph/api/resources/webhooks?view=graph-rest-beta) всех сообщений канала или всех сообщений в Организации.
- [Отклоните](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta) [запрос на замену смен](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta) другим пользователем в [группе](/graph/api/resources/team?view=graph-rest-beta).

## <a name="january-2020-new-and-generally-available"></a>Январь 2020 г.: новые и общедоступные возможности

### <a name="security"></a>Безопасность
В рамках управления оповещениями используйте метод [обновления оповещений](/graph/api/alert-update?view=graph-rest-1.0) и обновляйте поле **комментариев** как `Closed in IPC` или `Closed in MCAS`.

### <a name="teamwork"></a>Командная работа
Используйте свойство навигации **primaryChannel** [группы](/graph/api/resources/team?view=graph-rest-1.0) для доступа к каналу по умолчанию **General**.

### <a name="users"></a>Пользователи
Чтобы получить доступ к одному или нескольким удостоверениям, которые [пользователь](/graph/api/resources/user?view=graph-rest-1.0) может использовать для входа в учетную запись пользователя Azure AD, используйте свойство **удостоверения **. Удостоверения могут предоставляться поставщиками услуг Майкрософт, организаций или социальных удостоверений, таких как Facebook, Google или Microsoft. Это свойство позволяет пользователю входить в учетную запись пользователя с помощью любого из этих удостоверений.

## <a name="january-2020-new-in-preview"></a>Январь 2020: Новое в предварительной версии

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [Январь](changelog.md#january-2020).


## <a name="december-2019-new-and-generally-available"></a>Декабрь 2019 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Коммуникации из облака
API коммуникаций из облака имеет общедоступное состояние, API ресурсов [call](/graph/api/resources/call?view=graph-rest-1.0) и [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-1.0) [доступны в версии 1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0).

### <a name="education"></a>Образование
Используйте свойство **classSettings**, чтобы управлять параметрами для конкретного класса, например включением отправки еженедельных дайджестов заданий.  Это свойство доступно в ресурсе [team](/graph/api/resources/team?view=graph-rest-1.0), когда команда представляет собой [группу обучения](/graph/api/resources/educationclass?view=graph-rest-1.0).

### <a name="identity-and-access"></a>Удостоверение и доступ 
[При попытке получить объекты-контейнеры с ограниченными разрешениями часть данных возвращается](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects). В качестве примера можно привести экземпляр [группы](/graph/api/resources/group?view=graph-rest-1.0), связанный с [пользователем](/graph/api/resources/user?view=graph-rest-1.0), другую **группу** и [устройство](/graph/api/resources/device?view=graph-rest-1.0). Приложение, у которого есть только разрешения User.Read.All и Group.Read.All, при попытке получить доступ к этому экземпляру **группы** получит объекты **user** и **group**, а также ограниченные данные для объекта **device** (только тип данных и ИД объекта), не включающие значения свойств.

### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика
API аналитики имеет общедоступное состояние. Используйте этот API в рабочих приложениях для определения наиболее релевантных документов, которые:

- [касаются](/graph/api/insights-list-trending?view=graph-rest-1.0) пользователя;
- [используются](/graph/api/insights-list-used?view=graph-rest-1.0) пользователем;
- [к которым предоставлен доступ](/graph/api/insights-list-shared?view=graph-rest-1.0) пользователю или пользователем.

### <a name="reports"></a>Отчеты
Чтобы получить отчеты об использовании Microsoft 365 с помощью разрешений, делегированных пользователем, администраторам необходимо назначить пользователю роль ограниченного администратора Azure AD. Это может быть одна из следующих ролей: администратор организации, администратор Exchange, администратор SharePoint, администратор Lync, глобальный читатель или читатель отчетов. Для получения дополнительных сведений см. [авторизация для API для чтения отчетов об использовании Microsoft 365](reportroot-authorization.md) .

### <a name="toolkit"></a>Набор средств
Выпущен набор средств Microsoft Graph версии 1.1. Список улучшений и исправлений ошибок см. в [разделе за декабрь 2019 г.](changelog.md#december-2019) журнала изменений.

## <a name="december-2019-new-in-preview"></a>Декабрь 2019 г.: новые возможности в предварительной версии

### <a name="cloud-communications"></a>Коммуникации из облака
- Чтобы получить сведения о доступности и текущей активности одного или нескольких пользователей, используйте новый ресурс [presence](/graph/api/resources/presence?view=graph-rest-beta).
- [Удалите](/graph/api/onlinemeeting-delete?view=graph-rest-beta) экземпляр [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta).
- Ознакомьтесь с [разделом за декабрь 2019 г.](changelog.md#december-2019) журнала изменений, чтобы переименовать или удалить несколько элементов ресурсов [call](/graph/api/resources/call?view=graph-rest-beta) и [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta) и обеспечить соответствие версии v1 этих ресурсов.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [декабрь](changelog.md#december-2019)

### <a name="identity-and-access"></a>Удостоверение и доступ 
- Исправлено поведение отношений **appRoleAssignments** и **appRoleAssignedTo** в [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta).
- Используйте [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta) в [функции управления правами в Azure AD](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta) для запроса добавления ресурса к [каталогу](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta), чтобы роли этого ресурса можно было использовать в [пакете для доступа](/graph/api/resources/accesspackage?view=graph-rest-beta).
- Используйте [API оценки угроз](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta), чтобы дать администраторам возможность сообщать о подозрительной почте, URL-адресах фишинга, вложениях электронной почты и других файлах. Вывод, сделанный при сканировании потока, может побудить их изменить политику организации соответствующим образом.

### <a name="teamwork"></a>Командная работа
- [Настройка уведомлений об изменениях, включающих данные](webhooks-with-resource-data.md) для ресурсов [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) в каналах и чатах Microsoft Teams.
- [Подписка на уведомления](/graph/api/resources/subscription?view=graph-rest-beta) о новых и измененных [сообщениях канала или чата](/graph/api/resources/chatmessage?view=graph-rest-beta).
- Используйте ресурс [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta), чтобы включить указание доступности пользователя для назначения смен в [графике](/graph/api/resources/schedule?view=graph-rest-beta). Настройте эту возможность в [параметрах](/graph/api/resources/usersettings?view=graph-rest-beta) пользователя.


## <a name="november-2019-new-and-generally-available"></a>Ноябрь 2019 г.: новые и общедоступные возможности

### <a name="groups"></a>Группы
- Использование разрешений приложения или делегированных разрешений GroupMember.Read.All и GroupMember.ReadWrite.All для перечисления групп, чтения основных свойств групп, считывания (и обновления при наличии разрешения на чтение и запись) сведений об участии в группах, к которым у приложения есть доступ.
- Использование разрешения приложения Group.Create для создания групп без необходимости входа пользователя.
- Для указанной [группы](/graph/api/resources/group?view=graph-rest-1.0) [проверка участия](/graph/api/group-checkmemberobjects?view=graph-rest-1.0) в других группах или ролях каталога.

### <a name="identity-and-access"></a>Идентификация и доступ
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


## <a name="october-2019-new-and-generally-available"></a>Октябрь 2019 г.: новые и общедоступные возможности

### <a name="identity-and-access"></a>Удостоверение и доступ
- Использование [контактов организации](/graph/api/resources/orgcontact?view=graph-rest-1.0) в рабочих приложениях. Контакты организации находятся под управлением администраторов организации и синхронизируются из локальной службы каталогов Active Directory или из Exchange Online.
- Настройка [проверки подлинности на основе сертификатов](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) в [организации](/graph/api/resources/organization?view=graph-rest-1.0).
- Добавление и удаление [учетных данных с паролем](/graph/api/resources/passwordcredential?view=graph-rest-1.0) для [приложений](/graph/api/resources/application?view=graph-rest-1.0).

### <a name="mail"></a>Почта
Использование нового параметра **message** для обновления любых записываемых свойств [message](/graph/api/resources/message?view=graph-rest-1.0) при [ответе](/graph/api/message-reply?view=graph-rest-1.0) на сообщение, например [для добавления получателя в ответ](/graph/api/message-reply#example?view=graph-rest-1.0).

### <a name="microsoft-graph-data-connect"></a>Подключение к данным Microsoft Graph
Разработчики и исследователи данных теперь могут использовать [инструменты для преобразования данных Office 365 в формат общей модели данных](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md). В этом случае обеспечивается согласование схемы данных с другими наборами данных, совместимыми с Open Data Initiative (ODI). 


### <a name="microsoft-graph-sdks"></a>Пакеты SDK Microsoft Graph
- Использование обработчиков хаоса в SDK JavaScript для проверки устойчивости приложения к сбоям серверов, возникающим в трудновоспроизводимых условиях.
- Прочтите о [создании вызовов API с помощью пакетов SDK](/graph/sdks/create-requests).

### <a name="users"></a>Пользователи
- [Получение](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0) или [настройка](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0) параметров предпочитаемого пользователем формата даты и времени [для почтового ящика пользователя](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). 
- Отслеживание даты и времени последнего изменения пароля [пользователя](/graph/api/resources/user?view=graph-rest-1.0).

## <a name="october-2019-new-in-preview"></a>Октябрь 2019 г.: новые возможности в предварительной версии

### <a name="calendar"></a>Календарь
- Организаторы собраний могут [разрешить приглашенным предлагать другое время собраний](outlook-calendar-meeting-proposals.md). При получении ответа на приглашение, содержащего предложение другого времени, организатор может принять предложение и [обновить](/graph/api/event-update?view=graph-rest-beta) время собрания.
- Программное предоставление доступа к календарю с более тесным взаимодействием с использованием пользовательского интерфейса Outlook. Поддерживается отслеживание разрешений текущего пользователя и состояния общего доступа к календарю, а также следующие возможности:
  - Для каждого [календаря](/graph/api/resources/calendar?view=graph-rest-beta) теперь можно управлять [разрешениями](/graph/api/resources/calendarpermission?view=graph-rest-beta) каждого пользователя, которому предоставлен доступ к календарю. 
  - Для каждого [почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-beta) теперь можно указать, кто получает сообщения о собраниях и ответы на эти сообщения: делегат, владелец почтового ящика или и тот, и другой. 
- Дополнительная поддержка собраний по сети:
  - В каждом **календаре** можно указать разрешенных и используемых по умолчанию поставщиков собраний по сети.
  - Можно создать или обновить [мероприятие](/graph/api/resources/event?view=graph-rest-beta), доступное по сети, и предоставить участникам сведения для присоединения к собранию по сети. 
  - В частности, можно использовать **onlineMeetingProvider** и **onlineMeeting** — это новые свойства **мероприятий**, с помощью которых можно задать или указать Microsoft Teams в качестве поставщика собраний по сети. Это временное решение [известной проблемы](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) со свойством **onlineMeetingUrl**.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [октябрь](changelog.md#october-2019)

### <a name="graph-explorer"></a>Песочница Graph
Попробуйте [следующую версию песочницы Graph](https://developer.microsoft.com/graph/graph-explorer/preview) и воспользуйтесь полезной контекстной информацией, включая разрешения, маркеры доступа и фрагменты кода SDK, на новых вкладках **Разрешения**, **Проверка подлинности** и **Фрагменты кода**. С помощью ползунка **просмотра** можно переключаться между [рабочей](https://developer.microsoft.com/graph/graph-explorer) и новой предварительной версией песочницы Graph.

### <a name="groups"></a>Группы
- Управление видимостью [групп](/graph/api/resources/group?view=graph-rest-beta) в определенных частях пользовательского интерфейса Outlook или в клиенте Outlook с помощью свойств **hideFromAddressLists** и **hideFromOutlookClients**.
- [Назначение](/graph/api/group-assignlicense?view=graph-rest-beta) и удаление лицензий пользователям в [группе](/graph/api/resources/group?view=graph-rest-beta).

### <a name="identity-and-access"></a>Идентификация и доступ
- Использование [политик условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) для настройки правил доступа для организации. Эти правила учитывают сигналы о пользователях или об удостоверениях устройств, включая членство пользователей или групп, расположение IP-адреса, а также поведение, включая попытки доступа к определенным приложениям и опасное поведение при входе.
- [Управление правами](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta) можно использовать для управления доступом к группам, приложениям и сайтам SharePoint Online для пользователей внутри организации и вне ее.
- Добавление и удаление [учетных данных с паролем](/graph/api/resources/passwordcredential?view=graph-rest-beta) для [приложений](/graph/api/resources/application?view=graph-rest-beta) и [субъектов-служб](/graph/api/resources/serviceprincipal?view=graph-rest-beta).
- Управление [ключами политики инфраструктуры доверия](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta) Azure AD B2C.
- Можно определить политики [пользовательского процесса](/graph/api/resources/identityuserflow?view=graph-rest-beta) Azure AD B2C для входа, регистрации, объединенной процедуры регистрации и входа, сброса пароля и обновления профиля.
- Настройка [меток защиты информации](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta), чтобы классифицировать конфиденциальность данных для пользователя или клиента.
- Существующие приложения, использующие API для [событий с риском для идентификации](/graph/api/resources/identityriskevent?view=graph-rest-beta), должны перейти на использование функций [обнаружения риска](/graph/api/resources/riskdetection?view=graph-rest-beta) в службе защиты идентификации Azure AD. Дополнительные сведения и график прекращения использования прежнего решения см. в [публикации в блоге](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/).


### <a name="mail"></a>Почта
[Вложение больших файлов размером до 150 МБ](outlook-large-attachments.md) в экземпляр [сообщения](/graph/api/resources/message?view=graph-rest-beta) путем создания [сеанса отправки](/graph/api/resources/uploadsession?view=graph-rest-beta) и итерационной отправки диапазонов файла, пока не отправятся все байты файла. 

### <a name="microsoft-graph-security-api"></a>Microsoft Graph Security API
- Предварительная версия интеграции с RSA NetWitness, ServiceNow и Splunk для сопоставления и синхронизации [оповещений](/graph/api/resources/security-api-overview?view=graph-rest-beta#alerts), улучшения защиты от угроз и реагирования.
- Новые переключатели добавлены в [соединитель безопасности Microsoft Graph](https://docs.microsoft.com/connectors/microsoftgraphsecurity/) и в [сборники схем](https://docs.microsoft.com/azure/security-center/security-center-playbooks) для логических приложений и потоков. См. [примеры сборников схем](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Поддержка отправки [индикаторов угроз](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) в Microsoft Defender ATP для блокирования или отправки оповещений об угрозах с использованием собственных источников аналитики. Интеграция с партнерами, такими как ThreatConnect, дает заказчикам возможность отправлять индикаторы непосредственно из решений аналитики угроз и автоматизации. 

### <a name="notifications"></a>Уведомления
- [Создание и отправка уведомлений](/graph/api/user-post-notifications?view=graph-rest-beta) всем клиентам приложения во всех конечных точках устройств, где пользователи могли войти в систему, без необходимости управлять разрешениями, делегированными пользователями.
- [Целевые конечные точки политики](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta) в [уведомлениях](/graph/api/resources/notification?view=graph-rest-beta) пользователей позволяют целенаправленно управлять уведомлениями на платформах Windows, iOS, Android или WebPush.
- Можно указать [политику отката](/graph/api/resources/fallbackpolicy?view=graph-rest-beta) для уведомлений для конечных точек iOS, чтобы отправлять высокоприоритетные необработанные уведомления, доставка которых на устройства другими способами может быть невозможной из-за ограничений, действующих для конкретной платформы, например, из-за использования режима экономии заряда аккумулятора.

 
### <a name="powershell-sdk"></a>Пакет SDK для PowerShell 
Разработчики и ИТ-специалисты могут обратить внимание на выпуск [пакета SDK Microsoft Graph для Powershell](https://github.com/microsoftgraph/msgraph-sdk-powershell). Этот пакет будет формировать модули, содержащие командлеты для создания запросов API REST Microsoft.

## <a name="september-2019-new-and-generally-available"></a>Сентябрь 2019 г.: новые и общедоступные возможности

### <a name="calendar-mail-and-group"></a>Календарь, почта и группа
[Получение необработанного содержимого файла или содержимого MIME элемента](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment), добавленного в качестве [вложения](/graph/api/resources/attachment?view=graph-rest-1.0) в [событие](/graph/api/resources/event?view=graph-rest-1.0), [сообщение](/graph/api/resources/message?view=graph-rest-1.0) или [запись](/graph/api/resources/post?view=graph-rest-1.0) группы.

### <a name="calendar-mail-outlook-task-personal-contact"></a>Календарь, почта, задача Outlook, личный контакт
Преобразование идентификатора элемента Outlook в поддерживаемые [форматы](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values), включая стандартный и неизменяемый формат идентификаторов Microsoft Graph, с помощью функции [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0). 

Преобразование формата идентификатора поддерживают следующие ресурсы:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0)
- [contact](/graph/api/resources/contact?view=graph-rest-1.0)
- [event](/graph/api/resources/event?view=graph-rest-1.0)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0)
- [message](/graph/api/resources/message?view=graph-rest-1.0)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0)

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

  - Определение операций, которые могут влиять на двоичное содержимое объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta), с помощью нового свойства **pendingOperations**.
  - [Восстановление](/graph/api/driveitem-restore?view=graph-rest-beta) удаленного объекта **driveItem**. 
- Использование защищенного алгоритма хэширования (SHA-256) для улучшения безопасности и целостности данных ресурса [file](/graph/api/resources/file?view=graph-rest-beta).
- Получение или настройка ориентации ресурса [photo](/graph/api/resources/photo?view=graph-rest-beta). Настройка поддерживается в OneDrive персональный.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Использование нового свойства **identities** и получение удостоверений, которые может применять [пользователь](/graph/api/resources/user?view=graph-rest-beta) для входа в учетную запись. Удостоверения могут предоставляться организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт.
- Добавочные улучшения для [синхронизации удостоверений](/graph/api/resources/synchronization-overview?view=graph-rest-beta) в облачном приложении для клиента:

  - Сохранение параметров для [задания синхронизации](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)
  - Указание причины применения [карантина](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta) для задания синхронизации

### <a name="teamwork"></a>Командная работа
Использование канала **Общий** в [команде](/graph/api/resources/team?view=graph-rest-beta) или настройка [параметров участников](/graph/api/resources/teammembersettings?view=graph-rest-beta), чтобы разрешить участникам команд создавать закрытые каналы в **команде**.

### <a name="users"></a>Пользователи
- Получение или обновление удостоверений, с помощью которых [пользователь](/graph/api/resources/user?view=graph-rest-beta) может войти в учетную запись. Эти удостоверения могут предоставляться бизнес-организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт.
- Получение или обновление параметров предпочитаемого пользователем формата даты и времени [для почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-beta).


## <a name="august-2019-new-and-generally-available"></a>Август 2019 г.: новые и общедоступные возможности 

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0) касательно числа и размера удаленных элементов.
- Отслеживайте идентификаторы групп Microsoft 365 при [получения сведений о действиях в группах](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0).
- Отслеживайте имя субъекта-владельца при получении [сведений об использовании хранилища OneDrive учетной записью](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0) и [сведений об использовании сайта SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0).
- Получение числа активных и неактивных пользователей в Microsoft 365 при [получении отчета о счетчиках пользователей для службы microsoft 365](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0).

### <a name="security"></a>Безопасность
- Используйте новую [надстройку Microsoft Graph Security API для Splunk](https://aka.ms/graphsecuritysplunkaddon), чтобы передавать оповещения системы безопасности и аналитику из различных продуктов партнеров в Splunk, облегчая сопоставление их данных по безопасности в режиме реального времени. Дополнительные сведения см. в [объявлении](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972). 
- [Ознакомьтесь со списком других решений и соединителей](security-integration.md), разработанных корпорацией Майкрософт или партнерами Майкрософт, которые подключаются к API безопасности и позволяют работать с данными в едином формате.


## <a name="august-2019-new-in-preview"></a>Август 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [август](changelog.md#august-2019)

### <a name="education"></a>Образование
- Свяжите [преподавателя](/graph/api/resources/educationuser?view=graph-rest-beta) или [задание](/graph/api/resources/educationassignment?view=graph-rest-beta) с [рубрикой оценивания](/graph/api/resources/educationrubric?view=graph-rest-beta), чтобы задать определенные показатели качества и уровни заданий. К примерам показателей качеств относятся орфография и грамматика, а к примерам уровней — "хорошо" и "неудовлетворительно". Кроме того, вы можете связать с рубрикой баллы и веса. Дополнительные сведения см. в [обзоре образовательных рубрик](education-rubric-overview.md).
- Оцените задание и представьте результаты в виде [отзыва](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta), [числовой оценки](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta) или [рубрики](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta).

### <a name="files"></a>Файлы
До этого момента вы могли [отслеживать](/graph/api/driveitem-follow?view=graph-rest-beta) объект [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) для удобного доступа или упрощения таких действий, как перемещение, копирование и сохранение в определенном формате. Теперь вы можете использовать действие [отмены отслеживания](/graph/api/driveitem-unfollow?view=graph-rest-beta), чтобы прекратить отслеживание таких элементов диска.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Поставщики управления доступом на основе ролей (RBAC) могут [управлять ролями](/graph/api/resources/rolemanagement?view=graph-rest-beta) в Azure Active Directory, [определяя действия ролей](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta), которые могут выполняться с определенными ресурсами, и [назначая роли](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta) пользователям в соответствии с этими определениями, чтобы предоставить им доступ к этим ресурсам.
- Администраторы могут [просматривать обзоры доступа](/graph/api/accessreview-list?view=graph-rest-beta), чтобы эффективно проверять членство в группах, доступ к корпоративным приложениям и назначения ролей. Регулярные проверки доступа позволяют гарантировать, что только уполномоченные люди получают постоянный доступ к ресурсам определенными способами.

### <a name="social-and-workplace-intelligence"></a>Социальная и рабочая аналитика
Конечные пользователи могут использовать приложение Microsoft 365 [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) , чтобы получить сведения об управлении временем, совместной работе и балансировке сроков работы. Теперь с помощью [API аналитики](/graph/api/resources/social-overview?view=graph-rest-beta#help-users-gain-insights-into-their-work-patterns) можно интегрировать данные о времени, потраченном на рабочие задачи (например, звонки, чаты и электронную почту), чтобы повысить продуктивность пользователя и улучшить его самочувствие. 


## <a name="july-2019-new-and-generally-available"></a>Июль 2019 г.: новые и общедоступные возможности 

### <a name="example-code-snippets"></a>Примеры фрагментов кода
Теперь имеются фрагменты кода Objective-C для всех статей по API в справочных материалах для версии 1.0 и бета-версии. См. пример Objective-C для [получения события](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="group"></a>Группа
- Используйте функцию [валидатепропертиес](/graph/api/group-validateproperties?view=graph-rest-1.0) , чтобы убедиться, что отображаемое имя или псевдоним почты существующей группы Microsoft 365 соответствует политикам именования.
- Кроме того, перед созданием группы вы можете использовать функцию [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) для объекта [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), чтобы сначала проверить имена.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-1.0) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-1.0).
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#role-management-permissions) _RoleManagement.Read.Directory_ и _RoleManagement.ReadWrite.Directory_ для управления доступом на основе ролей (RBAC) в каталоге компании:

  - Используйте разрешение на чтение и запись, чтобы сначала [активировать](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0) роль каталога. 
  - Если роль активирована, вы можете использовать разрешение на чтение для [чтения ролей каталога](/graph/api/directoryrole-list?view=graph-rest-1.0), [перечисления участников ролей](/graph/api/directoryrole-list-members?view=graph-rest-1.0) и [перечисления шаблонов для ролей каталогов](/graph/api/directoryroletemplate-list?view=graph-rest-1.0). 
  - Вы также можете использовать разрешение на чтение и запись для [добавления](/graph/api/directoryrole-post-members?view=graph-rest-1.0) и [удаления](/graph/api/directoryrole-delete-member?view=graph-rest-1.0) участников ролей.


## <a name="july-2019-new-in-preview"></a>Июль 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="calendar"></a>Календарь 
Используйте новый [API мест](/graph/api/resources/place?view=graph-rest-beta), чтобы применять различные типы расположений, например [помещения](/graph/api/resources/room?view=graph-rest-beta) и [список помещений](/graph/api/resources/roomlist?view=graph-rest-beta), настроенные администраторами Exchange Online.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [июль](changelog.md#july-2019)

### <a name="files"></a>Файлы 
Применяйте дату и время окончания срока действия или пароль при [создании ссылки для общего доступа](/graph/api/driveitem-createlink?view=graph-rest-beta) к файлу, папке или другому объекту [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новое разрешение приложений](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ для операций CRUD при [проверках доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta). 
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#administrative-units-permissions) _AdministrativeUnit.Read.All_ и _AdministrativeUnit.ReadWrite.All_ для чтения и записи (включая создание, обновление и удаление участников, а также управление ими) ресурсов [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta) соответственно.
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-beta) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-beta).
- Используйте новую функцию [обнаружения](/graph/api/directorydefinition-discover?view=graph-rest-beta) для поиска последней [схемы синхронизации](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta) каталога, чтобы синхронизировать объекты каталога, атрибуты и их типы с приложением.
- Используйте [политику развертывания функций](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta), чтобы помочь администраторам клиента выполнить пилотное развертывание функций для определенных групп перед включением их для всей организации.

### <a name="mail"></a>Почта
Используйте более детализированное разрешение приложений _Mail.ReadBasic.All_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Теперь его можно применять в [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) и [отслеживании изменений](delta-query-overview.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta) и объекта **mailFolder**.

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta) касательно числа и размера удаленных элементов.

### <a name="teamwork"></a>Командная работа
- [Устанавливайте](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta), [удаляйте](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta), [обновляйте](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta) и [перечисляйте установленные приложения Microsoft Teams](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) для пользователя.
- Используйте доступ только для приложения, чтобы читать сообщения канала, а также отвечать на сообщения в каналах и беседах. [Запросите и получите утверждение](teams-protected-apis.md) для такого доступа.

## <a name="may---june-2019-new-and-generally-available"></a>Май–июнь 2019 г.: новые и общедоступные возможности

### <a name="calendar-mail-and-personal-contacts"></a>Календарь, почта и личные контакты
Администраторы Exchange могут предоставлять приложению разрешения приложения и [ограничить доступ приложения только к подмножеству почтовых ящиков](auth-limit-mailbox-access.md) вместо доступа ко всем почтовым ящикам в организации, используемого по умолчанию. Такое ограничение доступа будет применено ко всем разрешениям приложения, предоставленным приложению для [календарей](permissions-reference.md#calendars-permissions), [контактов](permissions-reference.md#contacts-permissions), а также [параметров почты и почтового ящика](permissions-reference.md#mail-permissions). См. связанное [объявление в блоге](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/).

### <a name="mail"></a>Почта
Используйте API [папок поиска почты](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0) для поиска сообщений и доступа к результатам поиска по электронной почте Outlook. См. связанное [объявление в блоге](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/).

### <a name="postman"></a>Postman
В качестве альтернативы песочнице Graph используйте API Microsoft Graph в [коллекции Postman Microsoft Graph](use-postman.md), чтобы изучить поведение API и ускорить разработку приложения.

### <a name="tutorials"></a>Учебники
Воспользуйтесь новым [руководством для создания консольного приложения Java](/graph/tutorials/java), чтобы получить информацию о календаре пользователя.

### <a name="user"></a>Пользователь
Администраторы и пользователи могут [отзывать](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) все выданные маркеры обновления для пользователя. Обычно это используется для того, чтобы запретить доступ к данным организации для приложений на потерянных и украденных устройствах.


## <a name="may---june-2019-new-in-preview"></a>Май–июнь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [май](changelog.md#may-2019) 
- Обновления Intune за [июнь](changelog.md#june-2019)

### <a name="education"></a>Образование
- Разностный запрос для [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta).
- Разностный запрос и добавления свойств для [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) и [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta).

### <a name="group"></a>Группа
Получение [меток конфиденциальности](/graph/api/resources/assignedlabel?view=graph-rest-beta) для защиты конфиденциальных данных группы Microsoft 365 и соответствие политикам соответствия требованиям. Эти метки являются объектами [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta), опубликованными администраторами в Центре безопасности и соответствия требованиям Microsoft 365, в рамках возможностей Microsoft Information Protection. 

### <a name="identity-and-access"></a>Удостоверение и доступ
- Получите экземпляр [приложения](/graph/api/resources/applicationtemplate?view=graph-rest-beta) или добавьте экземпляр из коллекции приложений Azure AD в ваш каталог в качестве шаблона.
- Получите журнал всех [событий подготовки](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta) каталога в клиенте.
- Получите сведения об [обнаруженном пользователе или рисках входа в систему](/graph/api/resources/riskdetection?view=graph-rest-beta) в среде Azure AD. Эта функциональность обнаружения рисков является частью Azure AD Identity Protection (Защиты идентификации Azure AD).

### <a name="mail"></a>Почта
Используйте более детализированное делегированное разрешение _Mail.ReadBasic_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Доступно для методов чтения [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) и [отслеживания изменений](delta-query-overview.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta) и объекта **mailFolder**.

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
[Набор средств Microsoft Graph](/graph/toolkit/overview) — это набор не зависящих от платформы веб-компонентов и помощников, обеспечивающий удобную проверку подлинности и доступ к данным в Microsoft Graph.  Так как набор средств Microsoft Graph находится в состоянии предварительной версии, используйте компоненты и поставщиков наборов средств только для тех приложений, которые не предназначены для рабочей среды.

### <a name="reports"></a>Отчеты
- Получайте [отчеты о методах проверки подлинности](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta), используемых пользователями в организации, таких как самостоятельное хранение пароля и многофакторная проверка подлинности (MFA).

### <a name="sites"></a>Сайты
Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-beta) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-beta) сайтов SharePoint. 

### <a name="teamwork"></a>Командная работа
- Размещайте [изображения](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta) в [сообщениях в чатах](/graph/api/resources/chatmessage?view=graph-rest-beta) Microsoft Teams.
- Поддерживайте [настройку](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta) способа обнаружения закрытой команды.


## <a name="january---april-2019-new-and-generally-available"></a>Январь–апрель 2019 г.: новые и общедоступные возможности

[Подключение к данным Microsoft Graph](data-connect-concept-overview.md)

### <a name="calendar"></a>Календарь
[Получение сведений о доступности](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>Удостоверение и доступ
[Поставщики удостоверений](/graph/api/resources/identityprovider?view=graph-rest-1.0)
[Руководство по улучшенной проверке подлинности](/graph/auth)
[Миграция приложений из Azure AD Graph в Microsoft Graph](migrate-azure-ad-graph-overview.md)

### <a name="sdks"></a>Пакеты SDK
[Руководство по пакетам SDK](/sdks/sdks-overview.md) Фрагменты API ([пример](/graph/api/user-get?view=graph-rest-1.0&tabs=cs#sdk-sample-code))

### <a name="security"></a>Безопасность
[Оценка безопасности клиента](/graph/api/resources/securescore?view=graph-rest-1.0)

## <a name="january---april-2019-new-in-preview"></a>Январь–апрель 2019 г.: новые возможности в предварительной версии

### <a name="calendar-group-mail-to-do-tasks"></a>Календарь, группа, почта, задачи To-Do
[Получение необработанного контента или содержимого MIME вложений](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment) для события, сообщения, задачи Outlook или записи в группе

### <a name="change-notifications"></a>Уведомления об изменениях
[Уменьшение числа пропущенных уведомлений об изменениях для ресурсов Outlook](webhooks-outlook-authz.md)

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [январь](changelog.md#january-2019) 
- Обновления Intune за [февраль](changelog.md#february-2019)
- Обновления Intune за [март](changelog.md#march-2019)
- Обновления Intune за [апрель](changelog.md#april-2019)

### <a name="files"></a>Файлы
[Приглашение к совместному использованию](/graph/api/driveitem-invite?view=graph-rest-beta) включает истечение срока его действия и пароль

### <a name="financials"></a>Финансовые показатели
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>Удостоверения и доступ
[Проверки доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta) поддерживают разрешения для приложений [Журналы аудита и входа](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta)
[Настраиваемые вход и регистрация в Azure AD B2C](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)
[Рискованный пользователь](/graph/api/resources/riskyuser?view=graph-rest-beta) и [журнал](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta)

### <a name="mail"></a>Почта
[Получение содержимого MIME сообщений](outlook-get-mime-message.md)

### <a name="reports"></a>Отчеты
[Отчеты о входе в приложение](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)

### <a name="security"></a>Система безопасности
[Действия по обеспечению безопасности](/graph/api/resources/securityaction?view=graph-rest-beta)
[Индикаторы угроз](/graph/api/resources/tiindicator?view=graph-rest-beta)

### <a name="teamwork"></a>Командная работа
[Личные чаты](/graph/api/resources/chat?view=graph-rest-beta)
[Управление сменами](/graph/api/resources/shift?view=graph-rest-beta)

## <a name="see-also"></a>См. также
- Ознакомьтесь [с текущими новыми возможностями](whats-new-overview.md) в Microsoft Graph.
- Периодически просматривайте [блог разработчика, посвященный Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).