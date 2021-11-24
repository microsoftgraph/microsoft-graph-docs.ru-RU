---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 37f80e951ea71d5847e0c793053c3a1bc9cd42dc
ms.sourcegitcommit: c6bbba6cb9aaa7ad35374d1b5d4466c49878ab43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/22/2021
ms.locfileid: "61135174"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.


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
- Только участники из одной компании.

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
