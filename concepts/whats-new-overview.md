---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: a19df8d75063cf36d99e9023b029c8619c4dd4fb
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289406"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API представлен в разделах " [Май](changelog.md#may-2020) " и " [Апрель](changelog.md#april-2020) " журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="may-2020-new-and-generally-available"></a>Май 2020: новый и обычно доступный

### <a name="calendar--place"></a>Календарь | Место
GA API для почтовых [мест](/graph/api/resources/place) в версии 1.0 используйте этот API в производственных приложениях для получения, обновления или удаления [комнаты](/graph/api/resources/room) или [списка помещений](/graph/api/resources/roomlist) в клиенте. [Узнайте больше](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) об API мест.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Intune [можно](changelog.md#may-2020) обновить в версии 1.0.

### <a name="graph-explorer"></a>Песочница Graph
Используйте многие новые возможности [проводника Graph](https://developer.microsoft.com/en-us/graph/graph-explorer) , которые улучшают обучение и создание прототипов в песочнице. Пример
- Просмотрите фрагменты кода, соответствующие введенному запросу REST API, в C#, Java, JavaScript и целевом языке C.
- Войти в систему с помощью клиента, просмотреть и скопировать маркер доступа в ваше клиентское приложение REST.

Для получения дополнительных сведений см. [новый проводник Graph](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/) .

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


## <a name="may-2020-new-in-preview-only"></a>Май 2020: новый только предварительный просмотр

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
- В рамках [API защиты удостоверений](/graph/api/resources/identityprotection-root?view=graph-rest-beta)используйте свойство **рискевенттипе** , чтобы [получить тип обнаруженного риска](/graph/api/riskdetection-get?view=graph-rest-beta), или [Получите тип риска в журнале пользователя](/graph/api/riskyuser-list-history?view=graph-rest-beta). Не используйте свойство **рисктипе** , так как оно является устаревшим.
- Укажите типы клиентских приложений в свойстве **клиентапптипес** [набора условий](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta) для [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta).

### <a name="teamwork"></a>Командная работа
Приложения Teams, [поддерживающие единый вход (SSO)](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) , могут указывать значение `WebApplicationInfo.id` из манифеста приложения Teams в свойстве **азуреадаппид** объекта [теамсаппдефинитион](/graph/api/resources/teamsappdefinition?view=graph-rest-beta).


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

### <a name="reports--office-365-usage-reports"></a>Отчеты | Отчеты об использовании Office 365
Просмотр данных о **созданных собраниях** и **действиях с уведомлениями о собраниях** в отчетах CSV, включающих [счетчики действий с электронной почтой](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta), [счетчики пользователей, совершающих действия с электронной почтой](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) и [данные о действиях пользователей с электронной почтой](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta).


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

