---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: c3c777812ca45cc1ad8d28bdbb266b63b0df3880
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764516"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.

## <a name="september-2021-new-and-generally-available"></a>Сентябрь 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Собрания по сети
Используйте `OnlineMeetingArtifact.Read.All` как делегированное разрешение или разрешение приложения для чтения артефактов собраний по сети. Дополнительные сведения см. в статье [Разрешения для собраний по сети](permissions-reference.md#online-meetings-permissions).

### <a name="files"></a>Файлы
- Получите сведения о любом вирусе, обнаруженном в [driveItem](/graph/api/resources/driveItem), с помощью свойства **malware**.
- Используйте функцию [delta](/graph/api/driveitem-delta) для отслеживания изменений как в корневой папке, так и в других папках на диске.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- Поставщики управления доступом на основе ролей (RBAC) могут [управлять ролями](/graph/api/resources/rolemanagement) в Azure Active Directory, [определяя действия ролей](/graph/api/resources/unifiedroledefinition), которые могут выполняться с определенными ресурсами, и [назначая роли](/graph/api/resources/unifiedroleassignment) пользователям в соответствии с этими определениями, чтобы предоставить им доступ к этим ресурсам.

### <a name="search--query"></a>Поиск | Запрос
- Объедините числовые или строковые результаты поиска, импортированные [соединителями Microsoft Graph](/microsoftsearch/connectors-overview) и настроенные как доступные для уточнения в [схеме](/graph/api/resources/schema). Ознакомьтесь с дополнительными сведениями об [уточнении результатов поиска с помощью агрегирования](search-concept-aggregation.md).
- [Сортируйте](/graph/api/resources/search-api-overview#sort-search-results) результаты поиска для OneDrive и SharePoint с помощью любого свойства, поддерживающего сортировку. Дополнительные сведения см. в статье [Использование API Поиска (Майкрософт) для сортировки результатов поиска](search-concept-sort.md).

### <a name="teamwork"></a>Командная работа
- Использование единого действия [provisionEmail](/graph/api/channel-provisionemail) для получения адреса электронной почты ресурса [channel](/graph/api/resources/channel), если таковой существует, или его создания. Использование действия [removeEmail](/graph/api/channel-removeemail) для удаления адреса электронной почты.

### <a name="workbooks-and-charts"></a>Книги и диаграммы
Создавайте строки таблицы асинхронно. Для оптимальной производительности при создании нескольких строк таблицы рекомендуется сгруппировать их в одной операции [create tableRow](/graph/api/table-post-rows) и выполнить операцию асинхронно. Затем выполните операцию [GET workbookOperation](/graph/api/workbookoperation-get) и воспользуйтесь функцией [tableRowOperationResult](/graph/api/workbook-tableRowOperationResult), чтобы получить новый ресурс [workbookTableRow](/graph/api/resources/workbooktablerow).


## <a name="september-2021-new-in-preview-only"></a>Сентябрь 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Собрания по сети
Получите общее число участников в [отчете об участии в собрании](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) для [собрания по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Операция [create case](/graph/api/ediscovery-case-post?view=graph-rest-beta&preserve-view=true) всегда создает дела в большом формате. Это позволяет увеличить размер дела и вместить больший объем данных и большее число элементов. Подробные сведения см. в статье [Преимущества больших дел](/microsoft-365/compliance/advanced-ediscovery-large-cases?view=o365-worldwide&preserve-view=true#benefits-of-large-cases).

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- [Повторно подготовьте облачный ПК](/graph/api/manageddevice-reprovisioncloudpc?view=graph-rest-beta&preserve-view=true) как управляемый в облаке виртуальный рабочий стол, зарегистрированный в Intune.
- [Измените размер облачного ПК](/graph/api/manageddevice-resizecloudpc?view=graph-rest-beta&preserve-view=true) путем перехода на использование более ранней или поздней конфигурации с новым виртуальным ЦП и размером хранилища.

### <a name="education"></a>Образование
Поддержка добавления заданий только в календари учащихся при использовании заголовка запроса `Prefer: include-unknown-enum-members` в операциях для ресурса [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) или [educationAssignmentDefaults](/graph/api/resources/educationassignmentdefaults?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
[Удалите](/graph/api/accesspackageassignmentrequest-delete?view=graph-rest-beta&preserve-view=true) [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true), чтобы удалить отклоненный или выполненный запрос.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход
Разрешите пользователям выполнять многофакторную проверку подлинности с помощью [OATH-токена программного обеспечения](/graph/api/resources/softwareOathAuthenticationMethod?view=graph-rest-beta&preserve-view=true). OATH-токен программного обеспечения — это генератор номеров на основе программного обеспечения, использующий стандарт TOTP (Time-Based One-Time Password).


## <a name="august-2021-new-and-generally-available"></a>Август 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
[Участник](/graph/api/resources/participant) может включить метаданные как большой двоичный объект данных в список участников [звонка](/graph/api/resources/call).

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Собрания по сети
- Создайте [собрание по сети](/graph/api/resources/onlinemeeting) в виде трансляции, настроив [параметры трансляции](/graph/api/resources/broadcastMeetingSettings) и [сведения об участниках собрания](/graph/api/resources/meetingparticipantinfo) с помощью роли организатора. См. [пример](/graph/api/application-post-onlinemeetings#example-2-create-a-live-event-with-user-token).
- Включите или отключите чат либо ограничьте его длительность для онлайн-собрания с помощью свойства **allowMeetingChat**.
- Включите или отключите реакции для онлайн-собрания с помощью свойства **allowTeamworkReactions**.
- Разрешите участнику включить камеру или микрофон с помощью свойства **allowAttendeeToEnableCamera** или **allowAttendeeToEnableMic** соответственно.

### <a name="cloud-communications--presence"></a>Облачные коммуникации | Присутствие
- [Задайте состояние присутствия пользователя](/graph/api/presence-setpresence), являющееся агрегированным состоянием для каждого клиента Teams (классического, мобильного или веб-клиента).
- [Очистите сеанс присутствия](/graph/api/presence-clearpresence) пользователя.


### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune для версии 1.0. Присвойте фильтру **Дата** значение "Август 2021 г." и найдите раздел с таким заголовком.

### <a name="devices-and-apps--service-health-and-communications"></a>Устройства и приложения | Работоспособность и взаимодействие служб
Общедоступная версия [API взаимодействия служб](service-communications-concept-overview.md) в Microsoft Graph для доступа к состоянию работоспособности и записям центра сообщений об облачных службах (Майкрософт).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Получите коллекцию областей проверки доступа, в которой определены проверяющие и запасные проверяющие для [экземпляра проверки доступа](/graph/api/resources/accessReviewInstance).

### <a name="sites-and-lists--taxonomy"></a>Сайты и списки | Таксономия
Доступ к таксономии [банка терминов](/graph/api/resources/termstore-store) SharePoint — иерархии, состоящей из ресурсов [group](/graph/api/resources/termstore-group), [set](/graph/api/resources/termstore-set) и [term](/graph/api/resources/termstore-term), а также ресурсов [relation](/graph/api/resources/termstore-relation) для связей между терминами.

### <a name="teamwork"></a>Командная работа
[Перечислите чаты](/graph/api/chat-list), участником которых является пользователь, в делегированном контексте.

## <a name="august-2021-new-in-preview-only"></a>Август 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
- Поставьте [участника](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true) на удержание и воспроизводите музыку в фоновом режиме с помощью действия [startHoldMusic](/graph/api/participant-startHoldMusic?view=graph-rest-beta&preserve-view=true).
- Повторно добавьте в вызов участника, ранее поставленного на удержание, с помощью действия [stopHoldMusic](/graph/api/participant-stopHoldMusic?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Собрания по сети
Настройте автоматическую запись [собрания по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true)

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
[Окончание льготного периода](/graph/api/cloudPC-endGracePeriod?view=graph-rest-beta&preserve-view=true) для облачного ПК. Льготный период обеспечивает доступ пользователей к облачным ПК в течение семи дней до отмены подготовки. В случае окончания льготного периода подготовка облачного ПК будет отменена сразу же, до истечения семи дней.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune для бета-версии. Присвойте фильтру **Дата** значение "Август 2021 г." и найдите раздел с таким заголовком.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- [Повторно обработайте](/graph/api/accesspackageassignmentrequest-reprocess?view=graph-rest-beta&preserve-view=true) запрос[ на назначение пакета доступа](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true), чтобы автоматически повторить попытку выполнения запроса пользователя на доступ к пакету.
- [Повторно обработайте](/graph/api/accesspackageassignment-reprocess?view=graph-rest-beta&preserve-view=true) запрос[ на назначение пакета доступа](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true), чтобы автоматически проверить назначения пользователя и обеспечить их выполнение.
- [Получите набор требований политики](/graph/api/accesspackage-getapplicablepolicyrequirements?view=graph-rest-beta&preserve-view=true) чтобы создать [запрос назначения для пакета доступа](/graph/api/resources/accesspackageassignmentrequestrequirements?view=graph-rest-beta&preserve-view=true).
- Получите коллекцию ресурсов [проверки доступа и проверяющих](/graph/api/resources/accessreviewreviewer?view=graph-rest-beta&preserve-view=true), где определены проверяющие, с которыми будет установлена связь для [экземпляра проверки доступа](/graph/api/resources/accessReviewInstance?view=graph-rest-beta&preserve-view=true).
- Получите или задайте длительность бездействия, на основе которого будут настраиваться рекомендации, в разделе [параметров расписания проверки доступа](/graph/api/resources/accessReviewScheduleSettings?view=graph-rest-beta&preserve-view=true), используя свойство **recommendationLookBackDuration**.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Организации могут использовать [политики для применения рекомендованных методик для приложений, использующих методы проверки подлинности приложений](/graph/api/resources/applicationauthmethodpolicy?view=graph-rest-beta&preserve-view=true). Такие политики могут применяться к [приложениям и субъектам-службам](/graph/api/resources/appmanagementpolicy?view=graph-rest-beta&preserve-view=true) или [всем приложениям и субъектам-службам в клиенте](/resources/tenantappmanagementpolicy?view=graph-rest-beta&preserve-view=true).
- Поддержка страниц в свойстве навигации **appRoleAssignments** для [пользователей](/api/user-list-approleassignments?view=graph-rest-beta&preserve-view=true), [групп](/api/group-list-approleassignments?view=graph-rest-beta&preserve-view=true) и [субъектов-служб](/api/serviceprincipal-list-approleassignments?view=graph-rest-beta&preserve-view=true).
- Разрешите клиенту Azure Active Directory (Azure AD) настроить [федерацию с другой организацией, поставщик удостоверений (IdP) которой поддерживает протокол SAML или WS-Fed](/graph/api/resources/samlOrWsFedExternalDomainFederation?view=graph-rest-beta&preserve-view=true). Это позволит клиенту Azure AD предоставить доступ к своим ресурсам гостевым пользователям.

### <a name="teamwork"></a>Командная работа
- Получите [сведения о собрании по сети](/graph/api/resources/teamworkOnlineMeetingInfo?view=graph-rest-beta&preserve-view=true), связанные с [чатом](/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- Получите идентификатор клиента, в котором создается **чат**.

### <a name="users"></a>Пользователи
Используйте последние значения даты и времени интерактивного и неинтерактивного входа для [signInActivity](/graph/api/resources/signInActivity?view=graph-rest-beta&preserve-view=true) пользователей, чтобы [управлять неактивными учетными записями](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).

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
