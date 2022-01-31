---
title: Обзор предыдущих выпусков Microsoft Graph
description: Новые возможности в предыдущих выпусках Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 018d206a1fec429934334289bcc66ab2157b06b9
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282025"
---
# <a name="highlights-of-earlier-releases"></a>Обзор предыдущих выпусков

## <a name="november-2021-new-and-generally-available"></a>Ноябрь 2021 г.: новые и общедоступные возможности

### <a name="files"></a>Файлы
Узнайте состояние диска на определенный момент времени, указав соответствующую метку времени, зашифрованную в виде URL-адреса. См. [пример](/graph/api/driveitem-delta#example-4-retrieving-delta-results-using-a-timestamp).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход
- Запустите [кампании](/graph/api/resources/authenticationMethodsRegistrationCampaign) и [заставьте пользователей регистрироваться](/graph/api/resources/registrationEnforcement) во время регистрации, чтобы настроить целевые методы проверки подлинности.
-  Настройте [поставщика удостоверений Apple](/graph/api/resources/applemanagedidentityprovider) в клиенте Azure AD B2C.

## <a name="november-2021-new-in-preview-only"></a>Ноябрь 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
Автоматический допуск новых типов участников в собрания по сети в обход "зала ожидания" собрания.
- Только пользователи, которых приглашает организатор.
- Только участники из одной и той же компании.

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- Определите [конфигурацию](/graph/api/resources/cloudPcDomainJoinConfiguration?view=graph-rest-beta&preserve-view=true) того, как подготовленное устройство с облачным компьютером может присоединиться к Azure Active Directory (Azure AD): только в облаке и присоединиться только к Azure AD, или в гибридной системе и присоединиться к локальной службе Active Directory и Azure AD.
- Получите [ресурс образа коллекции](/graph/api/resources/cloudPcGalleryImage?view=graph-rest-beta&preserve-view=true) текущей организации, который можно использовать для подготовки облачного компьютера к работе.

### <a name="devices-and-apps--device-updates"></a>Устройства и приложения | Обновления устройств
- Используйте [параметры мер безопасности](/graph/api/resources/windowsupdates-safeguardSettings?view=graph-rest-beta&preserve-view=true), чтобы отказаться от защиты от вероятных проблем при развертывании.
- Поддержка [состояния развертывания](/graph/api/resources/windowsupdates-deploymentState?view=graph-rest-beta&preserve-view=true) при невозможности развертывания из-за того, что содержимое больше не может быть развернуто, например после окончания обслуживания.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- Определите и назначьте [настраиваемые атрибуты безопасности](/graph/api/resources/custom-security-attributes-overview?view=graph-rest-beta&preserve-view=true) объектам Azure AD. Используйте эти атрибуты для хранения информации, классификации объектов или применения детального контроля доступа к определенным ресурсам Azure. Используйте эти атрибуты вместе с [контролем доступа на основе атрибутов Azure](/azure/role-based-access-control/conditions-overview) (Azure ABAC).
- [Создайте группу в административной единице](/graph/api/administrativeunit-post-members?view=graph-rest-beta&preserve-view=true).

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
[Отчеты об использовании Microsoft 365](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true) в типе вывода JSON больше не строго типизированы и имеют тип `Edm.Stream`. Подробности см. в статье [Изменение свойств OData в API отчетов об использовании Microsoft 365 в Microsoft Graph](https://devblogs.microsoft.com/microsoft365dev/odata-property-changes-to-microsoft-365-usage-reports-api-in-microsoft-graph/).

### <a name="teamwork"></a>Teamwork
Отметьте чат как [прочитанный](/graph/api/chat-markChatReadForUser?view=graph-rest-beta&preserve-view=true) или [непрочитанный](/graph/api/chat-markchatunreadforuser?view=graph-rest-beta&preserve-view=true) для пользователя.


## <a name="october-2021-new-and-generally-available"></a>Октябрь 2021 г. Новые и общедоступные

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
- [Передача](/graph/api/call-transfer) активного однорангового звонка.
- Передача группового звонка указанному участнику (принимающему).

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Онлайн-собрания
Поддержка нескольких платных и бесплатных номеров для телефонного подключения к конференции ([аудиоконференции](/graph/api/resources/audioConferencing)) [виртуального собрания](/graph/api/resources/onlinemeeting).

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


## <a name="july-2021-new-and-generally-available"></a>Июль 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
Поддержка ограничения емкости для количества участников, которое приложение может обрабатывать при [ответе](/graph/api/call-answer) на [вызов](/graph/api/resources/call), в организациях, внедряющих [запись звонков на основе политики Teams](/microsoftteams/teams-recording-policy).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Общедоступные поставщики удостоверений с общим базовым типом [identityProviderBase](/graph/api/resources/identityproviderbase):
  - Встроенные поставщики удостоверений для сценариев Azure AD B2B в клиенте Azure AD. Эти поставщики могут поддерживать Azure AD, учетную запись Майкрософт (MSA) или разовые коды доступа, отправляемые по электронной почте.
  - Поставщики социальных удостоверений в клиенте Azure AD B2C, позволяющие пользователям зарегистрироваться и войти в службу с помощью учетной записи социальных сетей, например Microsoft, Google, Facebook, Amazon, LinkedIn или Twitter.
- Не рекомендуется пользование предыдущими API [поставщика удостоверений](/graph/api/resources/identityprovider).

### <a name="users"></a>Пользователи
Позвольте пользователям [менять собственный пароль](/graph/api/user-changepassword) без роли администратора.


## <a name="july-2021-new-in-preview-only"></a>Июль 2021 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
Локальное подключение [проверки работоспособности ](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) может выявлять больше возможных типов ошибок проверки работоспособности.
- Учетная запись облачного ПК не найдена в подразделении (`adJoinCheckComputerObjectAlreadyExists`).
- Объект облачного ПК не найден в Azure AD (`azureAdDeviceSyncCheckDeviceNotFound`).
- Превышено время ожидания с момента проверки синхронизации объекта облачного ПК с Azure AD (`azureAdDeviceSyncCheckLongSyncCircle`). 

Подробные сведения и рекомендуемые действия по исправлению см. в [справочных материалах](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true#cloudpconpremisesconnectionhealthcheckerrortype-values).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Ежемесячные обновления Intune за сентябрь для бета-версии. Установите фильтр **Дата** в значение "июль 2021" и найдите раздел с таким заголовком.

### <a name="devices-and-apps--multi-tenant-management"></a>Устройства и приложения | Управление несколькими клиентами
Дебютный выпуск [Microsoft 365 Lighthouse API](managedtenants-concept-overview.md), который позволяет поставщикам управляемых служб удаленно управлять несколькими пользовательскими клиентами в масштабе для обеспечения соответствия требованиям и обнаружения угроз, а также обеспечивать работоспособное и безопасное состояние устройств клиента.

### <a name="education"></a>Образование
- Получите количество ошибок и сообщение о состоянии как часть [состояния синхронизации учебных данных](/graph/api/resources/educationsynchronizationprofilestatus?view=graph-rest-beta&preserve-view=true).
- Получите `extracting` или `validating` как возможные состояния такой синхронизации.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Получите коллекцию ошибок в жизненном цикле [экземпляра проверки доступа](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Поиск
- Используйте [API Поиска (Майкрософт) для получения сведений о людях](search-concept-person.md), наиболее релевантных для пользователя. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. 
- Получите доступ к [API индексации соединителей](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true) в подпространстве имен microsoft.graph.externalConnectors.

### <a name="teamwork"></a>Командная работа
- [Подпишитесь на уведомления об изменениях в ресурсе чата](teams-changenotifications-chat.md).
- [Подпишитесь на уведомления об изменениях пользователей в чате](teams-changenotifications-chatmembership.md), в [канале](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) или в [группе](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) (например, ресурсы [conversationMember](/graph/api/resources/conversationmember?view=graph-rest-beta&preserve-view=true)).
- Получайте сведения о событиях, происходящих в чате, канале или команде, путем доступа к ресурсу [eventMessageDetail](/graph/api/resources/EventMessageDetail?view=graph-rest-beta&preserve-view=true) из [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) или [чата](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true). Например, о таких событиях, как добавление участников в канал или чат, или изменение описания команды.


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
GA интерфейса API [просмотра доступа](/graph/api/resources/accessreviewsv2-overview). Ознакомьтесь с [обзором](accessreviews-overview.md) и инструкциями по [просмотру доступа в группы безопасности](tutorial-accessreviews-securitygroup.md) и [доступа в группы Microsoft 365](tutorial-accessreviews-m365group.md). Обратите внимание на то, что поддержка [предыдущего API просмотра доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) прекращается, и он перестанет возвращать данные в мае 2023 г.


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
Настройка уведомлений пользователей или участников группы о ходе выполнения [проверки доступа](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true) с помощью свойства **additionalNotificationRecipients** [определения расписания](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).

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
Ежемесячные обновления Intune для бета-версии. Присвойте фильтру **Дата** значение "Июнь 2021 г." и найдите раздел с таким заголовком.

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

## <a name="april-2021-new-and-generally-available"></a>Апрель 2021 г.: новые и общедоступные возможности

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход
- Управляйте [политикой проверки подлинности](/graph/api/resources/authenticationflowspolicy) на уровне клиента для включения или отключения [самостоятельной регистрации](/graph/api/resources/selfservicesignupauthenticationflowconfiguration) внешних пользователей.
- Администраторы могут связывать пользовательские потоки с приложениями, общий доступ к которым предоставлен внешним пользователям, и включить [самостоятельную регистрацию](/azure/active-directory/external-identities/self-service-sign-up-overview) в этих приложениях. Они могут настраивать пользовательские потоки самостоятельной регистрации и создавать персонализированные интерфейсы регистрации. После связи приложения с пользовательским потоком пользователи, переходящие в это приложение, смогут запускать поток регистрации, предоставляющий гостевую учетную запись.
- Настройка [атрибутов потоков пользователей](/graph/api/resources/identityuserflowattribute) в клиенте Azure AD позволяет собирать информацию о пользователе во время регистрации. Кроме того, можно собрать встроенный набор атрибутов или настроить специальные атрибуты потоков пользователей для сбора информации о пользователе, не встроенном в каталог. 
- В [пользовательском потоке Azure Active Directory](/graph/api/resources/b2xidentityuserflow) вы можете управлять стандартными языковыми параметрами и [настраивать языки и строки, отображаемые для пользователей в пользовательском потоке](/graph/api/resources/userflowlanguageconfiguration).
- Использование [соединителя API](/graph/api/resources/identityapiconnector) в пользовательских потоках для самостоятельной регистрации Azure AD и регистрации Azure AD B2C, чтобы вызывать API на определенном шаге для воздействия на выполнение пользовательского потока.

### <a name="teamwork"></a>Командная работа
- Определяйте канал по свойству **channelIdentity**, если [chatMessage](/graph/api/resources/chatmessage) находится в [канале](/graph/api/resources/channel).
- Определяйте чат по свойству **chatId**, если **[chatMessage](/graph/api/resources/chatmessage)** находится в [чате](/graph/api/resources/chat).
- Используйте связь **messages**, чтобы получить все ресурсы [chatMessage](/graph/api/resources/chatmessage) в [чате](/graph/api/resources/chat).
- Используйте разрешения приложения, чтобы [получить](/graph/api/chat-get) свойства указанного [чата](/graph/api/resources/chat).
- Используйте разрешения приложения, чтобы [получить указанного участника чата](/graph/api/chat-get-members) или [всех участников чата](/graph/api/chat-list-members), включенных в чат. Поскольку данные пользователей как участников чата являются конфиденциальными (кроме получения разрешений приложения), [запросите дополнительный доступ](teams-protected-apis.md) к этим операциям.

### <a name="use-the-toolkit"></a>Использование Toolkit
Впервые используете [Microsoft Graph Toolkit](/graph/toolkit/overview)? Попробуйте новую [схему обучения Toolkit](/learn/paths/m365-msgraph-toolkit/?WT.mc_id=m365-19989-cxa), используйте набор веб-компонентов и поставщиков проверки подлинности Toolkit для подключения веб-приложения к Microsoft Graph и загрузки данных из Microsoft 365.

## <a name="april-2021-new-in-preview-only"></a>Апрель 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Онлайн-собрания
- Получите [отчет](/graph/api/resources/meetingattendancereport?view=graph-rest-beta&preserve-view=true) о [присутствии каждого участника](/graph/api/resources/attendancerecord?view=graph-rest-beta&preserve-view=true) на запланированном онлайн-собрании с помощью свойства [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) **meetingAttendanceReport**.
- Включите или отключите чат либо ограничьте его длительность для онлайн-собрания с помощью свойства **allowMeetingChat**.
- Включите или отключите реакции для онлайн-собрания с помощью свойства **allowTeamworkReactions**.

### <a name="compliance"></a>Соответствие требованиям
[Получите](/graph/api/ediscovery-settings-get?view=graph-rest-beta&preserve-view=true), [обновите](/graph/api/ediscovery-settings-update?view=graph-rest-beta&preserve-view=true) или [сбросьте до значений по умолчанию](/graph/api/ediscovery-settings-resettodefault?view=graph-rest-beta&preserve-view=true) следующие [параметры](/graph/api/resources/ediscovery-settings?view=graph-rest-beta&preserve-view=true) для [дела](/graph/api/resources/ediscovery-case?view=graph-rest-beta&preserve-view=true) обнаружения электронных данных:
- [Обнаружение дубликатов, неполных дубликатов](/microsoft-365/compliance/near-duplicate-detection-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true) и [цепочек сообщений](/microsoft-365/compliance/email-threading-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true) с помощью свойства **redundancyDetection**.
- [Определение тем](/microsoft-365/compliance/themes-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true), являющихся преобладающими в документах набора для проверки, с помощью свойства **topicModeling**.
- [Извлечение текста из файлов изображений путем распознавания текста (OCR)](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery?view=o365-worldwide&preserve-view=true#optical-character-recognition-ocr) с помощью свойства **ocr**.

Эти параметры обеспечивают функциональность аналитики, [позволяющую выполнить интеллектуальный отбор данных](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true#cull-data-intelligently) в комплексном рабочем процессе [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true).

### <a name="devices-and-apps--device-updates"></a>Устройства и приложения | Обновления устройств
Появление API для службы развертывания Центра обновления Windows для бизнеса. Служба поддерживает развертывание обновлений компонентов Windows 10 и ускорение обновления системы безопасности Windows 10 на устройствах. Чтобы получить дополнительные сведения, начните с [обзора API обновлений Windows](windowsupdates-concept-overview.md).

### <a name="education"></a>Образование
- Свяжите папку с [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) для хранения всех связанных файловых ресурсов с помощью свойства **resourcesFolderUrl**.
- Используйте прямую ссылку на [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) с помощью свойства **webUrl**.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Администраторы могут [получить](/graph/api/accessreviewpolicy-get?view=graph-rest-beta&preserve-view=true) или [обновить](/graph/api/accessreviewpolicy-update?view=graph-rest-beta&preserve-view=true) политики на уровне каталога для проверки доступа с помощью ресурса [accessReviewPolicy](/graph/api/resources/accessreviewpolicy?view=graph-rest-beta&preserve-view=true). Например, администраторы могут использовать политику проверки доступа, чтобы включить или отключить владельцев группы, проверяющих доступ в группах, которыми они владеют.

### <a name="search"></a>Поиск
[Включите варианты написания слов или исправления](search-concept-speller.md) для пользовательского запроса. Это полезно, когда пользовательский запрос содержит опечатки или когда из-за ошибок не удается получить результаты поиска.

### <a name="teamwork"></a>Командная работа
- Используйте [предоставление разрешения для определенных ресурсов](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true), чтобы перечислять приложения с доступом к указанной [группе ](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) или [чату](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).
- [Получите](/graph/api/teamsappicon-get?view=graph-rest-beta&preserve-view=true) свойства [значка](/graph/api/resources/teamsAppIcon?view=graph-rest-beta&preserve-view=true), связанного с приложением Teams. Чтобы получить фактическое изображение значка, используйте [получение размещенного содержимого](/graph/api/teamworkhostedcontent-get?view=graph-rest-beta&preserve-view=true).

### <a name="use-sdks"></a>Использование пакетов SDK
- Попробуйте [предварительный выпуск клиентской библиотеки JavaScript для Microsoft Graph версии 3.0.0](https://www.npmjs.com/package/@microsoft/microsoft-graph-client/v/3.0.0-Preview.1). Этот выпуск включает несколько потоков проверки подлинности, проверку подлинности на стороне сервера, отправку больших файлов Node.js Stream, отслеживание хода выполнения и многое другое. Дополнительные сведения см. в [руководстве по обновлению](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/changelogs/v3-upgrade-guide.md).
- Попробуйте новую схему обучения, чтобы [ознакомиться со сценариями Microsoft Graph для разработки JavaScript](/learn/paths/m365-msgraph-scenarios/?WT.mc_id=m365-16105-cxa).


## <a name="march-2021-new-and-generally-available"></a>Март 2021 г.: новые и общедоступные возможности

### <a name="applications"></a>Приложения
- Общая доступность ресурса [applicationTemplate](/graph/api/resources/applicationtemplate), поддерживающего [перечисление](/graph/api/applicationtemplate-list) приложений в коллекции приложений Azure AD и [добавление](/graph/api/applicationtemplate-instantiate) экземпляра такого приложения в каталог.
- Используйте разрешение только для приложения `Application.ReadWrite.OwnedBy` при [добавления](/graph/api/applicationtemplate-instantiate) такого экземпляра.
- Используйте свойство **signInAudience** объекта [servicePrincipal](/graph/api/resources/serviceprincipal), чтобы получить учетные записи пользователей, поддерживаемые текущим приложением.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Общая доступность [API облачной печати](universal-print-concept-overview.md) для универсальной печати! Ознакомьтесь с [объявлением](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778) и узнайте, как [начать работу с универсальной печатью](/universal-print/fundamentals/universal-print-license).
- [Подписывайтесь на уведомления об изменениях](universal-print-webhook-notifications.md) в [определении задачи печати](/graph/api/resources/printtaskdefinition) или ресурсе [printer](/graph/api/resources/printer).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Используйте [запросы согласия](/graph/api/resources/consentrequests-root) Azure Active Directory (Azure AD) для управления процессом запроса для пользователей, пытающихся получить доступ к приложениям, которым требуется утверждение администратора. API использует следующие ресурсы.
  - Ресурс [adminConsentRequestPolicy](/graph/api/resources/adminconsentrequestpolicy) для создания и управления запросами на доступ к приложениям для организации.
  - Ресурс [appConsentRequest](/graph/api/resources/appconsentrequest) для объединения запросов пользователей (и управления ими) на доступ к определенному приложению.
  - Ресурс [userConsentRequest](/graph/api/resources/userConsentRequest) для пользователей, запрашивающих доступ к приложению, для которого требуется авторизация администратора. 
  - Ресурс [accessReviewReviewerScope](/graph/api/resources/accessReviewReviewerScope) определяет, кто указан в **adminConsentRequestPolicy** для просмотра объектов **appConsentRequest** и **userConsentRequest**.
  - Ресурс [approval](/graph/api/resources/approval) представляет решение об утверждении запроса.
- Общая доступность API-интерфейса условий использования, поддерживающего настраиваемое [соглашение об условиях использования](/graph/api/resources/agreement) в Azure AD.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Общая доступность [методов проверки подлинности](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true), включая [ключи безопасности FIDO2](/graph/api/resources/fido2authenticationmethod), [приложение Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod) и [Windows Hello для бизнеса](/graph/api/resources/windowshelloforbusinessauthenticationmethod).
- Общая доступность [политик методов проверки подлинности](/graph/api/resources/authenticationmethodspolicies-overview), определяющих методы проверки подлинности и пользователей, которые могут использовать их для входа и многофакторной проверки подлинности (MFA) в Azure AD. Политики методов проверки подлинности, которыми можно управлять в Microsoft Graph, включают [ключи безопасности FIDO2](/graph/api/resources/fido2authenticationmethodconfiguration), беспарольный вход с помощью телефона с использованием [приложения Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration) и [политику методов проверки подлинности OTP](/graph/api/resources/emailauthenticationmethodconfiguration) клиента.
- Общая доступность [политики развертывания функций](/graph/api/resources/featureRolloutPolicy), которая позволяет администраторам клиента выполнить пилотное развертывание функций для определенных групп перед включением их для всей организации.
- Общая доступность [свойств фирменной символики организации](/graph/api/resources/organizationalbrandingproperties), которая позволяет настраивать внешний вид и удобство использования экранов входа в Azure Active Directory. Организации могут выполнять настройку на основе региональных параметров для отдельных пользователей.

### <a name="tasks-and-plans"></a>Задачи и планы
- Используйте делегированное разрешение `Tasks.Read` для операций чтения всех ресурсов Планировщика.
- Используйте делегированное разрешение `Tasks.ReadWrite` для операций чтения и записи всех ресурсов Планировщика.

### <a name="teamwork"></a>Командная работа
- Общая доступность операций [чата](/graph/api/resources/chat), объектов [conversationMember](/graph/api/resources/conversationmember) чата, [app](/graph/api/resources/teamsappinstallation) чата, [tab](/graph/api/resources/teamstab) чата и соответствующих методов.
- Общая доступность дополнительных свойств объекта [teamsAppDefinition](/graph/api/resources/teamsAppDefinition), представляющих сведения о версии приложения в каталоге приложения Microsoft Teams, включая следующие:
  - **createdBy**, **description**, **shortDescription**, **lastModifiedDateTime**
  - свойство **publishingState**, которое может находиться в состоянии `submitted` и проверяться, `published` или `rejected` администратором
  - связь **bot** типа [teamworkBot](/graph/api/resources/teamworkbot), представляющая сведения о боте, указанные в манифесте приложения Teams.
- Используйте API уведомлений ленты новостей, чтобы лучше взаимодействовать с пользователями в трех контекстах:
  - [Отправка уведомления пользователю в чате](/graph/api/chat-sendactivitynotification)
  - [Отправка уведомления пользователю в команде](/graph/api/team-sendactivitynotification)
  - [Отправка уведомления пользователю](/graph/api/userteamwork-sendactivitynotification)
- Перенесите журнал сообщений и данные пользователей из внешней системы в канал Teams, чтобы они могли беспрепятственно продолжать общение. Используйте следующие методы, поддерживающие сценарий миграции:
  - [Создание команды](/graph/api/team-post)
  - [Создание канала](/graph/api/channel-post)
  - [Создание объекта chatMessage в канале](/graph/api/channel-post-messages)
  - [Ответ на сообщение в канале](/graph/api/channel-post-messagereply)
  - [Завершение переноса сообщения в команду](/graph/api/team-completemigration)
  - [Завершение переноса сообщения в канал](/graph/api/channel-completemigration)
- [Перечисление](/graph/api/chatmessage-list-chatmessagehostedcontents) или [получение](/graph/api/chatmessagehostedcontent-get) форматированного контента, размещенного в [chatMessage](/graph/api/resources/chatmessage), например изображений или фрагментов кода.
- Поддержка делегированных разрешений `ChannelMessage.Read.All` для подписки на уведомления об изменениях в ресурсах [chatMessage](/graph/api/resources/chatmessage).

## <a name="march-2021-new-in-preview-only"></a>Март 2021 г.: новые возможности только в предварительной версии

### <a name="applications"></a>Приложения
[Создавайте и добавляйте самозаверяющие сертификаты](/graph/api/servicePrincipal-addTokenSigningCertificate?view=graph-rest-beta&preserve-view=true) в приложения SAML. Используйте это для включения единого входа для приложений коллекции Azure AD в клиенте, разрешив Azure AD подписывать отклики SAML.

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
В ресурс [cloudPcDeviceImage](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) добавлено еще две причины сбоя при отправке исходного образа устройства: операционная система не поддерживается (`osVersionNotSupported`) или недопустимый исходный образ для подготовки ВМ Windows (`sourceImageInvalid`).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
Получение даты и времени (свойство **lastSeenDateTime**), когда принтер в последний раз взаимодействовал с универсальной печатью.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [март](https://developer.microsoft.com/graph/changelog/?from=2021-03-01&to=2021-03-31&filterBy=Corporate%20management) для бета-версии.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Применение новой модели [проверок доступа](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true) для участия в группах и всех других поддерживаемых типов ресурсов. Отказ от [устаревшей модели проверки доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Сайты и списки
- Поддержка определенного типа контента или шаблона для документов или наборов документов в конкретных семействах веб-сайтов с помощью набора новых свойств и методов объекта [contentType](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true). К методам относятся следующие:
  - [addCopy](/graph/api/contenttype-addcopy?view=graph-rest-beta&preserve-view=true)
  - [associateWithHubSites](/graph/api/contenttype-associatewithhubsites?view=graph-rest-beta&preserve-view=true)
  - [copyToDefaultContentLocation](/graph/api/contenttype-copytodefaultcontentlocation?view=graph-rest-beta&preserve-view=true)
  - [isPublished](/graph/api/contenttype-ispublished?view=graph-rest-beta&preserve-view=true)
  - [publish](/graph/api/contenttype-publish?view=graph-rest-beta&preserve-view=true)
  - [unpublish](/graph/api/contenttype-unpublish?view=graph-rest-beta&preserve-view=true)
- Настройка типов контента по их столбцам. Столбцы представлены объектом [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta&preserve-view=true) и поддерживают полный набор операций CRUD.
- [Получение типов контента сайта, которые можно применить к списку](/graph/api/site-getApplicableContentTypesForList?view=graph-rest-beta&preserve-view=true).
- Различение типов столбцов по следующим свойствам в объекте **columnDefinition**: boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text. Эти свойства являются взаимоисключающими.

### <a name="sites-and-lists--taxonomy"></a>Сайты и списки | Таксономия
- Переходите с [сайта](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) к [банку терминов таксономии](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true), используя связь **termStore**.
- В обратном направлении получайте ИД родительского сайта банка терминов с помощью свойства **parentSiteId**.

### <a name="users"></a>Пользователи
- [Получение](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) или [обновление](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) пользовательских [настроек для перевода языков](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true). Например, следует ли переводить, переводить автоматически или отображать запрос перед переводом определенных языков в сообщениях, чатах и на веб-страницах, а также любые [переопределения перевода](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true).
- [Активация плана обслуживания](/graph/api/user-activateServicePlan?view=graph-rest-beta&preserve-view=true) для пользователя.


## <a name="february-2021-new-and-generally-available"></a>Февраль 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Собрание по сети
Использование разрешений приложений `OnlineMeetings.Read.All` или `OnlineMeetings.ReadWrite.All`, основанных на политике, для операций и методов ресурса [onlineMeeting](/graph/api/resources/onlinemeeting). Администраторы могут [настроить политику доступа приложения](cloud-communication-online-meeting-application-access-policy.md), чтобы разрешить приложениям доступ к собраниям по сети от имени пользователя.

### <a name="sites-and-lists"></a>Сайты и списки
Использование ресурса [permission](/graph/api/resources/permission) и его операций CRUD для управления разрешением общего доступа, предоставленным для [driveItem](/graph/api/resources/driveitem). Разрешения с аспектом link представляют ссылки для совместного доступа, созданные в элементе. Разрешения с аспектом invitation представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.

## <a name="february-2021-new-in-preview-only"></a>Февраль 2021 г.: новые возможности только в предварительной версии

### <a name="applications"></a>Приложения
Использование разрешений приложений для [API синхронизации](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true), которые автоматизируют подготовку (создание, обслуживание) и отмену подготовки (удаление) удостоверений в Azure AD.

### <a name="cloud-communications--calls"></a>Облачные коммуникации | Звонки
Поддержка [записей на основе политики для звонков](/microsoftteams/teams-recording-policy), когда при использовании административной политики звонки автоматически записываются для последующей обработки и хранения по требованиям соответствующей корпоративной или нормативной политики. Прежде чем участник на основе политики присоединится к звонку, политика предписывает отправить ресурс [participantJoiningNotification](/graph/api/resources/participantJoiningNotification?view=graph-rest-beta&preserve-view=true) боту, связанному с политикой, у которого есть возможность для обработки нового участника. Бот отвечает одним из ресурсов [acceptJoinResponse](/graph/api/resources/acceptjoinresponse?view=graph-rest-beta&preserve-view=true), [rejectJoinResponse](/graph/api/resources/rejectjoinresponse?view=graph-rest-beta&preserve-view=true), или [inviteNewBotResponse](/graph/api/resources/invitenewbotresponse?view=graph-rest-beta&preserve-view=true) в полезной нагрузке отклика.

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
- Использование ресурса [legalHold](/graph/api/resources/ediscovery-legalhold?view=graph-rest-beta&preserve-view=true) и его API для бессрочной защиты контента от удаления для целей судебного разбирательства, внутреннего расследования или других юридических действий.
- Использование ресурса [sourceCollection](/graph/api/resources/ediscovery-sourcecollection?view=graph-rest-beta&preserve-view=true) и его API для поиска и идентификации важных документов из охраняемых и неохраняемых расположений в Microsoft 365.
- Использование ресурса [tag](/graph/api/resources/ediscovery-tag?view=graph-rest-beta&preserve-view=true) и API для пометки документов во время проверки, чтобы разделять адаптивное и неадаптивное содержимое.
- [Экспорт](/graph/api/ediscovery-reviewset-export?view=graph-rest-beta&preserve-view=true) документов из [набора для проверки](/graph/api/resources/ediscovery-reviewset?view=graph-rest-beta&preserve-view=true).
- Использование действия [addToReviewSet](/graph/api/ediscovery-reviewset-addtoreviewset?view=graph-rest-beta&preserve-view=true), чтобы добавлять документы в **sourceCollection** для **reviewSet**.
- [Применение тегов](/graph/api/ediscovery-reviewsetquery-applytags?view=graph-rest-beta&preserve-view=true) к документам на основе [запроса набора для проверки](/graph/api/resources/ediscovery-reviewsetquery?view=graph-rest-beta&preserve-view=true).
- Определены все API обнаружения электронных данных в пространстве имен `microsoft.graph.ediscovery`.
- Модель делегированных разрешений изменена с `User.Read` на `eDiscovery.Read.All` и `eDiscovery.ReadWrite.All`.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
- Обновления Intune за [февраль](https://developer.microsoft.com/graph/changelog/?from=2021-02-01&to=2021-02-28&filterBy=Corporate%20management) для бета-версии.
- Новые свойства, установленные Intune для ресурса [device](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true): **deviceCategory**, **deviceOwnership**, **domainName**, **регистрацииProfileName**, **enrollmentType**, **isRooted**, **managementType** и **registrationDateTime**.

### <a name="education"></a>Образование
Используйте [educationAssignmentDefaults](/graph/api/resources/educationAssignmentDefaults?view=graph-rest-beta&preserve-view=true), чтобы указать стандартные рекомендации в задании для класса, например время сдачи задания, URL-адрес канала для уведомлений о задании. Вы по-прежнему можете настраивать значения при создании задания.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Использование ресурса [smsAuthenticationMethodConfiguration](/graph/api/resources/smsAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true) для [получения](/graph/api/smsauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true), [обновления](/graph/api/smsauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true) или [удаления](/graph/api/smsauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) параметров конфигурации политики проверки подлинности текстовых сообщений в организации.
- Использование ресурса [temporaryAccessPassAuthenticationMethodConfiguration](/graph/api/resources/temporaryaccesspassauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true) для [получения](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-get?view=graph-rest-beta&preserve-view=true), [обновления](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-update?view=graph-rest-beta&preserve-view=true) или [удаления](/graph/api/temporaryaccesspassauthenticationmethodconfiguration-delete?view=graph-rest-beta&preserve-view=true) параметров конфигурации политики проверки подлинности с предоставлением временного доступа в организации.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Назначение данных географического расположения [пакету доступа](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true) ресурсу в [запросе на назначение пакета доступа](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).
- Получение списка всех [сред ресурсов пакета доступа](/graph/api/resources/accesspackageresourceenvironment?view=graph-rest-beta&preserve-view=true), представляющих географические расположения, в которых хранятся ресурсы SharePoint Online.
- Использование разрешений приложений (`EntitlementManagement.Read.All` или `EntitlementManagement.ReadWrite.All`) для операций следующих ресурсов:
  - [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignment](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)
  - [accessPackageAssignmentResourceRole](/graph/api/resources/accesspackageassignmentresourcerole?view=graph-rest-beta&preserve-view=true)
  - [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)
  - [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true)
  - [connectedOrganization](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true)
  - [entitlementManagementSettings](/graph/api/resources/entitlementmanagementsettings?view=graph-rest-beta&preserve-view=true)

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Получение дополнительных свойств из [детальных отчетов об использовании сайтов SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta&preserve-view=true): anonymousLinkCount, companyLinkCount, externalSharing, geolocation, secureLinkForGuestCount, secureLinkForMemberCount, siteSensitivityLabelId и unmanagedDevicePolicy.

### <a name="tasks-and-plans"></a>Задачи и планы
- Определяйте до 25 категорий в объекте [plan details](/graph/api/resources/plannerplandetails?view=graph-rest-beta&preserve-view=true) для плана. Для каждой категории укажите описательную метку и свяжите задачи в плане с одной или несколькими из этих категорий. 
- Используйте ресурс [roster](/graph/api/resources/plannerRoster?view=graph-rest-beta&preserve-view=true), чтобы представить коллекцию пользователей, совместно работающих над [планом](/graph/api/resources/plannerplan?view=graph-rest-beta&preserve-view=true). Используйте связь **rosterPlans**, чтобы получать списки, в которых пользователь является [участником](/graph/api/resources/plannerrostermember?view=graph-rest-beta&preserve-view=true). 
- Для планов, отображаемых в решениях вне Планировщика, например в Microsoft Teams, укажите в [сведениях о контексте плане](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta&preserve-view=true) способ отображения ссылки на [контекст плана](/graph/api/resources/plannerPlanContext?view=graph-rest-beta&preserve-view=true). 

### <a name="use-sdks"></a>Использование пакетов SDK
Попробуйте предварительный выпуск [пакета SDK Microsoft Graph Java версии 3](https://github.com/microsoftgraph/msgraph-sdk-java/tree/feature/v3)! Дополнительные сведения см. в соответствующей [записи блога](https://developer.microsoft.com/graph/blogs/announcing-the-public-preview-of-microsoft-graph-java-sdk-v3/).

## <a name="january-2021-new-in-preview-only"></a>Январь 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications"></a>Облачные коммуникации
- Организация трансляций как ресурсов [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). См. [пример](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true#example-3-create-a-live-event-with-a-user-token). 
- Получение потока содержимого в виде [отчета об участниках](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-4-retrieve-the-attendee-report-of-a-live-event), [записи](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-5-retrieve-the-recording-of-a-live-event) или альтернативной записи трансляции.
- Получение статуса [присутствия](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) пользователя, которого [нет на месте](/graph/api/resources/outofofficesettings?view=graph-rest-beta&preserve-view=true), а также любого сообщения, заданного в качестве этого статуса.

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- [Обновление пароля домена Active Directory](/graph/api/cloudpconpremisesconnection-updateaddomainpassword?view=graph-rest-beta&preserve-view=true) для успешного [локального сетевого подключения](/graph/api/resources/cloudPcOnPremisesConnection?view=graph-rest-beta&preserve-view=true).
- [Запуск проверок работоспособности локального сетевого подключения](/graph/api/cloudpconpremisesconnection-runhealthcheck?view=graph-rest-beta&preserve-view=true) теперь может выявлять 5 дополнительных типов ошибок в ресурсе [проверки работоспособности локального подключения](/graph/api/resources/cloudpconpremisesconnectionhealthcheck?view=graph-rest-beta&preserve-view=true). Дополнительные сведения о типах ошибок см. в [журнале изменений](https://developer.microsoft.com/graph/changelog) за январь 2021 г.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- [Подписка на уведомления об изменениях облачной печати](universal-print-webhook-notifications.md) — при запуске задания печати и когда принтер готов скачать задание печати.
- Получение более полного диапазона [возможных значений](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true#printerprocessingstatedetail-values) для состояния [принтера](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true).
- Использование делегированных разрешений в приложениях от имени вошедшего пользователя:
  - `PrinterShare.ReadBasic.All` для чтения основных сведений об общих принтерах, кроме сведений об управлении доступом.
  - `PrintConnector.Read.All` для чтения соединителей печати.
  - `PrintConnector.ReadWrite.All` для чтения и записи соединителей печати.
  - `PrintJob.Create` для создания заданий печати и отправки содержимого в задания печати.
  - `PrintSettings.Read.All` для чтения параметров печати на уровне клиента.
  - `PrintSettings.ReadWrite.All` для чтения или записи параметров печати на уровне клиента.
  - `Reports.Read.All` для чтения сводки об использовании печати для определенного пользователя или принтера.

### <a name="education"></a>Образование
Использование [параметров заданий](/graph/api/resources/educationAssignmentSettings?view=graph-rest-beta&preserve-view=true) на уровне класса, чтобы включить или отключить анимацию для празднования сдачи задания.

### <a name="groups"></a>Группы
Получение состояния обработки динамической группы на основе правил с помощью свойства **membershipRuleProcessingStatus**. Это удобно, когда изменяется атрибут пользователя, участие пользователя в [группе Microsoft 365](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) на основе правил подвергается повторной оценке в соответствии с правилами участия в группе, настроенными в организации. 

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Получение [права использования](/graph/api/resources/UsageRight?view=graph-rest-beta&preserve-view=true) стороннего программного обеспечения, созданного на основе PowerApps, которым обладает пользователь или устройство, или права использования подписки, которым обладает устройство. Право использования содержит идентификаторы соответствующей службы или продукта и текущее состояние права использования, например "активно", "неактивно", "с предупреждением" или "приостановлено".

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Приложения могут использовать разрешения приложений, чтобы позволить администраторам управлять [способами проверки подлинности](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) для пользователей.
- Поддержка [Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethod?view=graph-rest-beta&preserve-view=true) в качестве способа проверки подлинности пользователя для входа или многофакторной проверки подлинности в Azure AD.
- Использование [политики Microsoft Authenticator](/graph/api/resources/microsoftauthenticatorauthenticationmethodconfiguration?view=graph-rest-beta&preserve-view=true), чтобы определить параметры конфигурации, а также пользователей или группы, которым разрешено применять Microsoft Authenticator в качестве способа проверки подлинности. Использование политики Microsoft Authenticator вместо [политики входа по телефону без пароля с помощью Microsoft Authenticator](/graph/api/resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true), поддержка которой прекращена. 
- Поддержка [Windows Hello для бизнеса](/graph/api/resources/windowshelloforbusinessauthenticationmethod?view=graph-rest-beta&preserve-view=true) в качестве способа проверки подлинности пользователя при входе на устройствах с Windows без применения пароля.

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
- [Получение отчета о количестве зарегистрированных пользователей или пользователей, которым доступны различные функции регистрации](/graph/api/authenticationmethodsroot-usersregisteredbyfeature?view=graph-rest-beta&preserve-view=true), включая многофакторную проверку подлинности, самостоятельный сброс пароля или проверку подлинности без пароля.
- [Получение отчета о количестве пользователей, зарегистрированных для каждого способа проверки подлинности](/graph/api/authenticationmethodsroot-usersregisteredbymethod?view=graph-rest-beta&preserve-view=true), включая пароль, Windows Hello для бизнеса или вход без пароля с помощью телефона.

## <a name="december-2020-new-and-generally-available"></a>Декабрь 2020 г.: новые и общедоступные возможности

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
Общая доступность набора средств Microsoft Graph Toolkit 2.0. Этот выпуск включает новый [компонент для задач Microsoft Graph To-Do](./toolkit/components/todo.md), отличающийся от [компонента задач Планировщика](./toolkit/components/tasks.md), и улучшенный [компонент карточки контакта](./toolkit/components/person-card.md). Дополнительную сведения см. [в соответствующей записи блога](https://developer.microsoft.com/graph/blogs/announcing-the-general-availability-of-microsoft-graph-toolkit-2-0/).


## <a name="december-2020-new-in-preview-only"></a>Декабрь 2020 г.: новые возможности только в предварительной версии

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
В рамках [управления правами](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true) Azure Active Directory, когда пользователи хотят получить доступ к группам или приложениям либо сайты SharePoint Online запрашивают назначение для [пакета доступа](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true), они теперь могут отвечать на [вопросы](/graph/api/resources/accesspackagequestion?view=graph-rest-beta&preserve-view=true), представленные [локализованном содержимом](/graph/api/resources/accesspackagelocalizedcontent?view=graph-rest-beta&preserve-view=true) [запросa на назначение пакета доступа](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true).

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


## <a name="november-2020-new-and-generally-available"></a>Ноябрь 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачная коммуникация
- Общая доступность свойства **роль** типа [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo), разделяющего участников [виртуального собрания](/graph/api/resources/onlinemeeting) на участников и докладчиков.
- Общая доступность свойства **lobbyBypassSettings** и его [значений](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) для допуска пользователей к виртуальному собранию.
- Общая доступность свойства **isEntryExitAnnounced** для настройки параметров объявления пользователей, присоединяющихся к виртуальному собранию или покидающих его.
- Общая доступность свойства **allowedPresenters** для разрешения отдельным пользователям выступать на собрании.

### <a name="search"></a>Поиск
- Общая доступность [API запросов](/graph/api/resources/search-api-overview) Поиска (Майкрософт), поддерживающих поиск данных следующих типов:
  - [Сообщения Outlook](./search-concept-messages.md)
  - [События календаря Outlook](./search-concept-events.md)
  - [Ресурсы OneDrive и SharePoint](./search-concept-files.md).

### <a name="teamwork"></a>Командная работа

- Общая доступность разрешений с согласием для конкретных ресурсов (RSC). Разрешения RSC позволяют владельцам команд предоставлять детальные разрешения рабочим приложениям на доступ и/или изменение конкретных данных команды, например на чтение параметров команды или изменение названий каналов, описаний и других параметров.
- Общая доступность API, применяемых к [каналу](/graph/api/resources/channel) или сообщениям в канале. API включают:
  - [Создание](/graph/api/conversationmember-add) или [удаление](/graph/api/conversationmember-delete) участника беседы из канала.
  - [Обновление роли участника](/graph/api/conversationmember-update) в канале.
  - Получение конкретного сообщения или всех сообщений в канале.
  - Получение конкретного ответа или всех ответов в канале.
  - [Отслеживание новых или обновленных сообщений в канале](/graph/api/chatmessage-delta).


## <a name="november-2020-new-in-preview-only"></a>Ноябрь 2020 г.: новые возможности только в предварительной версии

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
Дебютное представление интерфейса [API проверки доступа в целях предоставления членства в группе](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true) для регулярной проверки доступа пользователей. Интерфейс позволяет обеспечивать постоянный доступ только нужным пользователям и эффективно управлять членством в группе.

### <a name="search"></a>Поиск
Вы можете объединять числовые или строковые результаты поиска, импортированные [соединителями Microsoft Graph](/microsoftsearch/connectors-overview), которые настроены в качестве уточняемых в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Ознакомьтесь с дополнительными сведениями об [уточнении результатов поиска с помощью агрегирования](search-concept-aggregation.md).

## <a name="october-2020-new-and-generally-available"></a>Октябрь 2020 г.: новые и общедоступные возможности

### <a name="application"></a>Приложение
- Разрешите [адрес электронной почты в качестве альтернативного имени для входа в Azure AD](/azure/active-directory/authentication/howto-authentication-use-email-signin) с помощью политики [обнаружения домашней области](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery). Политика обнаружения домашней области определяет, требовать ли от пользователя проверки подлинности после предоставления пользователем имени для входа. В этом случае настройка свойства **AlternateIdLogin** ресурса [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) может разрешить пользователю входить с помощью адреса электронной почты.
- Получайте сведения о проверенном издателе для объектов [application](/graph/api/resources/application) или [servicePrincipal](/graph/api/resources/serviceprincipal) и [настройте](/graph/api/application-setverifiedpublisher) или [удалите](/graph/api/application-unsetverifiedpublisher) сведения о проверенном издателе для объекта **application**.

### <a name="change-notifications"></a>Уведомления об изменениях
Приложения рабочей среды теперь могут подписываться на уведомления жизненного цикла элементов Outlook [message](/graph/api/resources/message), [event](/graph/api/resources/event) и [contact](/graph/api/resources/contact), а также элемента Teams [chatMessage](/graph/api/resources/chatmessage), чтобы [сократить количество пропущенных уведомлений о подписках и изменениях](webhooks-lifecycle.md).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Общая доступность расширенных параметров системных запросов OData (`$count`, `$search` и `$filter`) для объектов каталогов.
- Ознакомьтесь с примерами, демонстрирующими преобразование OData для объектов каталога.
- Списки расширенных API см. в разделе удостоверения и доступа в обновлениях за [октябрь](changelog.md#october-2020) журнала изменений.

### <a name="teamwork"></a>Командная работа
- Общая доступность полного набора операций CRUD для ресурса [conversationMember](/graph/api/resources/conversationmember) и [aadUserConversationMember](/graph/api/resources/aaduserconversationmember). Эти ресурсы представляют участника чата или беседы канала, который может быть или не быть пользователем в Azure AD.
- Общая доступность уведомлений жизненного цикла для ресурсов [chatMessage](/graph/api/resources/chatmessage) в Teams для [сокращения количества пропущенных уведомлений о подписках и изменениях](webhooks-lifecycle.md).

### <a name="to-do-tasks"></a>Задачи To-Do
Общая доступность [API Microsoft To Do](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true) — используйте API To-Do в приложении рабочей среды для создания задач и управления ими в рамках рабочего процесса пользователя, например при создании задачи из письма.  

### <a name="users"></a>Пользователи
Получайте новые свойства, относящиеся к [пользователю](/graph/api/resources/user), который является корпоративным сотрудником: дата найма, связь с организацией, например отдел и место возникновения затрат, и тип сотрудника, например консультант, подрядчик или поставщик. Эти свойства требуют указания параметра запроса OData `$select` в операции GET.

## <a name="october-2020-new-in-preview-only"></a>Октябрь 2020 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Собрание по сети
- Определите роль участника в [собрании по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) в качестве участника или выступающего, используя свойство **role** типа [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo?view=graph-rest-beta&preserve-view=true).
- Получайте объект [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) путем [фильтрации по свойству joinWebUrl собрания](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-3-retrieve-an-online-meeting-by-joinweburl).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать

- Прекращение поддержки действия **uploadData**, вместо которого применяется [создание сеанса отправки](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) для [отправки документа](upload-data-to-upload-session.md) на принтер или общий принтер.
- Прекращение поддержки свойства **printDocument** в [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true), вместо которого применяется аналогичное свойство **configuration** в [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Получайте URL-адрес исходного или конечного задания для перенаправляемого объекта **printJob**, используя свойство **redirectedFrom** или **redirectedTo**.
- Получайте текущее состояние **printJob**, используя свойство **state** и новое свойство **details**.
- Получайте коллекцию общих принтеров, связанных с объектом [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), используя связь **shares**. 
- Прекращение поддержки свойства **processingStateReasons** объекта **printer**, вместо которого применяется свойство **status**. Свойство **status** относится к типу [printer status](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) и представляет свойство **details**. Используйте свойство **details** для определения причины текущего состояния принтера.
- Прекращение поддержки свойства **feedDirections** в [printerCapabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true), вместо которого применяется свойство **feedOrientations** для получения ориентации подачи лотка, поддерживаемой принтером.
- Сведения о нескольких переименованиях API и свойств, а также о прекращении поддержки нескольких элементов см. в разделе облачной печати в обновлениях за [октябрь](changelog.md#october-2020) журнала изменений.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [октябрь](changelog.md#october-2020) для бета-версии.

### <a name="files"></a>Файлы
[Отменяйте](/graph/api/permission-revokegrants?view=graph-rest-beta&preserve-view=true) доступ к элементу [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) или [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true), предоставленный с помощью ссылки для общего доступа.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Управляйте [политиками метода проверки подлинности](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true), чтобы определять пользователей, которые могут использовать конкретные методы многофакторной проверки подлинности для входа в Azure Active Directory. Настройте политики, чтобы определить следующее:
  - Типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.
  - Пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход без пароля с помощью телефона для входа в Azure AD.
- Настройте [метод проверки подлинности электронной почты](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true), чтобы пользователи самостоятельно сбрасывали пароли.
- Используйте [Azure AD B2C](/azure/active-directory-b2c/overview) и [выберите механизм настройки и проверки подлинности пользователей с помощью локальных учетных записей](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true).
- Используйте `Policy.ReadWrite.AuthenticationMethod` для чтения и записи политик метода проверки подлинности в организации в виде делегированного разрешения от имени вошедшего пользователя или разрешения приложения без необходимости входа пользователя.
- Укажите в [политике авторизации](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true), можно ли приглашать внешних пользователей в организацию и кому это разрешено.

### <a name="people-and-workplace-intelligence--insights"></a>Люди и рабочая аналитика | Аналитика 
Администраторы могут просмотреть [примеры использования командлетов PowerShell](insights-customize-item-insights-privacy.md#how-to-configure-item-insights-settings-via-powershell), чтобы настроить параметры аналитики элементов для организации.

### <a name="teamwork"></a>Командная работа
- Используйте атрибут **channelCreationMode** экземпляра, чтобы указать, что создается [канал](/graph/api/resources/channel?preserve-view=true&view=graph-rest-beta#instance-attributes) для обслуживания миграции данных. Используйте атрибут [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true), чтобы указать на завершение миграции и возможность публикации и чтения сообщений участниками.
- Используйте атрибут **teamCreationMode** экземпляра, чтобы указать, что создается [команда](/graph/api/resources/team?preserve-view=true&view=graph-rest-beta#instance-attributes) для обслуживания миграции. Используйте атрибут [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true), чтобы указать на завершение миграции и возможность выполнения операций участников и публикации сообщений участниками.

## <a name="september-2020-new-and-generally-available"></a>Сентябрь 2020г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
Общая доступность необязательного свойства **transactionId** ресурса [event](/graph/api/resources/event), которое настраивается клиентским приложением, чтобы избежать лишних операций POST, если клиент повторно пытается создать то же событие. Это полезно в тех случаях, когда из-за плохого сетевого подключения клиент отключается, не успев получить от сервера ответ на предыдущий запрос клиента на создание события.

### <a name="cloud-communications"></a>Облачные коммуникации
[Удаление участника](/graph/api/participant-delete) из [звонка](/graph/api/resources/call). Вы можете использовать эту операцию даже в тех случаях, когда нужно удалить участника из активного звонка.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [сентябрь](changelog.md#september-2020) для версии 1.0.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Общая доступность [API административных единиц](/graph/api/resources/administrativeunit), позволяющих организациям делить Azure Active Directory на подразделения, а также управлять административными обязанностями и делегировать их этим подразделениям. Эти подразделения могут представлять регионы, отделы, места возникновения затрат и т. д.

### <a name="reports"></a>Отчеты
[Получите отчет, включающий количество уникальных пользователей](/graph/api/reportroot-getemailappusageversionsusercounts) для Outlook 2019 и Outlook в Microsoft 365.

### <a name="teamwork"></a>Командная работа
- Получите свойство **lastEditedDateTime**, чтобы узнать, когда отправитель последний раз внес изменения в [сообщение чата](/graph/api/resources/chatmessage).
- Получите свойство **lastModifiedDateTime**, чтобы узнать, когда отправитель создал сообщение чата или когда любой пользователь изменил его другими способами, в том числе добавив или удалив реакции. 
- [Получайте уведомления об изменениях](webhooks.md) в [сообщениях чата](/graph/api/resources/chatmessage).
- [Обновите](/graph/api/chatmessage-update?view=graph-rest-beta&preserve-view=true) свойство **policyViolation** объекта [chatMessage](/graph/api/resources/chatmessagepreserve-view=true) в [канале](/graph/api/resources/channel&preserve-view=true) или [чате](/graph/api/resources/chat&preserve-view=true), позволив приложениям защиты от потери данных (DLP) отслеживать [нарушения политики сообщений чатов](/graph/api/resources/chatmessagepolicyviolation?preserve-view=true), чтобы сообщения не содержали данные, которые пользователи не должны отправлять.

### <a name="use-the-sdks"></a>Использование пакетов SDK
Общая доступность пакета [SDK PowerShell Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-powershell), обеспечивающего понятный и согласованный доступ ко всем возможностям Microsoft Graph.

### <a name="use-the-toolkit"></a>Использование набора средств
Воспользуйтесь новыми пошаговыми руководствами по началу работы для набора средств Microsoft Graph и насладитесь удобством набора средств:
- [Создание веб-приложения в JavaScript](./toolkit/get-started/build-a-web-app.md)
- [Создание веб-части SharePoint](./toolkit/get-started/build-a-sharepoint-web-part.md)
- [Создание вкладки Microsoft Teams](./toolkit/get-started/build-a-microsoft-teams-tab.md)
- [Использование набора средств с помощью React](./toolkit/get-started/use-toolkit-with-react.md)
- [Использование набора средств с помощью Angular](./toolkit/get-started/use-toolkit-with-angular.md)

### <a name="users"></a>Пользователи
Помимо получения SMTP-адреса [пользователя](/graph/api/resources/user) с помощью свойства **mail**, теперь вы можете установить это свойство и обновить адрес электронной почты пользователя. 

## <a name="september-2020-new-in-preview-only"></a>Сентябрь 2020г.: новые возможности только в предварительной версии

### <a name="application"></a>Для приложений
Создание, перечисление и удаление [классификаций делегированных разрешений](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true), применяемых [субъектом-службой](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true). Используйте классификации делегированных разрешений в сочетании с [параметрами согласия пользователей](/azure/active-directory/manage-apps/configure-user-consent), чтобы устанавливать ограничения на то, когда пользователям разрешено предоставлять согласие приложениям.

### <a name="cloud-communications"></a>Облачные коммуникации
- Не рекомендуется использовать свойства **autoAdmittedUsers** из [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Вместо этого следует использовать новое свойство **lobbyBypassSettings** и его [значения](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
- Используйте дополнительные параметры, связанные для объявления звонящим о присоединении или выходе из собрания по сети (свойство **isEntryExitAnnounced**), и разрешения конкретных выступающих доступа к собранию (свойство **allowedPresenters**).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- [Получите документы для каждого задания печати, связанного с принтером](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true), применив `$expand` [параметр запроса системы OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters). 
- Отфильтруйте задания печати по пользователю, который их создал, применив `$filter` [параметр системного запроса OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [сентябрь](changelog.md#september-2020) для бета-версии.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- [Получите ключ восстановления BitLocker](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true) от имени вошедшего пользователя, который является владельцем устройства или выполняет соответствующую роль. При получении ключа восстановления создается [журнал аудита](/azure/active-directory/reports-monitoring/concept-audit-logs) наравне с пользовательским интерфейсом.
- Получите общее и использованное значение [квоты каталога](/graph/api/resources/directorysizequota?view=graph-rest-beta&preserve-view=true) в [организации](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) с помощью свойства **directorySizeQuota**.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
Вы можете включить [расписание](/graph/api/resources/requestschedule?view=graph-rest-beta&preserve-view=true) при запросе или удалении [назначения пользователя на пакет доступа](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true), который определяет доступ к группам, приложениям или сайтам SharePoint.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Организации могут [получить](/graph/api/continuousaccessevaluationpolicy-get?view=graph-rest-beta&preserve-view=true) или [обновить](/graph/api/continuousaccessevaluationpolicy-update?view=graph-rest-beta&preserve-view=true) [политику оценки непрерывного доступа](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true), чтобы управлять сеансами проверки подлинности в режиме реального времени.

### <a name="search"></a>Поиск

- Используйте дополнительные возможности в [API Поиска (Майкрософт)](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) для соединителей OneDrive, SharePoint, Microsoft Graph: 

  - Получайте [дополнительные типы](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types) содержимого из OneDrive и SharePoint: **drive**, **list**, **listItem** и **site**. 
  - Объединяйте свойства в области в результатах поиска для [выбранных свойств](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#get-selected-properties). 
  - Получайте настраиваемые свойства в ресурсах [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true).
  - [Сортируйте](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#sort-search-results) результаты поиска для OneDrive и SharePoint с помощью любого свойства, поддерживающего сортировку.
  - [Уточняйте результаты с помощью агрегатов](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#refine-results-using-aggregations) для OneDrive и SharePoint.
- Запрашивайте внешние данные, принятые соединителями Microsoft Graph, в [нескольких связях](./search-concept-custom-types.md).
- Воспользуйтесь улучшенным содержимым для соединителей Microsoft Graph, чтобы узнать о следующем:
  - [Управление связями](connecting-external-content-manage-connections.md)
  - [Управление схемой](connecting-external-content-manage-schema.md)
  - [Управление элементами](connecting-external-content-manage-items.md)
- Отслеживайте состояние [подключения](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) Microsoft Graph.
- Определите [внешнюю группу](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true), чтобы задать разрешения для объектов [внешних элементов](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true), добавленных в [подключение](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) Microsoft Graph. Внешние группы могут представлять группы, не относящиеся к Azure Active Directory, или похожие на группы конструкции, например бизнес-подразделения, которые устанавливают разрешения для содержимого во внешнем источнике данных.

### <a name="teamwork"></a>Командная работа
- Узнайте о дате и времени создания [канала](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) или [команды](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) Teams.


## <a name="august-2020-new-and-generally-available"></a>Август 2020 г.: новые и общедоступные возможности

### <a name="change-notifications"></a>Уведомления об изменениях
[Отслеживание изменений](delta-query-overview.md) поддерживаемых ресурсов в национальном облаке Microsoft Graph для государственных организаций США.

### <a name="cloud-communications"></a>Коммуникации из облака
- [Отмените](/graph/api/call-cancelmediaprocessing) любые действия интерактивного голосового ответа (IVR), выполняемые или находящиеся в очереди, которые [воспроизводят звуковой сигнал](/graph/api/call-playprompt) или [записывают ответ](/graph/api/call-record).
- Получите [сведения о расшифровке звонка](/graph/api/resources/calltranscriptioninfo) с помощью свойства **transcription**.

### <a name="teamwork"></a>Командная работа
- Используйте альтернативный способ [создания группы](/graph/api/team-post) без предварительного создания группы.
- Используйте свойство навигации **участники**, чтобы добавить участников в команду с большей надежностью и меньшей задержкой.
- Узнайте, в каком состоянии находится публикация [приложения](/graph/api/resources/teamsapp) Microsoft Teams с помощью свойства **publishingState** [определения приложения](/graph/api/resources/teamsappdefinition). Возможные значения состояния публикации: `submitted`, `published` и `rejected`. См. [пример](/graph/api/teamsapp-list?view=graph-rest-beta&preserve-view=true#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state).
- Воспользуйтесь делегированным разрешением `AppCatalog.Submit`, чтобы позволить пользователю [отправить приложение](/graph/api/teamsapp-publish) и оформить запрос на его проверку администратором. С помощью этого же разрешения пользователь может [отменить](/graph/api/teamsapp-delete) отправленное ранее приложение, которое не было опубликовано. 


## <a name="august-2020-new-in-preview-only"></a>Август 2020 г.: новые возможности только в предварительной версии

### <a name="applications"></a>Приложения
Поддержка единого входа на основе паролей в ресурсах приложения [субъекта-службы](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) и указание таких [параметров](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta&preserve-view=true) в свойстве **passwordSingleSignOnSettings**. Сведения о едином входе на основе паролей в Azure AD см. в статье [Настройка единого входа на основе пароля](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).

### <a name="calendar"></a>Календарь
Улучшенная программная поддержка сценариев, в которых используется повторяющееся [событие](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true):
- надежный поиск экземпляра события в повторяющемся ряду, в том числе измененного или отмененного, с помощью свойства **occurrenceId**;
- поиск любых исключений в ряду повторяющихся экземпляров события с помощью свойства **exceptionOccurrences**;
- поиск любых отмен в ряду повторяющихся экземпляров события с помощью свойства **cancelledOccurrences**.

### <a name="change-notifications"></a>Уведомления об изменениях
- Используйте свойство **includeResourceData** ресурса [subscription](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) для [настройки уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md). Не используйте свойство **includeProperties** свойства.
- Получение [уведомлений об изменениях, доставляемых через концентратор событий](change-notifications-delivery.md).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Предоставление всем пользователям и группам возможности [совместного использования принтера](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) с помощью свойства **allowAllUser**.
- С помощью новых делегированных разрешений и разрешений для приложений можно пользоваться и управлять [печатью документа](/graph/api/resources/printDocument?view=graph-rest-beta&preserve-view=true), [заданием на печать](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true), [принтером](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), [предоставлением общего доступа к принтеру](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) и [определением операции печати](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true). Подробные сведения об облачной печати см. в обновлении за [август](changelog.md#august-2020).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune в бета-версии за [август](changelog.md#august-2020).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Настройка [условий соглашения об использовании](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) для поддержки срока действия и периодичности соглашения с обязательным принятием пользователем соглашения на отдельных устройствах или повторным принятием соглашения с установленной периодичностью. 
- Используйте свойство **file** для перехода к [настраиваемому соглашению](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) условий. Не используйте **файлы** свойства.
- Добавление, удаление и перечисление внутренних или внешних кураторов, которые могут утверждать запросы от [подключенной организации](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true) на доступ к группе, приложению или сайту SharePoint Online. Дополнительную информацию см. в разделе [Управление правами](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Разрешите дальнейшую настройку [политики авторизации](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) для клиента, например разрешите [роли пользователя по умолчанию](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true) создавать приложения или группы безопасности или читать других пользователей, разрешите пользователям возможность подписываться на подписки через электронную почту или присоединяться к клиенту через проверку электронной почты, а также предоставьте пользователям возможность самостоятельного сброса пароля.
- Управляйте [предопределенными, настраиваемыми политиками как пользовательскими потоками в клиенте Azure Active Directory B2C](/graph/api/resources/b2cuserflows?view=graph-rest-beta&preserve-view=true). См. Дополнительные сведения о [пользовательских потоках B2C](/azure/active-directory-b2c/user-flow-overview).
- Включите [возможность самостоятельной регистрации в качестве пользовательских потоков B2X в клиенте Azure Active Directory](/graph/api/resources/b2xuserflows?view=graph-rest-beta&preserve-view=true). См. дополнительные сведения о [самостоятельной регистрации](/azure/active-directory/external-identities/self-service-sign-up-overview).

### <a name="people-and-workplace-intelligence--profile"></a>Люди и рабочая аналитика | Профиль
Добавление следующих дополнительных свойств пользовательского [профиля](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true) и управление ими. Их можно отображать в общих для пользователей интерфейсах в Microsoft 365 и сторонних приложениях:
- [addresses](/graph/api/resources/itemAddress?view=graph-rest-beta&preserve-view=true)
- [anniversaries](/graph/api/resources/personAnniversary?view=graph-rest-beta&preserve-view=true)
- [awards](/graph/api/resources/personAward?view=graph-rest-beta&preserve-view=true)
- [certifications](/graph/api/resources/personCertification?view=graph-rest-beta&preserve-view=true)
- [notes](/graph/api/resources/personAnnotation?view=graph-rest-beta&preserve-view=true)
- [patents](/graph/api/resources/itemPatent?view=graph-rest-beta&preserve-view=true)
- [publications](/graph/api/resources/itemPublication?view=graph-rest-beta&preserve-view=true)


### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Получение [отчетов об использовании приложений Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta&preserve-view=true), в частности сведений о пользователе, количества пользователей и количества используемых платформ.

### <a name="teamwork"></a>Командная работа
Получение [контента, размещенного в сообщении чата](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true), например изображений или фрагментов кода. См. [пример](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&preserve-view=true&branch=master#example-2-get-hosted-content-bytes-for-an-image), чтобы получить количество байтов содержимого для изображения.

### <a name="to-do-tasks"></a>Задачи To-Do
- Появление нового набора API для [Microsoft To Do](todo-concept-overview.md), позволяющего пользователям приложения упорядочивать и отслеживать личные задачи в клиентских приложениях Microsoft 365. Дополнительные сведения см. в статье [Использование API Microsoft To Do](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true).
- Прекращение поддержки [API задач Outlook](/graph/api/resources/outlooktask?view=graph-rest-beta&preserve-view=true).


## <a name="july-2020-new-and-generally-available"></a>Июль 2020 г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
GA функции, которая позволяет организаторам предлагать альтернативное время собраний, а приглашенным [предлагать новое время для собрания](outlook-calendar-meeting-proposals.md), когда они [предварительно принимают](/graph/api/event-tentativelyaccept?view=graph-rest-1.0&preserve-view=true&preserve-view=true) или[отклоняют](/graph/api/event-decline?view=graph-rest-1.0&preserve-view=true&preserve-view=true) событие.

### <a name="change-notifications"></a>Уведомления об изменениях
Удалено ошибочно реализованное свойство **sequenceNumber** из ресурса [changeNotification](/graph/api/resources/changenotification).

### <a name="groups"></a>Группы
Общая доступность следующих свойств объекта [group](/graph/api/resources/group): **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage** и **theme**.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Удаление пользователя в качестве зарегистрированного владельца или пользователя [устройства](/graph/api/resources/device).
- Отслеживайте изменения в новых, обновленных или удаленных локальных представлениях приложений (представленных ресурсами[servicePrincipals](/graph/api/resources/serviceprincipal)) и делегированных разрешениях (представленных ресурсами [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant)) без полного чтения всей коллекции ресурсов.
- GA [политики обеспечения безопасности по умолчанию](/graph/api/resources/identitysecuritydefaultsenforcementpolicy), которая защищает организации от распространенных атак.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- GA [политик условного доступа](/graph/api/resources/conditionalAccessPolicy), которые являются настраиваемыми правилами, определяющими сценарии доступа.
- GA [именованных расположений](/graph/api/resources/namedLocation), представляющих собой настраиваемые правила, которые определяют сетевые расположения, используемые в политике условного доступа.

### <a name="schema-extensions"></a>Расширения схемы
Функция [расширений схемы](/graph/api/resources/schemaextension) теперь общедоступна в [Microsoft Cloud for US Government](./deployments.md).

### <a name="teamwork"></a>Командная работа
Используйте делегированные разрешения `TeamsAppInstallation.ReadForTeam` или`TeamsAppInstallation.ReadWriteForTeam`, или разрешения приложений `TeamsAppInstallation.ReadForTeam.All` или `TeamsAppInstallation.ReadWriteForTeam.All`, чтобы [составить список приложений, установленных в группе](/graph/api/teamsappinstallation-list).

## <a name="july-2020-new-in-preview-only"></a>Июль 2020 г.: новые возможности только в предварительной версии

### <a name="cloud-communications"></a>Облачные коммуникации
- Использование операции [update](/graph/api/onlinemeeting-update?view=graph-rest-beta&preserve-view=true&preserve-view=true), чтобы обновить свойство **startDateTime**, **endDateTime**, **participants** или **subject** для [собрания по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true&preserve-view=true).
- Подписка на уведомления об изменениях о доступности пользователя в Microsoft Teams, представленной ресурсом [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--call-records"></a>Облачные коммуникации | Записи звонков
- [Получение](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta&preserve-view=true) записей звонков по ТСОП.
- [Получение](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta&preserve-view=true) записей звонков прямой маршрутизации.

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Появление [дел обнаружения электронных данных](/graph/api/resources/ediscoverycase?view=graph-rest-beta&preserve-view=true), которые могут содержать хранителей, удержания, коллекции, наборы для проверки и операции экспорта, доступные для использования в качестве доказательств в судебных делах.
Приложения теперь могут [запрашивать](/graph/api/resources/reviewsetquery?view=graph-rest-beta&preserve-view=true) и вызывать [данные наборов для проверки](/graph/api/resources/reviewset?view=graph-rest-beta&preserve-view=true), собранные для использования в судебных разбирательствах, расследованиях и нормативных запросах. Это добавление входит в состав [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true) Microsoft 365.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Использование разрешения приложений `Printer.ReadWrite.All` и [шифрования Internet Printing Protocol (IPP)](https://tools.ietf.org/html/rfc8010) для [обновления принтера](/graph/api/printer-update?view=graph-rest-beta&preserve-view=true).
- Использование разрешений приложений `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All` или `PrintJob.ReadWrite.All` для [получения задания печати](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true) или [перечисления заданий печати для принтера](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- При [получении задания печати](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true) используйте `$expand` для получения [задач печати](/graph/api/resources/printtask?view=graph-rest-beta&preserve-view=true), выполняемых или выполненных в рамках задания. Задачи печати, [определения задач](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true) и [триггеры задач](/graph/api/resources/printtasktrigger?view=graph-rest-beta&preserve-view=true) используются при [печати по запросу](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).
- [Перенаправление задания печати](/graph/api/printjob-redirect?view=graph-rest-beta&preserve-view=true) на другой принтер в рамках печати по запросу.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [июль](changelog.md#july-2020) в бета-версии.

### <a name="groups"></a>Группы
Используйте свойство **isAssignableToRole** [группы](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) Microsoft 365 и настройте его при создании группы, чтобы указать, можно ли назначить группу для роли Azure AD. Эта [помогает управлять назначениями ролей в Azure AD](/azure/active-directory/users-groups-roles/roles-groups-concept). Например, вместо назначения отдельным пользователям роли Azure AD привилегированный администратор ролей или глобальный администратор может создать группу Microsoft 365 и назначить ее этой роли, чтобы при присоединении пользователей к _группе_ им неявно назначалась нужная роль.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Получите маркер доступа](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta&preserve-view=true) для авторизации службы контроля использования Azure AD для предоставления пользователям доступа к приложению.
- [Получите](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta&preserve-view=true) или[обновите](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta&preserve-view=true)настройки управления правами, которые контролируют доступ к группам, приложениям и сайтам SharePoint Online для пользователей внутри или вне вашей организации. 

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Включение уровней риска пользователя (`low`, `medium`, `high`, `none`) при рассмотрении применения [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- [Использование смены пароля в качестве предоставления управления](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta&preserve-view=true#special-considerations-when-using-passwordchange-as-a-control), чтобы пройти политику условного доступа.
- Использование [поставщика Open ID Connect](/graph/api/resources/openidconnectprovider?view=graph-rest-beta&preserve-view=true) (ODIC) в качестве поставщика удостоверений в клиенте Azure AD и клиенте Azure AD B2C. Его свойство **claimsMapping** позволяет Azure AD [сопоставлять утверждения](/graph/api/resources/claimsmapping?view=graph-rest-beta&preserve-view=true) от поставщика OIDC с утверждениями, которые распознает и использует Azure AD.

### <a name="people-and-workplace-intelligence--insights"></a>Люди и рабочая аналитика | Аналитические сведения
Используйте более [детальное управление конфиденциальностью](insights-customize-item-insights-privacy.md) в отношении доступности и отображения[элементов аналитики](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true) в Microsoft 365. Эти данные представляют собой отношения между пользователем и документами в OneDrive для бизнеса, вычисляемые с использованием передовых методов анализа и машинного обучения. 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>Люди и рабочая аналитика | Настройка карточки профиля
Администраторы могут [настроить свойства, представленные в карточке профиля для своих организаций](add-properties-profilecard.md), используя API-интерфейс для [свойств карточки профиля](/graph/api/resources/profilecardproperty?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Сайты и списки
Доступ к таксономии [банка терминов](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true) SharePoint — иерархии, состоящей из ресурсов [group](/graph/api/resources/termstore-group?view=graph-rest-beta&preserve-view=true), [set](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true) и [term](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true), а также ресурсов [relation](/graph/api/resources/termstore-relation?view=graph-rest-beta&preserve-view=true) для связей между терминами.

### <a name="workbooks-and-charts"></a>Книги и диаграммы
[Получение состояния и любого результата](/graph/api/workbookoperation-get?view=graph-rest-beta&preserve-view=true) длительной [операции](/graph/api/resources/workbookoperation?view=graph-rest-beta&preserve-view=true) в [книге](/graph/api/resources/workbook?view=graph-rest-beta&preserve-view=true).



## <a name="june-2020-new-and-generally-available"></a>Июнь 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
- Использование `Accept-Language` заголовка HTTP при [создании онлайнового собрания](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0&preserve-view=true&preserve-view=true) для предоставления объединенной информации на основе языковой среды.
- Использование [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0&preserve-view=true&preserve-view=true) для возврата онлайнового собрания с указанным значением **externalId** или его создание в случае отсутствия, чтобы упростить внедрение получившегося собрания в стороннем календаре.

### <a name="files"></a>Файлы
- Улучшенная поддержка синхронизации:
  - Использование свойства **pendingOperations** для определения [операций](/graph/api/resources/pendingoperations), которые могут обновить бинарное содержание файла [driveItem](/graph/api/resources/driveitem), ожидающего выполнения.
  - [Восстановление](/graph/api/driveitem-restore) объекта **driveItem**, который был удален и находится в корзине OneDrive персональный.
- Получение или настройка ориентации ресурса [photo](/graph/api/resources/photo). Настройка поддерживается в OneDrive персональный.
- Использование защищенного алгоритма хэширования (SHA-256) для улучшения безопасности и целостности данных ресурса [file](/graph/api/resources/file).
- Использование параметра `deferCommit` для откладывания окончательного создания при [передаче, как правило, большого файла](/graph/api/driveitem-createuploadsession) в OneDrive для бизнеса до тех пор, пока приложение не выполнит запрос на выполнение передачи.
- Использование свойства **fileSize** для предоставления оценки как части параметра **item**, чтобы проверить квоту до [передачи файла](/graph/api/driveitem-createuploadsession) в OneDrive персональный.
- Поиск [storagePlanInformation](/graph/api/resources/storageplaninformation) с помощью свойства **quota** ресурса [drive](/graph/api/resources/drive), чтобы проверить доступность планов с более высокими квотами на хранение.

### <a name="groups"></a>Группы
Использование разрешений приложений `Group.Read.All` и `Group.ReadWrite.All` для получения ресурсов группы [беседа](/graph/api/resources/conversation) и [цепочки беседы](/graph/api/resources/conversationthread).

### <a name="identity-and-access"></a>Удостоверение и доступ 
- Общедоступная версия из двух наборов API для [защиты удостоверения](/graph/api/resources/identityprotectionroot): API [выявления рисков](/graph/api/resources/riskdetection) и [рискованных пользователей](/graph/api/resources/riskyuser).

### <a name="security"></a>Безопасность
- Отслеживание указанного ниже как свойств [оповещения](/graph/api/resources/alert?view=graph-rest-1.0&preserve-view=true&preserve-view=true):
  - Идентификаторы инцидентов, связанных с оповещением.
  - Идентификация [ресурса](/graph/api/resources/securityResource?view=graph-rest-1.0&preserve-view=true#securityresourcetype-values) как атакованного или как связанного ресурса в оповещении.
  - Указание начального и конечного расположений [сетевого подключения](/graph/api/resources/networkconnection?view=graph-rest-1.0&preserve-view=true), связанных с оповещением.

### <a name="sites-and-lists"></a>Сайты и списки
Указание геолокационных данных в [определении столбца](/graph/api/resources/columndefinition) для ресурса [списка](/graph/api/resources/list) SharePoint.

### <a name="teamwork"></a>Командная работа
- Использование делегированного разрешения [AppCatalog.Read.All](./permissions-reference.md#appcatalog-resource-permissions) для перечисления [приложений](/graph/api/resources/teamsapp?view=graph-rest-1.0&preserve-view=true) из каталога приложений Microsoft Teams.
- [Получение информации о папке](/graph/api/channel-get-filesfolder) с сопоставлением вкладки **Файлы** [канала](/graph/api/resources/channel) Teams.
- [Получение канала по умолчанию](/graph/api/team-get-primarychannel) с меткой **Общие** [команды](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Июнь 2020 г.: новые возможности только в предварительной версии

### <a name="calendar"></a>Календарь
Помимо отслеживания инкрементных изменений событий в **calendarView** (коллекции или событий, ограниченных начальными _и_ конечными данными), применяется функция [delta](/graph/api/event-delta?view=graph-rest-beta&preserve-view=true) к событиям в почтовом ящике пользователя или к событиям в календаре определенного пользователя.

### <a name="cloud-communications--presence"></a>Облачные коммуникации | Присутствие
[Получение статуса присутствия](/graph/api/presence-get?view=graph-rest-beta&preserve-view=true) всех пользователей в организации или определенного пользователя организации.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Указание [полей печати](/graph/api/resources/printmargin?view=graph-rest-beta&preserve-view=true) при настройке [документа для печати](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true).
- Поддержка следующих [возможностей принтера](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true):
  - направления подачи;
  - печати диапазонов страниц;
  - разрешение печати в точках на дюйм;
  - максимальный размер очереди заданий печати в байтах;
  - входные лотки;
  - поля;
  - разбор по копиям;
  - масштабирование документов.
- Поддержка разрешения печати (в точках на дюйм) и масштабирование документов как часть [настроек принтера по умолчанию](/graph/api/resources/printerdefaults?view=graph-rest-beta&preserve-view=true).
- Поддержка следующих настроек [конфигурации документов](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta&preserve-view=true):
  - входные лотки;
  - выходные лотки;
  - размеры носителей;
  - поля;
  - типы носителей;
  - финишная обработка, например сшивание или брошюрование;
  - количество страниц на лист;
  - многостраничный макет с указанием направления при размещении страниц на листе;
  - разбор по копиям;
  - масштабирование.
- Расширение документов при [перечислении заданий печати](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- [Регистрация принтера]() и использование ресурса [printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta&preserve-view=true) для отслеживания и проверки регистрации принтера.
- [Получение долгосрочной регистрации принтера](/graph/api/printoperation-get?view=graph-rest-beta&preserve-view=true) для текущего пользователя или клиента приложения.
- Несколько переименований свойств и типов нумерации. Более подробные сведения приведены в обновлениях журнала изменений для облачной печати за [июнь](changelog.md#june-2020).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [июнь](changelog.md#june-2020) в бета-версии.

### <a name="education"></a>Образование
- Возможность использовать делегированные разрешения `EduRoster.ReadBasic` для [получения](/graph/api/educationuser-get?view=graph-rest-beta&preserve-view=true) идентификатора [преподавателя](/graph/api/resources/educationteacher?view=graph-rest-beta&preserve-view=true) или [учащегося](/graph/api/resources/educationstudent?view=graph-rest-beta&preserve-view=true) во внешней исходной программе как свойство **externalId**.
- Использование свойства **externalSource** для отслеживания значения `lms`, если [организация](/graph/api/resources/educationorganization?view=graph-rest-beta&preserve-view=true) или [класс](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) в сфере образования созданы в системе управления обучением (LMS).

### <a name="identity-and-access"></a>Удостоверение и доступ
- ИТ-специалисты могут использовать ресурсы [connector](/graph/api/resources/connector?view=graph-rest-beta&preserve-view=true). Это легкие агенты для подключения к [прокси приложения Azure AD](/azure/active-directory/manage-apps/what-is-application-proxy) и [внешней публикации локальных веб-приложений](/graph/api/resources/onpremisespublishing?view=graph-rest-beta&preserve-view=true), чтобы удаленные пользователи организации могли безопасно получить доступ к этим приложениям.
- Управление [политикой проверки подлинности](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta&preserve-view=true) на уровне клиента для включения или отключения [регистрации с самообслуживанием](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta&preserve-view=true) внешних пользователей.
- [Подготовка учетной записи пользователя по требованию](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta&preserve-view=true) и возможность указывать объекты для выполнения правил подготовки и синхронизации.

### <a name="search"></a>Поиск
- Использование улучшения [свойства](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true) в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true) **isRefinable** для включения фильтрации результатов поиска и более точного управления взаимодействием при поиске, а также **псевдонимов** и **меток** для повышения релевантности.
- Возможность указать до 128 ресурсов **свойства** в **схеме**.
- Использование [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta&preserve-view=true) для диагностики.

### <a name="users"></a>Пользователи
- Использование свойства **userPurpose** [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) для выявления и дифференциации почтового ящика для одного пользователя от общего почтового ящика и почтового ящика оборудования в Exchange Online. 
- Использование [настроек пользователей](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) для [получения](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) или [обновления](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) [предпочитаемых языков и региональных настроек](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta&preserve-view=true).
- Настройки пользователей — это взаимосвязь, доступная через [пользователя](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true), которая обеспечивает единообразное взаимодействие с пользователем в разных приложениях за счет использования профиля Azure AD для применения одних и тех же предпочтений пользователя. См. статью [чем пользовательские параметры отличаются от параметров почтового ящика.](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true#user-preferences-for-languages-and-regional-formats).


## <a name="may-2020-new-and-generally-available"></a>Май 2020 г.: новые и общедоступные возможности

### <a name="calendar--place"></a>Календарь | Место
Общедоступная версия [API мест](/graph/api/resources/place) в версии 1.0. Используйте этот API в производственных приложениях, чтобы получить, обновить или удалить [помещение](/graph/api/resources/room) или [список помещений](/graph/api/resources/roomlist) в клиенте. [Узнайте больше](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) о API мест.

### <a name="change-notifications"></a>Уведомления об изменениях
- Подпишитесь на уведомления об изменениях в Microsoft Cloud для государственных учреждений США.

### <a name="cloud-communications--call-records"></a>Облачные коммуникации | Записи звонков
- Общедоступная версия [API записи звонков](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0&preserve-view=true). Используйте ресурс [callRecord](/graph/api/resources/callrecord?view=graph-rest-1.0&preserve-view=true) для получения метаданных звонков и онлайн-собраний в Microsoft Teams и Skype.
- Подпишитесь на [уведомления об изменениях](./webhooks.md) для отслеживания изменений всех ресурсов **callRecord** в организации.
- [Список сеансов](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true) в **callRecord** и дополнительное [разворачивание каждого сеанса на сегменты списка](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true#example-2-get-session-list-with-segments) в записи звонка.
- Поддержка значений диапазонов на 60 ГГц (`frequency60GHz`) и `unknownFutureValue` WiFi конечной точки мультимедиа в сегменте.
- Поддержка голосовой почты в качестве возможного типа конечной точки на стороне службы в [сегменте](/graph/api/resources/callrecords-segment) связи.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [май](changelog.md#may-2020) в версии 1.0.

### <a name="graph-explorer"></a>Песочница Graph
Используйте множество новых функций [песочницы Graph](https://developer.microsoft.com/en-us/graph/graph-explorer), которые улучшают обучение и создание прототипов в песочнице. Например,
- Просматривайте фрагменты кода, соответствующие введенному запросу API REST, в C#, Java, JavaScript и Objective C.
- Войдя в систему с помощью клиента, просматривайте и копируйте маркер доступа в свое избранное клиентское приложение для REST.

Дополнительные сведения см. в статье [Новая песочница Graph теперь общедоступная](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/).

### <a name="groups"></a>Группы
- При синхронизации локального каталога с Azure Active Directory с помощью Azure AD Connect теперь возвращаются свойства **onPremisesDomainName**, **onPremisesNetBiosName** и **onPremisesSamAccountName** в составе ресурса [group](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true).
- Подпишитесь на уведомления об изменении для ресурсов [group](/graph/api/resources/group) в службе Microsoft Cloud для Китая, предоставляемой 21Vianet.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Общедоступная версия API субъектов-служб в версии 1.0 Используйте ресурс [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true) в производственных приложениях для программного управления экземплярами приложений и контроля того, что приложение может сделать в рамках вашего клиента. Вы можете управлять тем, кто может использовать приложение, к каким ресурсам у приложения есть доступ, таким как добавление учетных данных, обработка сертификатов с истекающим сроком действия, а также управление делегированными разрешениями и назначениями ролей приложения.
- Общедоступная версия API [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0&preserve-view=true), который регистрирует назначение [appRole](/graph/api/resources/approle?view=graph-rest-1.0&preserve-view=true) (представляющее утверждение `roles` в маркерах идентификатора и маркерах доступа) [пользователю](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), [группе](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) или [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true).
- Используйте Facebook в качестве поставщика удостоверений в Azure Active Directory.
- Используйте делегированное разрешение или разрешение приложения `AppRoleAssignment.ReadWrite.All`, чтобы разрешить приложению управлять предоставлением разрешений для разрешений приложений для любого API (включая Microsoft Graph) и назначений приложений для любого приложения, соответственно, при наличии вошедшего в систему пользователя или без него.


### <a name="microsoft-graph-sdks"></a>Пакеты SDK Microsoft Graph
См. новые рекомендации к SDK в отношении следующего:
- [Разбиение на страницы](./sdks/paging.md)
- [Пакетная обработка](./sdks/batch-requests.md)
- [Отправка больших файлов в OneDrive](./sdks/large-file-upload.md)
- [Настройка клиента службы SDK с помощью компонентов ПО промежуточного слоя для HTTP](./sdks/customize-client.md).

### <a name="teamwork"></a>Командная работа
- Если ваш сценарий предполагает онлайн-собрания в Teams, см. рекомендации [ Как выбрать](choose-online-meeting-api.md) между [API календаря](outlook-calendar-online-meetings.md) и [API облачных средств обмена данными](cloud-communications-online-meetings.md) для создания онлайн-собраний и подключения к ним.
- [Отправка сообщений](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) и [ответ](/graph/api/channel-post-messagereply?view=graph-rest-1.0&preserve-view=true) на сообщения в [канале](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true).
- Получите расположение OneDrive для бизнеса файлов для [канала](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true), используя свойство навигации **fileFolder**.

### <a name="teamwork--shifts"></a>Командная работа | Смены
Общедоступная версия [shifts API](/graph/api/resources/shift?view=graph-rest-1.0&preserve-view=true) в версии 1.0. Используйте этот API в производственных приложениях для создания, обновления и управления расписаниями сотрудников без компьютеров, чтобы обеспечить их взаимодействие и эффективность совместной работы.

### <a name="users"></a>Пользователи
- Подпишитесь на уведомления об изменении для ресурсов [user](/graph/api/resources/user) в службе Microsoft Cloud для Китая, предоставляемой 21Vianet.
- Отслеживайте состояние и дату/время последнего изменения состояния внешнего пользователя, который был [приглашен](/graph/api/invitation-post?view=graph-rest-1.0&preserve-view=true) присоединиться к организации, с помощью свойств **externalUserState** и **externalUserStateChangeDateTime** ресурса **user**.

## <a name="may-2020-new-in-preview-only"></a>Май 2020 г.: новые возможности только в предварительной версии

### <a name="change-notifications"></a>Уведомления об изменениях
- Используйте формально схематизированные типы [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta&preserve-view=true) и [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta&preserve-view=true) для обработки уведомлений об изменении ресурса. 
- Отслеживайте, находится ли уведомление в последовательности или утеряно, используя свойство **sequenceNumber** в ресурсе **changeNotification**.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Ресурсы [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) и [printerShare](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) теперь аналогичны и имеют одинаковые свойства.
- Очищены некоторые имена свойств и типов вокруг общих принтеров:
  - Чтобы получить список общих принтеров, зарегистрированных в клиенте, используйте свойство навигации **shared** в [печати](/graph/api/resources/print?view=graph-rest-beta&preserve-view=true). 
  - Дополнительные сведения см. в журнале изменений за[май](changelog.md#may-2020).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [май](changelog.md#may-2020) в бета-версии.

### <a name="groups"></a>Группы
- [Оцените](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta&preserve-view=true), является ли (может являться) пользователь или устройство членом динамической группы, используя существующее правило для [группы](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) или указанное правило. [Динамическое членство на основе правил](/azure/active-directory/users-groups-roles/groups-dynamic-membership) снижает административные издержки при добавлении и удалении участников.
- В Microsoft 365 при создании [группы](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) настройте поведение группы, указав варианты поведения в свойстве **resourceBehaviorOptions**. Например, вы можете разрешить участникам публиковать записи, подписывать новых участников в беседы, отключать приветственные сообщения электронной почты и скрывать группу в Outlook.
- Укажите ресурсы для подготовки в свойстве **resourceProvisioningOptions**, которые обычно не входят в объем создания [группы](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) по умолчанию. В настоящее время поддерживается подготовка группы в качестве [команды](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) с возможностями Microsoft Teams.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Применяйте параметры системного запроса OData (`$count`, `$filter`, `$search`) при получении коллекций сущностей, которые являются производными [directoryObject](/graph/api/resources/directoryObject). Вы можете выполнить [поиск определенных маркеров](/graph/search-query-parameter#using-search-on-directory-object-collections) в свойствах **displayName** и **description** этих сущностей, а также использовать OData cast для обрезки результатов **directoryObject** до определенных производных типов. Подробные сведения приведены в статье [Создание расширенных запросов в Microsoft Graph с использованием атрибутов $count, $filter, $search и $orderby](https://developer.microsoft.com/en-us/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/).
- В рамках [API защиты удостоверений](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true) используйте свойство **riskEventType**, чтобы [получить тип определенного риска](/graph/api/riskdetection-get?view=graph-rest-beta&preserve-view=true) или [получить тип риска в журнале пользователя](/graph/api/riskyuser-list-history?view=graph-rest-beta&preserve-view=true). Не используйте свойств **riskType**, так как оно устарело.
- Укажите типы клиентского приложения в свойстве **clientAppTypes** [набора свойств](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta&preserve-view=true) для [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Используйте делегированное разрешение `EntitlementManagement.Read.All`, чтобы разрешить приложению считывание пакетов доступа, а также связанных ресурсов по управлению правами от имени пользователя, выполнившего вход.
- Используйте делегированные разрешения или разрешения приложения `Application.Read.All` и `Application.ReadWrite.All`, чтобы [перечислить приложения](/graph/api/application-list?view=graph-rest-beta&preserve-view=true) в организации.
- Управляйте параметрами авторизации в Azure AD с использованием типа ресурса [authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Командная работа
- Приложения Teams, [поддерживающие единый вход (SSO),](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) могут указывать `WebApplicationInfo.id` из манифеста приложения Teams в свойстве **azureADAppId** в [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true).
- Используйте [детализированные разрешения](./permissions-reference.md#team-resource-specific-consent-permissions) для доступа к ресурсам [team](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) и [channel](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true).


## <a name="april-2020-new-and-generally-available"></a>Апрель 2020 г.: новые и общедоступные возможности

### <a name="calendar"></a>Календарь
- [Делитесь календарями или делегируйте их](outlook-share-or-delegate-calendar.md) программным способом, соответствующим пользовательскому интерфейсу Outlook. Поддерживается отслеживание разрешений текущего пользователя и состояния общего доступа к календарю, а также следующие возможности:
  - Для каждого [календаря](/graph/api/resources/calendar?view=graph-rest-1.0&preserve-view=true) теперь можно управлять [разрешениями](/graph/api/resources/calendarpermission?view=graph-rest-1.0&preserve-view=true) каждого пользователя, которому предоставлен доступ к календарю. 
  - Для каждого [почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true) теперь можно указать, кто получает сообщения о собраниях и ответы на эти сообщения: делегат, владелец почтового ящика или и тот, и другой. 
- [Создание или обновление события в виде собрания по сети](outlook-calendar-online-meetings.md):
  - В каждом **календаре** можно указать разрешенных и используемых по умолчанию поставщиков собраний по сети.
  - Можно создать или обновить [мероприятие](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), доступное по сети, и предоставить участникам сведения для присоединения к собранию по сети. 
  - В частности, можно использовать **onlineMeetingProvider** и **onlineMeeting** — это новые свойства **мероприятий**, с помощью которых можно задать или указать Microsoft Teams в качестве поставщика собраний по сети. Это временное решение [известной проблемы](known-issues.md#onlinemeetingurl-property-is-not-supported-for-microsoft-teams) со свойством **onlineMeetingUrl**.
- Добавление [файловых вложений до 150 МБ](outlook-large-attachments.md) в [событие](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Файлы
- [Извлекайте](/graph/api/driveitem-checkout?view=graph-rest-1.0&preserve-view=true) и [возвращайте](/graph/api/driveitem-checkin?view=graph-rest-1.0&preserve-view=true) файлы в OneDrive, чтобы управлять их обновлением и делать обновления доступными для других пользователей.
- Применяйте необязательный пароль и дату/время истечения срока действия в качестве параметров действий[пригласить](/graph/api/driveitem-invite?view=graph-rest-1.0&preserve-view=true) и [создать ссылку совместного доступа](/graph/api/driveitem-createlink?view=graph-rest-1.0&preserve-view=true) для совместного доступа к [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).
- Получите или задайте пароль и дату/время истечения срока действия [разрешения](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true), а также отслеживайте [identitySet](/graph/api/resources/identityset?view=graph-rest-1.0&preserve-view=true) пользователей, которым предоставлено разрешение на совместный доступ к **driveItem**.
- Получите [разрешение](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true) для [общего элемента диска](/graph/api/resources/shareddriveitem?view=graph-rest-1.0&preserve-view=true), используя свойство навигации **permission**.
- Ограничьте действия пользователей со [ссылкой совместного доступа](/graph/api/resources/sharinglink?view=graph-rest-1.0&preserve-view=true) только просмотром без возможности скачивания содержимого общего элемента **driveItem** в OneDrive для бизнеса или в SharePoint.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Чтобы управлять ролями и назначать доступ к ресурсам в провайдерах управления доступом на основе ролей (RBAC), таких как Microsoft Intune, используйте [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0&preserve-view=true). Ресурс **unifiedRoleAssignmentMultiple** поддерживает определение одной роли в массиве областей и назначение роли для нескольких субъектов (например, пользователей).
- Получите доступ к определенным типам [политик для организации](/graph/api/resources/policy-overview?view=graph-rest-1.0&preserve-view=true), используя `/policies`сегмент URL и указав тип политики. Например, организация может применить политику для автоматического выхода пользователя из веб-сеанса после периода бездействия; см. операции CRUD для экземпляров [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0&preserve-view=true). Это [серьезное изменение](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/), упрощающее обнаружение всех политик путем группировки всех типизированных политик в сегменте `/policies`. Доступ к другим типизированным политикам осуществляется аналогичным образом: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0&preserve-view=true) и [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0&preserve-view=true). 

### <a name="mail"></a>Почта
Добавление [файловых вложений до 150 МБ](outlook-large-attachments.md) в [сообщение](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true).

### <a name="sites-and-lists"></a>Сайты и списки
- [Список сайтов](/graph/api/sites-list-followed?view=graph-rest-1.0&preserve-view=true), на которые подписан пользователь.
- Определите географическую область [семейства веб-сайтов](/graph/api/resources/sitecollection?view=graph-rest-1.0&preserve-view=true) с помощью свойства **dataLocationCode**.
- Определите клиента файла, папки или другого элемента в SharePoint, путем доступа к свойству **tenantId**, которое является частью **sharepointIds** в [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).

## <a name="april-2020-new-in-preview-only"></a>Апрель 2020 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать

Назначьте разрешенным пользователям и группам доступ к определенным [общим принтерам](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) Универсальной печати — облачной инфраструктуры печати Microsoft 365. Чтобы воспользоваться возможностями надежного централизованного управления печатью и предложить пользователям простой, но полнофункциональный и безопасный интерфейс печати, ознакомьтесь с [объявлением Универсальной печати](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775) и присоединитесь к программе по ознакомлению с предварительной версией.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [апрель](changelog.md#april-2020).

### <a name="groups"></a>Группы
Определите, какое приложение создало [группу](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true), по идентификатору приложения.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Отслеживание изменений](/graph/api/administrativeunit-delta?view=graph-rest-beta&preserve-view=true), касающихся [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true).
- [Отслеживание изменений](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta&preserve-view=true), касающихся [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta&preserve-view=true).
- [Управление](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) пользовательскими [методами проверки подлинности](/graph/api/resources/authenticationmethod?view=graph-rest-beta&preserve-view=true), среди которых [пароль](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta&preserve-view=true) или [телефон](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta&preserve-view=true). Например, [сброс пароля пользователя](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta&preserve-view=true) и [получение состояния сброса](/graph/api/authenticationoperation-get?view=graph-rest-beta&preserve-view=true) или [добавление номера телефона](/graph/api/authentication-post-phonemethods?view=graph-rest-beta&preserve-view=true) пользователя для проверки подлинности с помощью SMS или голосового вызова, если для этого пользователя включена соответствующая политика.

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
[Список](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta&preserve-view=true) [проверяющих сторон](/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts), настроенных в службах федерации Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Просмотр данных о **созданных собраниях** и **действиях с уведомлениями о собраниях** в отчетах CSV, включающих [счетчики действий с электронной почтой](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta&preserve-view=true), [счетчики пользователей, совершающих действия с электронной почтой](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta&preserve-view=true) и [данные о действиях пользователей с электронной почтой](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta&preserve-view=true).


## <a name="march-2020-new-and-generally-available"></a>Март 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Облачные коммуникации
- Получите функцию маршрутизации вызовов и контекст входящих [вызовов](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true).
- [Обновите состояние записи](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0&preserve-view=true) звонка.
- Укажите информацию о записи для [участника](/graph/api/resources/participant?view=graph-rest-1.0&preserve-view=true), включая инициатора и состояние записи.
- Для уникальной идентификации участников конференции или [звонка](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) от участника к участнику используйте свойство **callChainId**.
- Определите как часть [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0&preserve-view=true) код страны и тип конечной точки (например, Skype для бизнеса или Skype для бизнеса VoIP) участника.
- Сторонние партнеры в области устройств видеоконференцсвязи (VTC) могут регистрировать и предоставлять сведения о качестве связи для своих устройств через бот Cloud Video Interop (CVI) с помощью функции [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0&preserve-view=true). Качество мультимедиа включает данные открытого типа для [звука](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0&preserve-view=true), [видео](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0&preserve-view=true) и [совместного использования экрана](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Файлы
- [Удаленные элементы](/graph/api/resources/remoteitem?view=graph-rest-1.0&preserve-view=true), к которым пользователю предоставлен общий доступ, добавленные в хранилище OneDrive пользователя или возвращенные как результаты поиска, могут содержать метаданные для изображения или видео.
- [Отслеживайте](/graph/api/driveitem-follow?view=graph-rest-1.0&preserve-view=true) объект [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true) для удобного доступа или упрощения таких действий, как перемещение, копирование и сохранение в определенном формате. Используйте [отмену отслеживания](/graph/api/driveitem-unfollow?view=graph-rest-1.0&preserve-view=true), чтобы прекратить отслеживание элемента диска.
- [Предоставьте](/graph/api/permission-grant?view=graph-rest-1.0&preserve-view=true) пользователям разрешение на доступ к ссылке для общего доступа, чтобы поделиться соответствующим элементом диска.

### <a name="identity-and-access"></a>Удостоверение и доступ
- [Отслеживайте изменения](/graph/api/orgcontact-delta?view=graph-rest-1.0&preserve-view=true) в [контактах организации](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true).
- Используйте свойство **riskEventTypes_v2**, чтобы получить типы событий риска, связанные с [входом](/graph/api/resources/signin?view=graph-rest-1.0&preserve-view=true).
- Используйте делегированное разрешение `User.ManageIdentities.All`, чтобы разрешить приложению считывать, обновлять и удалять удостоверения, связанные с учетной записью пользователя, к которой имеет доступ зарегистрированный пользователь. Используйте это разрешение на уровне приложения без зарегистрированного пользователя. Это позволяет приложению [определить](/graph/api/user-update?view=graph-rest-1.0&preserve-view=true), с помощью каких удостоверений пользователь может войти.

### <a name="reports"></a>Отчеты
Используйте Администратор службы Teams и Администратор связи Teams в качестве принятых ролей пользователя, чтобы приложения могли читать отчеты об использовании службы Microsoft 365 от имени пользователя в качестве [форм делегированной пользователем авторизации](reportroot-authorization.md). 

### <a name="sites"></a>Сайты
- Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-1.0&preserve-view=true) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-1.0&preserve-view=true) сайтов SharePoint. 
- [Подпишитесь на уведомления об изменениях](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) в [списке](/graph/api/resources/list?view=graph-rest-1.0&preserve-view=true) SharePoint.

## <a name="march-2020-new-in-preview-only"></a>Март 2020: Новое только в превью

### <a name="calendar"></a>Календарь
- Используйте свойство **calendarGroupId**, чтобы получить группу [календаря](/graph/api/resources/calendargroup?view=graph-rest-beta&preserve-view=true), в которой создан [календарь](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true).
- Используйте свойство **в черновике**, чтобы идентифицировать [событие](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) как собрание, которое пользователь обновил в Outlook, но не отправил для обновления участников.

### <a name="cloud-communications"></a>Облачные коммуникации
- Используйте [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta&preserve-view=true), чтобы получить экземпляр [онлайн-собрания](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) с помощью внешнего настраиваемого идентификатора или создать его, если он еще не существует.
- Вы можете использовать свойство **externalId**, чтобы определить онлайн-собрание с помощью внешнего настраиваемого идентификатора.
- Используйте необязательный заголовок HTTP-запроса `Accept-Language`, чтобы [создать](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true) или [получить](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) экземпляр онлайн-собрания. При успешном выполнении операции отображается содержимое свойства **joinInformation** на указанном языке и вариант локали.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [март](changelog.md#march-2020).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте разрешение `AuditLog.Read.All` для списка [действий входа](/graph/api/resources/signinactivity?view=graph-rest-beta&preserve-view=true) [пользователя](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).
- Используйте разрешение на уровне приложения `PrivilegedAccess.Read.AzureResources` для [управления привилегированными удостоверениями (PIM) ресурсов Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true), чтобы настроить рабочий процесс доступа «точно в срок» для ролей инфраструктуры Azure на уровне группы управления, подписки, группы ресурсов или ресурса.
- Используйте объект [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta&preserve-view=true), чтобы [получить](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta&preserve-view=true) или [обновить](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta&preserve-view=true) предварительно настроенные параметры безопасности по умолчанию, которые защищают организации от распространенных атак.
- Используйте сегмент `identity` при вызове API условного доступа. Например, чтобы [получить](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta&preserve-view=true) [политику условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true): `GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`.
- Используйте свойство **authenticationRequirement**, чтобы получить наивысший уровень проверки подлинности, необходимый для успешного выполнения всех действий [входа](/graph/api/resources/signin?view=graph-rest-beta&preserve-view=true).
- Используйте разбивку на страницы при [перечислении событий подготовки](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta&preserve-view=true) в вашем клиенте.

### <a name="search"></a>Поиск
- Чтобы добавить данные в файле к результатам поиска, просто индексируйте данные как [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true). Тип **externalFile** устарел.
- [Обновите](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) [элемент в индексе](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true), обновив представление элемента в виде обычного текста (представленное свойством **content**) или контейнер свойств элемента (представленный свойством **properties**). При обновлении любого свойства в контейнере свойств перезаписывается весь контейнер свойств, поэтому убедитесь, что все свойства элемента явным образом включены в обновление.
- Проверьте наличие `HTTP 429` и заголовка ответа `Retry-After` после вызова операции [создания](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true), [обновления](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) или [удаления](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) элемента **externalItem**. Самый быстрый способ выполнить восстановление после [регулирования](throttling.md#best-practices-to-handle-throttling) — отложить запросы с помощью задержки `Retry-After`.

### <a name="teamwork"></a>Командная работа
Используйте разрешение на уровне приложения `ChannelMessage.Read.All` для чтения экземпляров [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) в каналах без зарегистрированного пользователя.

### <a name="universal-print"></a>Универсальная печать
Появление [API универсальной печати](universal-print-concept-overview.md), позволяющего пользователям печатать в Интернете или из приложения. API позволяет ИТ-администраторам управлять доступом пользователей и групп к принтерам в облаке Microsoft 365, а также удаленным общим доступом к принтерам для поддерживания доступности, отслеживать состояние принтеров и создавать отчеты о заархивированных заданиях печати и использовании. 

Обратите внимание, что с марта 2020 г. _служба_ универсальной печати доступна в закрытой предварительной версии. Дополнительные сведения об участии см. в статье [Представляем универсальную печать: облачное решение для печати](https://aka.ms/announcinguniversalprint).


## <a name="february-2020-new-and-generally-available"></a>2020 февраля: новая и общедоступная

### <a name="calendar"></a>Календарь
Просмотрите пример [создания события в общем или делегированном календаре](outlook-create-event-in-shared-delegated-calendar.md), а также действия и свойства, доступные для делегата, приглашенных и владельца календаря во время этого процесса.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Чтобы повысить безопасность при подписке на [уведомления об изменениях пользовательских данных](webhooks.md), [установите Transport Layer Security (TLS) 1.2](/configmgr/core/plan-design/security/enable-tls-1-2) или выше на клиентах и серверах сайтов, используемых в процессе уведомления. Новое требование вводится поэтапно, начиная с 15 февраля 2020 года. К 15 мая 2020 года все конечные точки уведомления должны соответствовать новому требованию TLS. [Узнайте о стадиях развертывания](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) и при необходимости воспользуйтесь новым свойством **latestSupportedTlsVersion** в качестве временного решения, чтобы избежать сбоев подписки до выполнения обновления TLS.
- Используйте соответствующие типы [запроса оценки угроз](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0&preserve-view=true) для отслеживания угроз от [почты](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0&preserve-view=true), [файла сообщения электронной почты](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (. EML-файл), [файлов вложений электронной почты](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (текстовых файлов, файлов Word и двоичных файлов) и [URL-адреса](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0&preserve-view=true).

### <a name="users"></a>Пользователи
[Повторная обработка](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0&preserve-view=true) всех назначений лицензий на основе группы для [пользователя](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).


## <a name="february-2020-new-in-preview-only"></a>Февраль 2020: новое только в предварительном просмотре

### <a name="calendar"></a>Календарь
Просмотрите [задачи, поддерживаемые API-интерфейсами предварительного просмотра, которые управляют совместным использованием и делегированием календаря](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Коммуникации из облака

- Используйте новую [запись вызова ](/graph/api/resources/callrecord?view=graph-rest-beta&preserve-view=true) ресурс, чтобы получить метаданные звонков и собрания по сети в Microsoft Teams и Skype для бизнеса в Организации.
- Для участника собрания используйте свойство **инициатора**, чтобы получить идентификационную информацию инициатора [записи](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true), если таковая имеется.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [Февраль](changelog.md#february-2020)

### <a name="groups"></a>Группы
Используйте метод [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true), чтобы назначить лицензии для продуктов, таких как Microsoft 365 или Enterprise Mobility + Security, группе. Поскольку Azure AD обеспечивает назначение лицензий членам группы, для участников, вступающих в группу или покидающих ее, больше не требуется управление лицензиями на индивидуальном уровне.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Установите параметры запроса, утверждения и проверки при создании [политики назначения пакетов доступа](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true).
- Получите доступ к определенным типам [политик для организации](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true), используя `/policies`сегмент URL и указав тип политики. Например, организация может применить политику для автоматического выхода пользователя из веб-сеанса после периода бездействия; см. операции CRUD для экземпляров [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta&preserve-view=true). Это [серьезное изменение](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/), упрощающее обнаружение всех политик путем группировки всех типизированных политик в сегменте `/policies`. Доступ к другим типизированным политикам осуществляется аналогичным образом: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta&preserve-view=true) и [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta&preserve-view=true). 
- Используйте уровень приложения и делегированное `Policy.ReadWrite.ApplicationConfiguration`разрешение для операций чтения и записи в [политиках](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) конфигурации приложений, упомянутых в предыдущем пункте.

### <a name="teamwork"></a>Командная работа
- Используйте [уведомления об изменениях,](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true) всех сообщений канала или всех сообщений в Организации.
- [Отклоните](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta&preserve-view=true) [запрос на замену смен](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta&preserve-view=true) другим пользователем в [группе](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).

## <a name="january-2020-new-and-generally-available"></a>Январь 2020 г.: новые и общедоступные возможности

### <a name="security"></a>Безопасность
В рамках управления оповещениями используйте метод [обновления оповещений](/graph/api/alert-update?view=graph-rest-1.0&preserve-view=true) и обновляйте поле **комментариев** как `Closed in IPC` или `Closed in MCAS`.

### <a name="teamwork"></a>Командная работа
Используйте свойство навигации **primaryChannel** [группы](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) для доступа к каналу по умолчанию **General**.

### <a name="users"></a>Пользователи
Чтобы получить доступ к одному или нескольким удостоверениям, которые [пользователь](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true) может использовать для входа в учетную запись пользователя Azure AD, используйте свойство **удостоверения**. Удостоверения могут предоставляться поставщиками услуг Майкрософт, организаций или социальных удостоверений, таких как Facebook, Google или Microsoft. Это свойство позволяет пользователю входить в учетную запись пользователя с помощью любого из этих удостоверений.

## <a name="january-2020-new-in-preview"></a>Январь 2020: Новое в предварительной версии

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [Январь](changelog.md#january-2020).


## <a name="december-2019-new-and-generally-available"></a>Декабрь 2019 г.: новые и общедоступные возможности

### <a name="cloud-communications"></a>Коммуникации из облака
API коммуникаций из облака имеет общедоступное состояние, API ресурсов [call](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) и [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-1.0&preserve-view=true) [доступны в версии 1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0&preserve-view=true).

### <a name="education"></a>Образование
Используйте свойство **classSettings**, чтобы управлять параметрами для конкретного класса, например включением отправки еженедельных дайджестов заданий.  Это свойство доступно в ресурсе [team](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true), когда команда представляет собой [группу обучения](/graph/api/resources/educationclass?view=graph-rest-1.0&preserve-view=true).

### <a name="identity-and-access"></a>Удостоверение и доступ 
[При попытке получить объекты-контейнеры с ограниченными разрешениями часть данных возвращается](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects). В качестве примера можно привести экземпляр [группы](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true), связанный с [пользователем](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), другую **группу** и [устройство](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true). Приложение, у которого есть только разрешения User.Read.All и Group.Read.All, при попытке получить доступ к этому экземпляру **группы** получит объекты **user** и **group**, а также ограниченные данные для объекта **device** (только тип данных и ИД объекта), не включающие значения свойств.

### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика
API аналитики стал общедоступным. Используйте этот API в рабочих приложениях для определения наиболее релевантных документов, которые:

- [касаются](/graph/api/insights-list-trending?view=graph-rest-1.0&preserve-view=true) пользователя;
- [используются](/graph/api/insights-list-used?view=graph-rest-1.0&preserve-view=true) пользователем;
- [к которым предоставлен доступ](/graph/api/insights-list-shared?view=graph-rest-1.0&preserve-view=true) пользователю или пользователем.

### <a name="reports"></a>Отчеты
Чтобы получать отчеты об использовании Microsoft 365 с помощью разрешений, делегированных пользователем, администраторам необходимо назначить пользователю роль администратора Azure AD с ограниченными правами. Это может быть одна из следующих ролей: администратор организации, администратор Exchange, администратор SharePoint, администратор Lync, глобальный читатель или читатель отчетов. Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](reportroot-authorization.md).

### <a name="toolkit"></a>Набор средств
Выпущен набор средств Microsoft Graph версии 1.1. Список улучшений и исправлений ошибок см. в [разделе за декабрь 2019 г.](changelog.md#december-2019) журнала изменений.

## <a name="december-2019-new-in-preview"></a>Декабрь 2019 г.: новые возможности в предварительной версии

### <a name="cloud-communications"></a>Коммуникации из облака
- Чтобы получить сведения о доступности и текущей активности одного или нескольких пользователей, используйте новый ресурс [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true).
- [Удалите](/graph/api/onlinemeeting-delete?view=graph-rest-beta&preserve-view=true) экземпляр [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).
- Ознакомьтесь с [разделом за декабрь 2019 г.](changelog.md#december-2019) журнала изменений, чтобы переименовать или удалить несколько элементов ресурсов [call](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) и [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) и обеспечить соответствие версии v1 этих ресурсов.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [декабрь](changelog.md#december-2019)

### <a name="identity-and-access"></a>Удостоверение и доступ 
- Исправлено поведение отношений **appRoleAssignments** и **appRoleAssignedTo** в [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Используйте [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true) в [функции управления правами в Azure AD](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true) для запроса добавления ресурса к [каталогу](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true), чтобы роли этого ресурса можно было использовать в [пакете для доступа](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true).
- Используйте [API оценки угроз](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta&preserve-view=true), чтобы дать администраторам возможность сообщать о подозрительной почте, URL-адресах фишинга, вложениях электронной почты и других файлах. Вывод, сделанный при сканировании потока, может побудить их изменить политику организации соответствующим образом.

### <a name="teamwork"></a>Командная работа
- [Настройка уведомлений об изменениях, включающих данные](webhooks-with-resource-data.md) для ресурсов [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) в каналах и чатах Microsoft Teams.
- [Подписка на уведомления](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) о новых и измененных [сообщениях канала или чата](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true).
- Используйте ресурс [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta&preserve-view=true), чтобы включить указание доступности пользователя для назначения смен в [графике](/graph/api/resources/schedule?view=graph-rest-beta&preserve-view=true). Настройте эту возможность в [параметрах](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) пользователя.


## <a name="november-2019-new-and-generally-available"></a>Ноябрь 2019 г.: новые и общедоступные возможности

### <a name="groups"></a>Группы
- Использование разрешений приложения или делегированных разрешений GroupMember.Read.All и GroupMember.ReadWrite.All для перечисления групп, чтения основных свойств групп, считывания (и обновления при наличии разрешения на чтение и запись) сведений об участии в группах, к которым у приложения есть доступ.
- Использование разрешения приложения Group.Create для создания групп без необходимости входа пользователя.
- Для указанной [группы](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) [проверка участия](/graph/api/group-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) в других группах или ролях каталога.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Регистрация [приложений](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true), проходящих проверку подлинности в Azure Active Directory (Azure AD). Используйте делегированные [разрешения](./permissions-reference.md#application-resource-permissions), Application.Read.All и Application.ReadWrite.All, или разрешение приложения, Application.Read.All.
- Для указанного [устройства](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true) [проверка участия](/graph/api/device-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) в других группах или ролях каталога.

### <a name="mail"></a>Почта
- Использование свойства **conversationIndex** для получения положения сообщения в беседе электронной почты Outlook.
- Использование делегированного разрешения Mail.ReadBasic и разрешения приложения Mail.ReadBasic.All, чтобы получить ресурсы [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) или [mail folder](/graph/api/resources/mailfolder?view=graph-rest-1.0&preserve-view=true), отслеживать их изменения, а также управлять [подпиской](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) на уведомления об изменениях сообщений.

### <a name="users"></a>Пользователи
- [Проверка участия в группах](/graph/api/user-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) для определенного [пользователя](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).
- Использование свойства **creationType**, чтобы узнать, как была создана учетная запись пользователя, например была ли она создана в качестве обычной учебной или рабочей учетной записи либо в качестве внешней учетной записи и т. д.

## <a name="november-2019-new-in-preview"></a>Ноябрь 2019 г.: новые возможности в предварительной версии

### <a name="calendar"></a>Календарь
- [Организация и посещение собраний по сети с помощью Outlook](outlook-calendar-online-meetings.md).
- [Настройка свойств](/graph/api/place-update?view=graph-rest-beta&preserve-view=true) для расширенных типов расположений [комната](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) и [список комнат](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communication"></a>Облачное взаимодействие
Тип ресурса [call](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) поддерживает следующие дополнительные функции:

- [Контекст входящего звонка](/graph/api/resources/incomingcontext?view=graph-rest-beta&preserve-view=true)
- Тип конечной точки для участника, например голосовая почта или Skype для бизнеса
- Возможность [обновления](/graph/api/call-updaterecordingstatus?view=graph-rest-beta&preserve-view=true) [сведений о записи](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true) для [участника](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true)

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [ноябрь](changelog.md#november-2019)

### <a name="education"></a>Образование
Администраторы могут включать параметры на уровне класса с помощью свойства **classSettings** [команды](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), связанной с [классом](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true). В настоящее время существует параметр для уведомления опекунов о еженедельных заданиях.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Использование разрешения приложения Policy.Read.All для чтения всех политик условного доступа и именованных расположений организации без необходимости входа пользователя.
- Поддержка для [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) состояния только для отчета `enabledForReportingButNotEnforced`.
- Использование делегированного разрешения ThreatAssessment.ReadWrite.All или разрешения приложения ThreatAssessment.Read.All для чтения (или создания при наличии разрешения на чтение и запись) запросов на оценку угроз в организации.

### <a name="mail"></a>Почта
Использование делегированного разрешения Mail.ReadBasic и разрешения приложения Mail.ReadBasic.All, чтобы управлять [подписками](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) на уведомления об изменениях в ресурсе [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true).

### <a name="notifications"></a>Уведомления
Можно использовать новые компактные [веб-SDK](https://aka.ms/GNSDK) уведомлений вместо [SDK Project Rome](https://github.com/Microsoft/project-rome), чтобы воспользоваться улучшенной моделью проверки подлинности и поддержкой веб-приложений с push-уведомлениями. 

### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика
Первое появление ресурса [профиль](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true), который является расширенным представлением нового поколения записей людей в службах Майкрософт. Этот ресурс связан с распространенными и удобными атрибутами людей, включая информацию о всех важных датах, таких как [годовщины](/graph/api/resources/personanniversary?view=graph-rest-beta&preserve-view=true), а также об [образовании](/graph/api/resources/educationalactivity?view=graph-rest-beta&preserve-view=true), [должностях](/graph/api/resources/workposition?view=graph-rest-beta&preserve-view=true) и [интересах](/graph/api/resources/personinterest?view=graph-rest-beta&preserve-view=true), уровнях владения [языками](/graph/api/resources/languageproficiency?view=graph-rest-beta&preserve-view=true) и [навыками](/graph/api/resources/skillproficiency?view=graph-rest-beta&preserve-view=true), об [участии в проектах](/graph/api/resources/projectparticipation?view=graph-rest-beta&preserve-view=true) и [связи с веб-сайтами](/graph/api/resources/personwebsite?view=graph-rest-beta&preserve-view=true), а также прочие сведения об [учетной записи](/graph/api/resources/useraccountinformation?view=graph-rest-beta&preserve-view=true) и контактные данные.

### <a name="search"></a>Поиск
Первое появление [API Microsoft Search](search-concept-overview.md), с помощью которого пользователи приложений могут получать индивидуально адаптированные, более актуальные и релевантные результаты поиска с использованием возможностей Microsoft Graph. Можно использовать функцию [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true), которая по умолчанию выполняет поиск в сообщениях и событиях Outlook, а также в файлах OneDrive и SharePoint в облаке Майкрософт. Можно использовать [соединители](/microsoftsearch/connectors-overview), доступные в [коллекции соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы задействовать поисковые данные за пределами облака Майкрософт. Также можно [создавать собственные соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), индексировать внешние настраиваемые элементы и файлы, а также отправлять запросы к определенным внешним источникам данных.

### <a name="teamwork"></a>Командная работа
Получение ресурсов [file](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true), связанных с [командой](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) и [каналом](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true), с помощью следующего синтаксиса HTTP-запроса:

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>Пользователи
Использование свойства **creationType**, чтобы узнать, как была создана учетная запись пользователя, например была ли она создана в качестве обычной учебной или рабочей учетной записи либо в качестве внешней учетной записи и т. д.


## <a name="october-2019-new-and-generally-available"></a>Октябрь 2019 г.: новые и общедоступные возможности

### <a name="identity-and-access"></a>Идентификация и доступ
- Использование [контактов организации](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true) в рабочих приложениях. Контакты организации находятся под управлением администраторов организации и синхронизируются из локальной службы каталогов Active Directory или из Exchange Online.
- Настройка [проверки подлинности на основе сертификатов](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) в [организации](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true).
- Добавление и удаление [учетных данных с паролем](/graph/api/resources/passwordcredential?view=graph-rest-1.0&preserve-view=true) для [приложений](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true).

### <a name="mail"></a>Почта
Использование нового параметра **message** для обновления любых записываемых свойств [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) при [ответе](/graph/api/message-reply?view=graph-rest-1.0&preserve-view=true) на сообщение, например [для добавления получателя в ответ](/graph/api/message-reply#example?view=graph-rest-1.0&preserve-view=true).

### <a name="microsoft-graph-data-connect"></a>Подключение к данным Microsoft Graph
Разработчики и исследователи данных теперь могут использовать [инструменты для преобразования данных Office 365 в формат общей модели данных](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md). В этом случае обеспечивается согласование схемы данных с другими наборами данных, совместимыми с Open Data Initiative (ODI). 


### <a name="microsoft-graph-sdks"></a>Пакеты SDK Microsoft Graph
- Использование обработчиков хаоса в SDK JavaScript для проверки устойчивости приложения к сбоям серверов, возникающим в трудновоспроизводимых условиях.
- Прочтите о [создании вызовов API с помощью пакетов SDK](./sdks/create-requests.md).

### <a name="users"></a>Пользователи
- [Получение](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0&preserve-view=true) или [настройка](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0&preserve-view=true) параметров предпочитаемого пользователем формата даты и времени [для почтового ящика пользователя](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true). 
- Отслеживание даты и времени последнего изменения пароля [пользователя](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).

## <a name="october-2019-new-in-preview"></a>Октябрь 2019 г.: новые возможности в предварительной версии

### <a name="calendar"></a>Календарь
- Организаторы собраний могут [разрешить приглашенным предлагать другое время собраний](outlook-calendar-meeting-proposals.md). При получении ответа на приглашение, содержащего предложение другого времени, организатор может принять предложение и [обновить](/graph/api/event-update?view=graph-rest-beta&preserve-view=true) время собрания.
- Программное предоставление доступа к календарю с более тесным взаимодействием с использованием пользовательского интерфейса Outlook. Поддерживается отслеживание разрешений текущего пользователя и состояния общего доступа к календарю, а также следующие возможности:
  - Для каждого [календаря](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true) теперь можно управлять [разрешениями](/graph/api/resources/calendarpermission?view=graph-rest-beta&preserve-view=true) каждого пользователя, которому предоставлен доступ к календарю. 
  - Для каждого [почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) теперь можно указать, кто получает сообщения о собраниях и ответы на эти сообщения: делегат, владелец почтового ящика или и тот, и другой. 
- Дополнительная поддержка собраний по сети:
  - В каждом **календаре** можно указать разрешенных и используемых по умолчанию поставщиков собраний по сети.
  - Можно создать или обновить [мероприятие](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true), доступное по сети, и предоставить участникам сведения для присоединения к собранию по сети. 
  - В частности, можно использовать **onlineMeetingProvider** и **onlineMeeting** — это новые свойства **мероприятий**, с помощью которых можно задать или указать Microsoft Teams в качестве поставщика собраний по сети. Это временное решение [известной проблемы](known-issues.md#onlinemeetingurl-property-is-not-supported-for-microsoft-teams) со свойством **onlineMeetingUrl**.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [октябрь](changelog.md#october-2019)

### <a name="graph-explorer"></a>Песочница Graph
Попробуйте [следующую версию песочницы Graph](https://developer.microsoft.com/graph/graph-explorer/preview) и воспользуйтесь полезной контекстной информацией, включая разрешения, маркеры доступа и фрагменты кода SDK, на новых вкладках **Разрешения**, **Проверка подлинности** и **Фрагменты кода**. С помощью ползунка **просмотра** можно переключаться между [рабочей](https://developer.microsoft.com/graph/graph-explorer) и новой предварительной версией песочницы Graph.

### <a name="groups"></a>Группы
- Управление видимостью [групп](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) в определенных частях пользовательского интерфейса Outlook или в клиенте Outlook с помощью свойств **hideFromAddressLists** и **hideFromOutlookClients**.
- [Назначение](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) и удаление лицензий пользователям в [группе](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Идентификация и доступ
- Использование [политик условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) для настройки правил доступа для организации. Эти правила учитывают сигналы о пользователях или об удостоверениях устройств, включая членство пользователей или групп, расположение IP-адреса, а также поведение, включая попытки доступа к определенным приложениям и опасное поведение при входе.
- [Управление правами](/graph/api/resources/entitlementmanagement-overview?view=graph-rest-beta&preserve-view=true) можно использовать для управления доступом к группам, приложениям и сайтам SharePoint Online для пользователей внутри организации и вне ее.
- Добавление и удаление [учетных данных с паролем](/graph/api/resources/passwordcredential?view=graph-rest-beta&preserve-view=true) для [приложений](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) и [субъектов-служб](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Управление [ключами политики инфраструктуры доверия](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta&preserve-view=true) Azure AD B2C.
- Можно определить политики [пользовательского процесса](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true) Azure AD B2C для входа, регистрации, объединенной процедуры регистрации и входа, сброса пароля и обновления профиля.
- Настройка [меток защиты информации](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta&preserve-view=true), чтобы классифицировать конфиденциальность данных для пользователя или клиента.
- Существующие приложения, использующие API для [событий с риском для идентификации](/graph/api/resources/identityriskevent?view=graph-rest-beta&preserve-view=true), должны перейти на использование функций [обнаружения риска](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) в службе защиты идентификации Azure AD. Дополнительные сведения и график прекращения использования прежнего решения см. в [публикации в блоге](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/).


### <a name="mail"></a>Почта
[Вложение больших файлов размером до 150 МБ](outlook-large-attachments.md) в экземпляр [сообщения](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) путем создания [сеанса отправки](/graph/api/resources/uploadsession?view=graph-rest-beta&preserve-view=true) и итерационной отправки диапазонов файла, пока не отправятся все байты файла. 

### <a name="microsoft-graph-security-api"></a>Microsoft Graph Security API
- Предварительная версия интеграции с RSA NetWitness, ServiceNow и Splunk для сопоставления и синхронизации [оповещений](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#alerts), улучшения защиты от угроз и реагирования.
- Новые переключатели добавлены в [соединитель безопасности Microsoft Graph](/connectors/microsoftgraphsecurity/) и в [сборники схем](/azure/security-center/security-center-playbooks) для логических приложений и потоков. См. [примеры сборника схем](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Поддержка отправки [индикаторов угроз](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#threat-indicators-preview) в Microsoft Defender для конечной точки с целью блокирования или отправки оповещений об угрозах с использованием собственных источников аналитики. Интеграция с партнерами, такими как ThreatConnect, дает заказчикам возможность отправлять индикаторы непосредственно из решений аналитики угроз и автоматизации. 

### <a name="notifications"></a>Уведомления
- [Создание и отправка уведомлений](/graph/api/user-post-notifications?view=graph-rest-beta&preserve-view=true) всем клиентам приложения во всех конечных точках устройств, где пользователи могли войти в систему, без необходимости управлять разрешениями, делегированными пользователями.
- [Целевые конечные точки политики](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta&preserve-view=true) в [уведомлениях](/graph/api/resources/notification?view=graph-rest-beta&preserve-view=true) пользователей позволяют целенаправленно управлять уведомлениями на платформах Windows, iOS, Android или WebPush.
- Можно указать [политику отката](/graph/api/resources/fallbackpolicy?view=graph-rest-beta&preserve-view=true) для уведомлений для конечных точек iOS, чтобы отправлять высокоприоритетные необработанные уведомления, доставка которых на устройства другими способами может быть невозможной из-за ограничений, действующих для конкретной платформы, например, из-за использования режима экономии заряда аккумулятора.

 
### <a name="powershell-sdk"></a>Пакет SDK для PowerShell 
Разработчики и ИТ-специалисты могут обратить внимание на выпуск [пакета SDK Microsoft Graph для Powershell](https://github.com/microsoftgraph/msgraph-sdk-powershell). Этот пакет будет формировать модули, содержащие командлеты для создания запросов API REST Microsoft.

## <a name="september-2019-new-and-generally-available"></a>Сентябрь 2019 г.: новые и общедоступные возможности

### <a name="calendar-mail-and-group"></a>Календарь, почта и группа
[Получение необработанного содержимого файла или содержимого MIME элемента](/graph/api/attachment-get?view=graph-rest-1.0&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment), добавленного в качестве [вложения](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true) в [событие](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), [сообщение](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) или [запись](/graph/api/resources/post?view=graph-rest-1.0&preserve-view=true) группы.

### <a name="calendar-mail-outlook-task-personal-contact"></a>Календарь, почта, задача Outlook, личный контакт
Преобразование идентификатора элемента Outlook в поддерживаемые [форматы](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true#exchangeidformat-values), включая стандартный и неизменяемый формат идентификаторов Microsoft Graph, с помощью функции [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true). 

Преобразование формата идентификатора поддерживают следующие ресурсы:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true)
- [contact](/graph/api/resources/contact?view=graph-rest-1.0&preserve-view=true)
- [event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0&preserve-view=true)
- [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0&preserve-view=true)

### <a name="mail"></a>Почта
[Получение содержимого MIME сообщения](outlook-get-mime-message.md)

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
Использование [набора средств Microsoft Graph](toolkit/overview.md) с целью разработки приложений для рабочей среды, обеспечивающих согласованный внешний вид и функции Microsoft 365, и экономии времени при проверке подлинности и доступе к данным из Microsoft Graph.

## <a name="september-2019-new-in-preview"></a>Сентябрь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [сентябрь](changelog.md#september-2019)

### <a name="files"></a>Файлы
- Улучшенная поддержка синхронизации:

  - Определение операций, которые могут влиять на двоичное содержимое объекта [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true), с помощью нового свойства **pendingOperations**.
  - [Восстановление](/graph/api/driveitem-restore?view=graph-rest-beta&preserve-view=true) удаленного объекта **driveItem**. 
- Использование защищенного алгоритма хэширования (SHA-256) для улучшения безопасности и целостности данных ресурса [file](/graph/api/resources/file?view=graph-rest-beta&preserve-view=true).
- Получение или настройка ориентации ресурса [photo](/graph/api/resources/photo?view=graph-rest-beta&preserve-view=true). Настройка поддерживается в OneDrive персональный.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Использование нового свойства **identities** и получение удостоверений, которые может применять [пользователь](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) для входа в учетную запись. Удостоверения могут предоставляться организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт.
- Добавочные улучшения для [синхронизации удостоверений](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) в облачном приложении для клиента:

  - Сохранение параметров для [задания синхронизации](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta&preserve-view=true)
  - Указание причины применения [карантина](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta&preserve-view=true) для задания синхронизации

### <a name="teamwork"></a>Командная работа
Использование канала **Общий** в [команде](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) или настройка [параметров участников](/graph/api/resources/teammembersettings?view=graph-rest-beta&preserve-view=true), чтобы разрешить участникам команд создавать закрытые каналы в **команде**.

### <a name="users"></a>Пользователи
- Получение или обновление удостоверений, с помощью которых [пользователь](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) может войти в учетную запись. Эти удостоверения могут предоставляться бизнес-организациями или поставщиками удостоверений социальных сетей, такими как Facebook, Google и Майкрософт.
- Получение или обновление параметров предпочитаемого пользователем формата даты и времени [для почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true).


## <a name="august-2019-new-and-generally-available"></a>Август 2019 г.: новые и общедоступные возможности 

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0&preserve-view=true) касательно числа и размера удаленных элементов.
- Отслеживайте идентификаторы групп Microsoft 365 при [получении сведений о действиях групп](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0&preserve-view=true).
- Отслеживайте имя субъекта-владельца при получении [сведений об использовании хранилища OneDrive учетной записью](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0&preserve-view=true) и [сведений об использовании сайта SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0&preserve-view=true).
- Узнайте число активных и неактивных пользователей в Microsoft 365 при [получении отчета о количестве пользователей в отдельных службах Microsoft 365](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0&preserve-view=true).

### <a name="security"></a>Безопасность
- Используйте новую [надстройку Microsoft Graph Security API для Splunk](https://aka.ms/graphsecuritysplunkaddon), чтобы передавать оповещения системы безопасности и аналитику из различных продуктов партнеров в Splunk, облегчая сопоставление их данных по безопасности в режиме реального времени. См. [объявление](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972), чтобы получить дополнительные сведения. 
- [Ознакомьтесь со списком других решений и соединителей](security-integration.md), разработанных корпорацией Майкрософт или партнерами Майкрософт, которые подключаются к API безопасности и позволяют работать с данными в едином формате.


## <a name="august-2019-new-in-preview"></a>Август 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [август](changelog.md#august-2019)

### <a name="education"></a>Образование
- Свяжите [преподавателя](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true) или [задание](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) с [рубрикой оценивания](/graph/api/resources/educationrubric?view=graph-rest-beta&preserve-view=true), чтобы задать определенные показатели качества и уровни заданий. К примерам показателей качеств относятся орфография и грамматика, а к примерам уровней — "хорошо" и "неудовлетворительно". Кроме того, вы можете связать с рубрикой баллы и веса. Дополнительные сведения см. в [обзоре образовательных рубрик](education-rubric-overview.md).
- Оцените задание и представьте результаты в виде [отзыва](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta&preserve-view=true), [числовой оценки](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta&preserve-view=true) или [рубрики](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta&preserve-view=true).

### <a name="files"></a>Файлы
До этого момента вы могли [отслеживать](/graph/api/driveitem-follow?view=graph-rest-beta&preserve-view=true) объект [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) для удобного доступа или упрощения таких действий, как перемещение, копирование и сохранение в определенном формате. Теперь вы можете использовать действие [отмены отслеживания](/graph/api/driveitem-unfollow?view=graph-rest-beta&preserve-view=true), чтобы прекратить отслеживание таких элементов диска.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Поставщики управления доступом на основе ролей (RBAC) могут [управлять ролями](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) в Azure Active Directory, [определяя действия ролей](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true), которые могут выполняться с определенными ресурсами, и [назначая роли](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta&preserve-view=true) пользователям в соответствии с этими определениями, чтобы предоставить им доступ к этим ресурсам.
- Администраторы могут [просматривать обзоры доступа](/graph/api/accessreview-list?view=graph-rest-beta&preserve-view=true), чтобы эффективно проверять членство в группах, доступ к корпоративным приложениям и назначения ролей. Регулярные проверки доступа позволяют гарантировать, что только уполномоченные люди получают постоянный доступ к ресурсам определенными способами.

### <a name="social-and-workplace-intelligence"></a>Социальная и рабочая аналитика
Пользователи могли использовать приложение [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) Microsoft 365 для получения аналитических сведений о распределении рабочего времени, совместной работе и балансе между трудовой и личной жизнью. Теперь с помощью [API аналитики](/graph/api/resources/social-overview?view=graph-rest-beta&preserve-view=true#help-users-gain-insights-into-their-work-patterns) можно интегрировать данные о времени, потраченном на рабочие задачи (например, звонки, чаты и электронную почту), чтобы повысить продуктивность пользователя и улучшить его самочувствие. 


## <a name="july-2019-new-and-generally-available"></a>Июль 2019 г.: новые и общедоступные возможности 

### <a name="example-code-snippets"></a>Примеры фрагментов кода
Теперь имеются фрагменты кода Objective-C для всех статей по API в справочных материалах для версии 1.0 и бета-версии. См. пример Objective-C для [получения события](/graph/api/event-get?view=graph-rest-1.0&preserve-view=true&tabs=objective-c#example).

### <a name="group"></a>Группа
- Используйте функцию [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0&preserve-view=true), чтобы отображаемое имя или почтовый псевдоним существующей группы Microsoft 365 соответствовали политикам именования.
- Кроме того, перед созданием группы вы можете использовать функцию [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0&preserve-view=true) для объекта [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0&preserve-view=true), чтобы сначала проверить имена.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-1.0&preserve-view=true).
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#role-management-permissions) _RoleManagement.Read.Directory_ и _RoleManagement.ReadWrite.Directory_ для управления доступом на основе ролей (RBAC) в каталоге компании:

  - Используйте разрешение на чтение и запись, чтобы сначала [активировать](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0&preserve-view=true) роль каталога. 
  - Если роль активирована, вы можете использовать разрешение на чтение для [чтения ролей каталога](/graph/api/directoryrole-list?view=graph-rest-1.0&preserve-view=true), [перечисления участников ролей](/graph/api/directoryrole-list-members?view=graph-rest-1.0&preserve-view=true) и [перечисления шаблонов для ролей каталогов](/graph/api/directoryroletemplate-list?view=graph-rest-1.0&preserve-view=true). 
  - Вы также можете использовать разрешение на чтение и запись для [добавления](/graph/api/directoryrole-post-members?view=graph-rest-1.0&preserve-view=true) и [удаления](/graph/api/directoryrole-delete-member?view=graph-rest-1.0&preserve-view=true) участников ролей.


## <a name="july-2019-new-in-preview"></a>Июль 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="calendar"></a>Календарь 
Используйте новый [API мест](/graph/api/resources/place?view=graph-rest-beta&preserve-view=true), чтобы применять различные типы расположений, например [помещения](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) и [список помещений](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true), настроенные администраторами Exchange Online.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [июль](changelog.md#july-2019)

### <a name="files"></a>Файлы 
Применяйте дату и время окончания срока действия или пароль при [создании ссылки для общего доступа](/graph/api/driveitem-createlink?view=graph-rest-beta&preserve-view=true) к файлу, папке или другому объекту [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новое разрешение приложений](./permissions-reference.md#access-reviews-permissions) _AccessReview.ReadWrite.Membership_ для операций CRUD при [проверках доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true). 
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#administrative-units-permissions) _AdministrativeUnit.Read.All_ и _AdministrativeUnit.ReadWrite.All_ для чтения и записи (включая создание, обновление и удаление участников, а также управление ими) ресурсов [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true) соответственно.
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-beta&preserve-view=true).
- Используйте новую функцию [обнаружения](/graph/api/directorydefinition-discover?view=graph-rest-beta&preserve-view=true) для поиска последней [схемы синхронизации](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta&preserve-view=true) каталога, чтобы синхронизировать объекты каталога, атрибуты и их типы с приложением.
- Используйте [политику развертывания функций](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta&preserve-view=true), чтобы помочь администраторам клиента выполнить пилотное развертывание функций для определенных групп перед включением их для всей организации.

### <a name="mail"></a>Почта
Используйте более детализированное разрешение приложений _Mail.ReadBasic.All_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Теперь применимо к [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) и [отслеживанию изменений](delta-query-overview.md) для [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) и **mailFolder**.

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta&preserve-view=true) касательно числа и размера удаленных элементов.

### <a name="teamwork"></a>Командная работа
- [Устанавливайте](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [удаляйте](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [обновляйте](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta&preserve-view=true) и [перечисляйте установленные приложения Microsoft Teams](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta&preserve-view=true) для пользователя.
- Используйте доступ только для приложения, чтобы читать сообщения канала, а также отвечать на сообщения в каналах и беседах. [Запросите и получите утверждение](teams-protected-apis.md) для такого доступа.

## <a name="may---june-2019-new-and-generally-available"></a>Май–июнь 2019 г.: новые и общедоступные возможности

### <a name="calendar-mail-and-personal-contacts"></a>Календарь, почта и личные контакты
Администраторы Exchange могут предоставлять приложению разрешения приложения и [ограничить доступ приложения только к подмножеству почтовых ящиков](auth-limit-mailbox-access.md) вместо доступа ко всем почтовым ящикам в организации, используемого по умолчанию. Такое ограничение доступа будет применено ко всем разрешениям приложения, предоставленным приложению для [календарей](permissions-reference.md#calendars-permissions), [контактов](permissions-reference.md#contacts-permissions), а также [параметров почты и почтового ящика](permissions-reference.md#mail-permissions). См. связанное [объявление в блоге](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/).

### <a name="mail"></a>Почта
Используйте API [папок поиска почты](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0&preserve-view=true) для поиска сообщений и доступа к результатам поиска по электронной почте Outlook. См. соответствующее [объявление в блоге](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/).

### <a name="postman"></a>Postman
В качестве альтернативы песочнице Graph используйте API Microsoft Graph в [коллекции Postman Microsoft Graph](use-postman.md), чтобы изучить поведение API и ускорить разработку приложения.

### <a name="tutorials"></a>Учебники
Воспользуйтесь новым [руководством для создания консольного приложения Java](/graph/tutorials/java), чтобы получить информацию о календаре пользователя.

### <a name="user"></a>Пользователь
Администраторы и пользователи могут [отзывать](/graph/api/user-revokesigninsessions?view=graph-rest-1.0&preserve-view=true) все выданные маркеры обновления для пользователя. Обычно это используется для того, чтобы запретить доступ к данным организации для приложений на потерянных и украденных устройствах.


## <a name="may---june-2019-new-in-preview"></a>Май–июнь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [май](changelog.md#may-2019) 
- Обновления Intune за [июнь](changelog.md#june-2019)

### <a name="education"></a>Образование
- Разностный запрос для [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta&preserve-view=true).
- Разностный запрос и добавления свойств для [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) и [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true).

### <a name="group"></a>Группа
Получите [метки конфиденциальности](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true), чтобы обеспечить защиту конфиденциальных данных группы Microsoft 365 и выполнение политик в отношении соответствия требованиям. Эти метки являются объектами [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true), опубликованными администраторами в Центре безопасности и соответствия требованиям Microsoft 365, в рамках возможностей Microsoft Information Protection. 

### <a name="identity-and-access"></a>Удостоверения и доступ
- Получите экземпляр [приложения](/graph/api/resources/applicationtemplate?view=graph-rest-beta&preserve-view=true) или добавьте экземпляр из коллекции приложений Azure AD в ваш каталог в качестве шаблона.
- Получите журнал всех [событий подготовки](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta&preserve-view=true) каталога в клиенте.
- Получите сведения об [обнаруженном пользователе или рисках входа в систему](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) в среде Azure AD. Эта функциональность обнаружения рисков является частью Azure AD Identity Protection (Защиты идентификации Azure AD).

### <a name="mail"></a>Почта
Используйте более детализированное делегированное разрешение _Mail.ReadBasic_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Доступно для чтения методов [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) и [отслеживанию изменений](delta-query-overview.md) для [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) и **mailFolder**.

### <a name="microsoft-graph-toolkit"></a>Набор средств Microsoft Graph
[Набор средств Microsoft Graph](./toolkit/overview.md) — это набор не зависящих от платформы веб-компонентов и помощников, обеспечивающий удобную проверку подлинности и доступ к данным в Microsoft Graph.  Так как набор средств Microsoft Graph находится в состоянии предварительной версии, используйте компоненты и поставщиков наборов средств только для тех приложений, которые не предназначены для рабочей среды.

### <a name="reports"></a>Отчеты
- Получайте [отчеты о методах проверки подлинности](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta&preserve-view=true), используемых пользователями в организации, таких как самостоятельное хранение пароля и многофакторная проверка подлинности (MFA).

### <a name="sites"></a>Сайты
Предоставляйте пользователям возможность [отслеживать](/graph/api/site-follow?view=graph-rest-beta&preserve-view=true) или [прекращать отслеживание](/graph/api/site-unfollow?view=graph-rest-beta&preserve-view=true) сайтов SharePoint. 

### <a name="teamwork"></a>Командная работа
- Размещайте [изображения](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta&preserve-view=true) в [сообщениях в чатах](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) Microsoft Teams.
- Поддерживайте [настройку](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta&preserve-view=true) способа обнаружения закрытой команды.


## <a name="january---april-2019-new-and-generally-available"></a>Январь–апрель 2019 г.: новые и общедоступные возможности

[Подключение к данным Microsoft Graph](data-connect-concept-overview.md)

### <a name="calendar"></a>Календарь
[Получение сведений о доступности](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>Удостоверения и доступ
[Поставщики удостоверений](/graph/api/resources/identityprovider?view=graph-rest-1.0&preserve-view=true)
[Руководство по улучшенной проверке подлинности](./auth/index.yml)
[Миграция приложений из Azure AD Graph в Microsoft Graph](migrate-azure-ad-graph-planning-checklist.md)

### <a name="sdks"></a>Пакеты SDK
[Руководство по пакетам SDK](/sdks/sdks-overview.md) Фрагменты API ([пример](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true&tabs=cs#sdk-sample-code))

### <a name="security"></a>Система безопасности
[Оценка безопасности клиента](/graph/api/resources/securescore?view=graph-rest-1.0&preserve-view=true)

## <a name="january---april-2019-new-in-preview"></a>Январь–апрель 2019 г.: новые возможности в предварительной версии

### <a name="calendar-group-mail-to-do-tasks"></a>Календарь, группа, почта, задачи To-Do
[Получение необработанного контента или содержимого MIME вложений](/graph/api/attachment-get?view=graph-rest-beta&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment) для события, сообщения, задачи Outlook или записи в группе

### <a name="change-notifications"></a>Уведомления об изменениях
[Уменьшение количества пропущенных уведомлений об изменениях](webhooks-lifecycle.md)

### <a name="devices-and-apps"></a>Устройства и приложения
- Обновления Intune за [январь](changelog.md#january-2019) 
- Обновления Intune за [февраль](changelog.md#february-2019)
- Обновления Intune за [март](changelog.md#march-2019)
- Обновления Intune за [апрель](changelog.md#april-2019)

### <a name="files"></a>Файлы
[Приглашение к совместному использованию](/graph/api/driveitem-invite?view=graph-rest-beta&preserve-view=true) включает истечение срока его действия и пароль

### <a name="financials"></a>Финансовые показатели
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>Удостоверения и доступ
[Проверки доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) поддерживают разрешения для приложений [Журналы аудита и входа](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta&preserve-view=true)
[Настраиваемые вход и регистрация в Azure AD B2C](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta&preserve-view=true)
[Рискованный пользователь](/graph/api/resources/riskyuser?view=graph-rest-beta&preserve-view=true) и [журнал](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta&preserve-view=true)

### <a name="mail"></a>Почта
[Получение содержимого MIME сообщений](outlook-get-mime-message.md)

### <a name="reports"></a>Отчеты
[Отчеты о входе в приложение](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta&preserve-view=true)

### <a name="security"></a>Система безопасности
[Действия по обеспечению безопасности](/graph/api/resources/securityaction?view=graph-rest-beta&preserve-view=true)
[Индикаторы угроз](/graph/api/resources/tiindicator?view=graph-rest-beta&preserve-view=true)

### <a name="teamwork"></a>Командная работа
[Личные чаты](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)
[Управление сменами](/graph/api/resources/shift?view=graph-rest-beta&preserve-view=true)

## <a name="see-also"></a>См. также
- Ознакомьтесь [с текущими новыми возможностями](whats-new-overview.md) в Microsoft Graph.
- Периодически просматривайте [блог разработчика, посвященный Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
