---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: a1934b1cc52ba26f6500ca585c76df3d9f85fb94
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890411"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.


## <a name="october-2021-new-and-generally-available"></a>Октябрь 2021 г. Новые и общедоступные

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
- [Передача](/graph/api/call-transfer) активного однорангового звонка.
- Передача группового звонка указанному участнику (принимающему).

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Онлайн-собрания
Поддержка нескольких платных и бесплатных номеров для телефонного подключения к конференции ([аудиоконференции](/graph/api/resources/audioConferencing)) [виртуального собрания](/graph/api/resources/onlinemeeting).

<!-- Hold off until permissions are deployed
As part of [privacy management in Microsoft 365](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true), subject rights request now debuts in both v1 and beta endpoints of Microsoft Graph. The [subject rights request API](/graph/api/resources/subjectrightsrequest) lets users make requests to review or manage their personal data in their organizations. It also lets organizations automate and scale managing these requests, helping them to meet industry regulations more efficiently.
-->

### <a name="education"></a>Образование
Поддержка [мультимедийных](/graph/api/resources/educationMediaResource) файлов или другого [внешнего ролевого ресурса](/graph/api/resources/educationExternalResource) в качестве [ресурса назначения](/graph/api/resources/educationassignmentresource).

### <a name="identity-and-access--applications"></a>Удостоверение и доступ | Приложения
- Чтобы обеспечить согласованное взаимодействие с [приложением](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true), укажите [ресурсы, к которые приложение должно получить доступ](/graph/api/resources/requiredresourceaccess?view=graph-rest-beta&preserve-view=true), включая набор делегированных разрешений OAuth 2.0 и ролей приложения, которые ему требуются.
- Ограничение числа необходимых API до 50, а необходимых разрешений — до 400 для каждого приложения.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- Установите [атрибуты расширения](/graph/api/resources/onpremisesextensionattributes) для [устройства](/graph/api/resources/device) и управляйте ими в Azure Active Directory при [создании](/graph/api/device-post-devices) или [обновлении](/graph/api/device-update) устройства.
- [Получите ключ восстановления BitLocker](/graph/api/bitlockerrecoverykey-get) от имени вошедшего пользователя, который является владельцем устройства или выполняет соответствующую роль. При получении ключа восстановления создается [журнал аудита](/azure/active-directory/reports-monitoring/concept-audit-logs) наравне с пользовательским интерфейсом.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Укажите список дополнительных пользователей или участников группы, которых нужно уведомлять о ходе выполнения проверки доступа, в свойстве **additionalNotificationRecipients** в [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Укажите устройства в [политике условного доступа](/graph/api/resources/conditionalaccesspolicy) как часть [условий](/graph/api/resources/conditionalAccessConditionSet), которые управляют временем применения политики.

### <a name="personal-contacts"></a>Личные контакты
Включите поддержку делегированных разрешений (`Contacts.Read` или `Contacts.ReadWrite`) для ресурсов [profilePhoto](/graph/api/resources/profilephoto?view=graph-rest-beta&preserve-view=true) в персональных учетных записях Microsoft.

### <a name="teamwork"></a>Teamwork
- [Получение всех сообщений чатов во всех каналах](/graph/api/channel-getallmessages) в [команде](/graph/api/resources/team).
- [Получение всех сообщений из всех чатов](/graph/api/chats-getallmessages), в которых участвует пользователь, включая приватные чаты, групповые чаты и чаты собраний.
- Ознакомьтесь с [моделями лицензирования и оплаты](teams-licenses.md), которые применяются к API Microsoft Teams в Microsoft Graph.

### <a name="users"></a>Пользователи
В пользовательских лицензиях для служб Azure Active Directory (Azure AD) теперь поддерживаются метки времени последнего обновления [состояния назначения лицензии](/graph/api/resources/licenseassignmentstate). 

## <a name="october-2021-new-in-preview-only"></a>Октябрь 2021 г.: новые возможности только в предварительном просмотре

### <a name="applications"></a>Приложения
Используйте [учетные данные федеративного удостоверения](/graph/api/resources/federatedidentitycredential?view=graph-rest-beta&preserve-view=true), чтобы управлять учетными данными приложения и разрешить облачным приложениям организации получать доступ к Azure AD без использования секретов и сертификатов.

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
Определение [участника](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true) звонка с помощью свойства **participantId** в типе ресурса [participantInfo](/graph/api/resources/participantInfo?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Онлайн-собрания
Включение [регистрации собрания](/graph/api/resources/meetingregistration?view=graph-rest-beta&preserve-view=true) и организация собраний по сети в виде [вебинара.](/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3) Привязка собрания к странице регистрации и регистрация всех или только представителей организации как [зарегистрированных участников собрания](/graph/api/resources/meetingregistrant?view=graph-rest-beta&preserve-view=true). 

### <a name="customer-booking"></a>Резервирование для пользователей
- Поддержка следующих атрибутов для [службы бронирования](/graph/api/resources/bookingService?view=graph-rest-beta&preserve-view=true):
  - Включение отправки SMS-уведомлений клиентам для их встреч (**свойство smsNotificationsEnabled**).
  - URL-адрес, который клиенты могут использовать для доступа к службе (свойство **webUrl**).
- Бронирование [встречи](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true) с использованием одного или нескольких следующих атрибутов:
  - Указание часового пояса клиента (свойство **customerTimeZone**).
  - Указание URL-адреса для встречи в сети (свойство **joinWebUrl**).
  - Включение SMS-уведомлений клиенту для встречи (свойство **smsNotificationsEnabled**).
- Указание одного или нескольких адресов или номеров телефона для [клиента](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true).
- Указание часового пояса для [сотрудника](/graph/api/resources/bookingStaffMember?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
[Составление списка](/graph/api/virtualendpoint-list-serviceplans?view=graph-rest-beta&preserve-view=true) [планов служб Windows 365](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true), на которые организация подписалась для своих облачных ПК. В соответствии с каждым [типом плана обслуживания](/graph/api/resources/cloudPcServicePlan?view=graph-rest-beta&preserve-view=true#cloudpcserviceplantype-values) (бизнес или предприятие) организация может выбрать подписку из ряда конфигураций плана, которые различаются по таким атрибутам, как виртуальный ЦП, ОЗУ и хранилище.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Указание [параметров конфигурации учетных данных ключей](/graph/api/resources/keycredentialconfiguration?view=graph-rest-beta&preserve-view=true), которые можно [настроить для применения ограничений в приложении или субъект-службе](/graph/api/resources/appmanagementconfiguration?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Включение следующих дополнительных [параметров](/graph/api/resources/assignmentReviewSettings?view=graph-rest-beta&preserve-view=true) для проверки [политики назначения пакета для доступа](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true):
- Поведение по умолчанию, если запрос не проверяется я в указанный срок (свойство **accessReviewTimeoutBehavior**).
- Отображение рекомендаций проверяющему (свойство **isAccessRecommendationEnabled**).
- Требование, чтобы проверяющий предоставил обоснование для утверждения (свойство **isApprovalJustificationRequired**).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Указание, нужно ли переносить или уже перенесли параметры [политики непрерывной оценки доступа](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) в [политику условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- В рамках [условного доступа](/azure/active-directory/conditional-access/overview) Azure Active Directory используйте новое средство контроля сеанса, [continuousAccessEvaluationSessionControl](/graph/api/resources/continuousAccessEvaluationSessionControl?view=graph-rest-beta&preserve-view=true), для непрерывной оценки доступа и принятия решений о доступе.

### <a name="search--index"></a>Поиск | Индекс
- Указание [параметров](/graph/api/resources/externalconnectors-searchsettings?view=graph-rest-beta&preserve-view=true) для возможностей поиска контента во [внешнем подключении](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true). Например, [шаблон отображения](/graph/api/resources/externalconnectors-displaytemplate?view=graph-rest-beta&preserve-view=true) результатов поиска и [правило](/graph/api/resources/externalconnectors-propertyRule?view=graph-rest-beta&preserve-view=true) для выбора шаблона отображения.
- Связывание одной или нескольких [внешних групп](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-beta&preserve-view=true) со внешним [подключением](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true). Например, внешняя группа, например бизнес-подразделение или рабочая группа, может определять разрешения на контент в источнике данных, представленном внешним подключением.
- Можно дополнительно указать ID приложения Teams во [внешнем подключении](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true) в свойстве **connectorId**.

### <a name="users"></a>Пользователи
[Проверка пароля](/graph/api/user-validatePassword?view=graph-rest-beta&preserve-view=true) в реальном времени относительно политики проверки паролей в организации во время ввода пароля пользователем. Получение [подробных сведений о проверке](/graph/api/resources/passwordValidationInformation?view=graph-rest-beta&preserve-view=true) относительно правил в политике.


## <a name="september-2021-new-and-generally-available"></a>Сентябрь 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
- Поставьте [участника](/graph/api/resources/participant) на удержание и воспроизводите музыку в фоновом режиме с помощью действия [startHoldMusic](/graph/api/participant-startHoldMusic).
- Повторно добавьте в вызов участника, ранее поставленного на удержание, с помощью действия [stopHoldMusic](/graph/api/participant-stopHoldMusic).

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Собрания по сети
- Получение потока контента отчета участника о [трансляции Teams](/microsoftteams/teams-live-events/what-are-teams-live-events).
- Получение или установка параметра для автоматической записи [виртуального собрания](/graph/api/resources/onlineMeeting).
- Используйте `OnlineMeetingArtifact.Read.All` как делегированное разрешение или разрешение приложения для чтения артефактов собраний по сети. Дополнительные сведения см. в статье [Разрешения для собраний по сети](permissions-reference.md#online-meetings-permissions).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
Состояние облачного принтера включает все стандартные значения в [протоколе IPP](https://www.iana.org/assignments/ipp-registrations/ipp-registrations.xhtml).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune за сентябрь для версии 1.0. В [changelog](https://developer.microsoft.com/graph/changelog) установите фильтр **Дата** на сентябрь 2021 г. и найдите раздел с таким же заголовком.

### <a name="files"></a>Файлы
- Получите сведения о любом вирусе, обнаруженном в [driveItem](/graph/api/resources/driveItem), с помощью свойства **malware**.
- Используйте функцию [delta](/graph/api/driveitem-delta) для отслеживания изменений как в корневой папке, так и в других папках на диске.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Поставщики управления доступом на основе ролей (RBAC) могут [управлять ролями](/graph/api/resources/rolemanagement) в Azure Active Directory, [определяя действия ролей](/graph/api/resources/unifiedroledefinition), которые могут выполняться с определенными ресурсами, и [назначая роли](/graph/api/resources/unifiedroleassignment) пользователям в соответствии с этими определениями, чтобы предоставить им доступ к этим ресурсам.

### <a name="search--query"></a>Поиск | Запрос
- Объедините числовые или строковые результаты поиска, импортированные [соединителями Microsoft Graph](/microsoftsearch/connectors-overview) и настроенные как доступные для уточнения в [схеме](/graph/api/resources/schema). Ознакомьтесь с дополнительными сведениями об [уточнении результатов поиска с помощью агрегирования](search-concept-aggregation.md).
- [Сортируйте](/graph/api/resources/search-api-overview#sort-search-results) результаты поиска для OneDrive и SharePoint с помощью любого свойства, поддерживающего сортировку. Дополнительные сведения см. в статье [Использование API Поиска (Майкрософт) для сортировки результатов поиска](search-concept-sort.md).

### <a name="teamwork"></a>Командная работа
Использование единого действия [provisionEmail](/graph/api/channel-provisionemail) для получения адреса электронной почты ресурса [channel](/graph/api/resources/channel), если таковой существует, или его создания. Использование действия [removeEmail](/graph/api/channel-removeemail) для удаления адреса электронной почты.

### <a name="workbooks-and-charts"></a>Книги и диаграммы
Создавайте строки таблицы асинхронно. Для оптимальной производительности при создании нескольких строк таблицы рекомендуется сгруппировать их в одной операции [create tableRow](/graph/api/table-post-rows) и выполнить операцию асинхронно. Затем выполните операцию [GET workbookOperation](/graph/api/workbookoperation-get) и воспользуйтесь функцией [tableRowOperationResult](/graph/api/workbook-tableRowOperationResult), чтобы получить новый ресурс [workbookTableRow](/graph/api/resources/workbooktablerow).


## <a name="september-2021-new-in-preview-only"></a>Сентябрь 2021 г.: новые возможности только в предварительной версии

### <a name="applications"></a>Приложения
Приложения, в которых используются потоки единого входа на языке SAML, могут указывать URI перенаправления по умолчанию (свойство **defaultRedirectUri** в [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)) или определять указанный URI перенаправления, при котором пользователей перенаправляют для входа (свойство **redirectUriSettings** в [webApplication](/graph/api/resources/webapplication?view=graph-rest-beta&preserve-view=true)). 

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Собрания по сети
Получите общее число участников в [отчете об участии в собрании](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) для [собрания по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Операция [create case](/graph/api/ediscovery-case-post?view=graph-rest-beta&preserve-view=true) всегда создает дела в большом формате. Это позволяет увеличить размер дела и вместить больший объем данных и большее число элементов. Подробные сведения см. в статье [Преимущества больших дел](/microsoft-365/compliance/advanced-ediscovery-large-cases?view=o365-worldwide&preserve-view=true#benefits-of-large-cases).

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- [Повторно подготовьте облачный ПК](/graph/api/manageddevice-reprovisioncloudpc?view=graph-rest-beta&preserve-view=true) как управляемый в облаке виртуальный рабочий стол, зарегистрированный в Intune.
- [Измените размер облачного ПК](/graph/api/manageddevice-resizecloudpc?view=graph-rest-beta&preserve-view=true) путем перехода на использование более ранней или поздней конфигурации с новым виртуальным ЦП и размером хранилища.
- [Настройка,](/graph/api/virtualendpoint-post-onpremisesconnections?view=graph-rest-beta&preserve-view=true) [составление списка](/graph/api/virtualendpoint-list-onpremisesconnections?view=graph-rest-beta&preserve-view=true) и [проверка работоспособности](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) [локальных сетевых подключений](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) для подготовки облачных ПК.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune за сентябрь для бета-версии. В [changelog](https://developer.microsoft.com/graph/changelog) установите фильтр **Дата** на сентябрь 2021 г. и найдите раздел с таким же заголовком.

### <a name="education"></a>Образование
- Разрешение преподавателям [переназначать](/graph/api/educationsubmission-reassign?view=graph-rest-beta&preserve-view=true) [отправку](/graph/api/resources/educationsubmission?view=graph-rest-beta&preserve-view=true) назначения учащемуся с отзывом для проверки.
- Поддержка добавления заданий только в календари учащихся при использовании заголовка запроса `Prefer: include-unknown-enum-members` в операциях для ресурса [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) или [educationAssignmentDefaults](/graph/api/resources/educationassignmentdefaults?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
[Удалите](/graph/api/accesspackageassignmentrequest-delete?view=graph-rest-beta&preserve-view=true) [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true), чтобы удалить отклоненный или выполненный запрос.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход
- Разрешите пользователям выполнять многофакторную проверку подлинности с помощью [OATH-токена программного обеспечения](/graph/api/resources/softwareOathAuthenticationMethod?view=graph-rest-beta&preserve-view=true). OATH-токен программного обеспечения — это генератор номеров на основе программного обеспечения, использующий стандарт TOTP (Time-Based One-Time Password).
- Определение, включено или отключено соответствие чисел для многофакторной проверки подлинности согласно политике в Azure AD, с помощью свойства **numberMatchingRequiredState** в [microsoftAuthenticatorAuthenticationMethodTarget](/graph/api/resources/microsoftAuthenticatorAuthenticationMethodTarget?view=graph-rest-beta&preserve-view=true).
- Определение, следует ли показывать дополнительный контекст пользователя в его уведомлении приложения для проверки подлинности, с помощью свойства **displayAppInformationRequiredState** в [microsoftAuthenticatorAuthenticationMethodTarget](/graph/api/resources/microsoftAuthenticatorAuthenticationMethodTarget?view=graph-rest-beta&preserve-view=true).
- Использование [потока пользователя B2C](/graph/api/resources/b2cidentityuserflow?view=graph-rest-beta&preserve-view=true) и [потока пользователя для регистрации и самообслуживания](/graph/api/resources/b2xidentityuserflow?view=graph-rest-beta&preserve-view=true) вместо API более раннего нерекомендованного [потока пользователя](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true).

### <a name="security--attack-simulation-and-training"></a>Безопасность | Имитация атак и обучение
Первое использование API для [имитации атак и обучения](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true) — служба, доступная как часть [Microsoft Defender для Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true). API позволяет администраторам клиентов [составлять список запущенных упражнений и тренингов по симуляции](/graph/api/attacksimulationroot-list-simulations?view=graph-rest-beta&preserve-view=true) и получать [отчеты](/graph/api/resources/report-m365defender-reports-overview?view=graph-rest-beta&preserve-view=true) об аналитике поведения пользователей в Интернете в условиях симуляции фишинга.

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
