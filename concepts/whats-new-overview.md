---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 156f15534b102d5a3e17acd7b04c32e30f34a3f7
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61803506"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.


## <a name="december-2021-new-and-generally-available"></a>Декабрь 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--presence"></a>Облачные коммуникации | Присутствие
[Подпишитесь на уведомления об изменениях](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&preserve-view=true) в состоянии [присутствия](/graph/api/resources/presence) указанного пользователя. Всегда указывайте сертификат шифрования в запросе подписки, так как это [подробные уведомления, которые включают зашифрованные данные ресурсов](webhooks-with-resource-data.md).


### <a name="compliance--subject-rights-requests"></a>Соответствие требованиям | Запросы прав субъектов
Средства [управления конфиденциальностью в Microsoft 365](/privacy/solutions/privacymanagement/privacy-management?view=o365-worldwide&preserve-view=true) включают [API запросов прав субъектов](/graph/api/resources/subjectrightsrequest), начиная с версии 1 и с бета-версий конечных точек Microsoft Graph. С помощью этого API пользователи могут создавать запросы, чтобы просматривать свои личные сведения или управлять ими в своих организациях. Этот API также дает возможность автоматизировать управление такими запросами и масштабировать его, что помогает эффективнее выполнять отраслевые регламенты.

### <a name="customer-booking"></a>Резервирование для пользователей
Используйте этот API для Microsoft Bookings в рабочих приложениях, воспользуйтесь следующими новыми функциями и обновлениями:
- Уведомите ваших клиентов в США или в Канаде о [встрече](/graph/api/resources/bookingappointment) или какой-либо определенной [службе](/graph/api/resources/bookingservice), связанной со встречей, с помощью SMS-сообщений.
- Включите собрание по сети для службы и автоматически сформируйте ссылку на собрание Microsoft Teams для встречи.
- Разрешение одного или нескольких клиентов на групповой встрече, установка максимального количества участников для службы и для встречи, отслеживание фактического количества участников встречи.
- Создание [настраиваемого вопроса](/graph/api/resources/bookingcustomquestion) для [бизнеса](/graph/api/resources/bookingbusiness), сопоставление вопроса с параметром, чтобы указать его в качестве обязательного для службы, отслеживание вопросов и ответов на встрече.
- Получение или установка часового пояса для клиента на встрече или для [сотрудника](/graph/api/resources/bookingstaffmember).
- Получение или установка расположения и номера телефона для [клиента](/graph/api/resources/bookingcustomer).
- Доступ к API версии 1 из новой конечной точки `https://graph.microsoft.com/v1.0/solutions/`. Обратите внимание, что API бета-версии остается в конечной точке `https://graph.microsoft.com/beta`.

### <a name="education"></a>Образование
- Укажите [задание](/graph/api/resources/educationassignment) для добавления только календари в учащихся с помощью свойств **addToCalendarAction**.
- [Повторное назначение](/graph/api/educationsubmission-reassign) [отправленного задания](/graph/api/resources/educationsubmission) учащемуся с отзывом для проверки.
- [Вывод списка заданий](/graph/api/educationuser-list-assignments) для [educationUser](/graph/api/resources/educationuser). 

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
[Обновление](/graph/api/accessreviewinstance-update) проверяющих и откат проверяющих для [экземпляра проверки доступа](/graph/api/resources/accessreviewinstance).

### <a name="teamwork"></a>Teamwork
- Определение [чата](/graph/api/resources/chat) в Microsoft Teams по его URL-адресу (с помощью свойства **webUrl**).
- Получайте сведения о событиях, происходящих в чате, канале или команде, путем доступа к ресурсу [eventMessageDetail](/graph/api/resources/EventMessageDetail) из [chatMessage](/graph/api/resources/chatmessage) или [чата](/graph/api/resources/chat). Например, о таких событиях, как добавление участников в канал или чат, или изменение описания команды.

## <a name="december-2021-new-in-preview-only"></a>Декабрь 2021 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meetings"></a>Облачные коммуникации | Собрания по сети
Включите регистрацию на [собрание по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) с помощью системы [внешней регистрации](/graph/api/resources/externalmeetingregistration?view=graph-rest-beta&preserve-view=true). 

### <a name="cloud-communications--presence"></a>Облачные коммуникации | Присутствие
- Используйте действие [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true), чтобы задать предпочтительное состояние доступности и активности для пользователя. Присутствие пользователя становится предпочтительным.
- Используйте действие [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true), чтобы очистить предпочтительное состояние доступности и активности для пользователя.
- Используйте `Presence.ReadWrite` в качестве делегированного разрешения с действиями [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) или [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).
- Используйте `Presence.ReadWrite.All` в качестве разрешения приложения с действиями [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) или [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- Администраторы могут включить [Microsoft Managed Desktop](/graph/api/resources/microsoftmanageddesktop?view=graph-rest-beta&preserve-view=true), указав параметры в [политике подготовки облачных компьютеров](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) и настроив функцию управляемых устройств для облачных компьютеров.
- [Перезагрузка](/graph/api/cloudpc-reboot?view=graph-rest-beta&preserve-view=true) [облачного компьютера](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true).
- [Переименование](/graph/api/cloudpc-rename?view=graph-rest-beta&preserve-view=true) для обновления отображаемого имени облачного компьютера.
- [Устранение неполадок](/graph/api/cloudpc-troubleshoot?view=graph-rest-beta&preserve-view=true) для проверки состояния работоспособности облачного компьютера и узла сеанса.
- Отслеживание результата последнего удаленного действия на облачном компьютере, включая перезагрузку, переименование, повторную подготовку и устранение неполадок, с помощью свойства **lastRemoteActionResult**.
- Отслеживать метки времени последнего входа на облачный компьютер с помощью свойства **lastLoginResult**.
- Отслеживание даты недоступности [образа устройства облачного компьютера](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) с помощью свойства **expirationDate**.
- Отслеживание состояния операционной системы в [образе устройства облачного компьютера](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) с помощью свойства **osStatus**.
- [Создание](/graph/api/rbacapplication-post-roledefinitions?view=graph-rest-beta&preserve-view=true), [обновление](/graph/api/unifiedroledefinition-update?view=graph-rest-beta&preserve-view=true) и [удаление](/graph/api/unifiedroledefinition-delete?view=graph-rest-beta&preserve-view=true) объекта [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) для поставщика RBAC облачного компьютера.

### <a name="education"></a>Образование
- [Отслеживание изменений](delta-query-overview.md) ресурсов[educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) и [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true).
- Укажите [задание](/graph/api/resources/educationassignment) для добавления только календари в учащихся с помощью свойств **addToCalendarAction**.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- [Получите](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) сведения о сертификате [приложения](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) с помощью свойства **certification**. Свойство задается только в том случае, если приложение сертифицировано по [программе Соответствия требованиям приложений Microsoft 365](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).  
- [Включите](/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-beta&preserve-view=true) или [исключите](/graph/api/permissiongrantpolicy-post-excludes?view=graph-rest-beta&preserve-view=true) сертификацию как [условие](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true) в [политике предоставления разрешений](/graph/api/resources/permissiongrantpolicy?view=graph-rest-beta&preserve-view=true) посредством свойства **certifiedClientApplicationsOnly** в [permissionGrantConditionSet](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true).

### <a name="search--index"></a>Поиск | Индекс
Используйте операцию [обновления](/graph/api/externalconnectors-schema-update?view=graph-rest-beta&preserve-view=true) для обновления свойств элементов схемы [подключения](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true), включая их псевдонимы и метки.

### <a name="teamwork"></a>Teamwork
- [Перечисление](/graph/api/teams-list?view=graph-rest-beta&preserve-view=true) всех команд в организации.

### <a name="to-do-tasks"></a>Задачи To-Do
- Чтобы предусмотреть возможность централизованного управления всеми задачами, поступающими из разных источников (сообщения Outlook, чаты Teams, документы OneDrive и т. д.):
  - Используйте [последнюю версию программного интерфейса To Do](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true) и обращайтесь к нему из новой конечной точки `https://graph.microsoft.com/beta/me/tasks/`.
  - Используйте сегмент `allTasks`, чтобы получить все задачи для пользователя: `https://graph.microsoft.com/beta/me/tasks/alltasks`.
  - Следует различать встроенные списки задач (например, **Помеченные сообщения электронной почты** или **Задачи**) и пользовательские списки задач. Встроенный список задач представлен ресурсом [wellKnownTaskList](/graph/api/resources/wellknowntasklist?view=graph-rest-beta&preserve-view=true), а пользовательский список задач — ресурсом [taskList](/graph/api/resources/tasklist?view=graph-rest-beta&preserve-view=true).
  - Следует различать определенный в настоящее время типа задач [task](/graph/api/resources/task?view=graph-rest-beta&preserve-view=true) и базовый тип [baseTask](/graph/api/resources/basetask?view=graph-rest-beta&preserve-view=true).
- Более сложную [задачу](/graph/api/resources/task?view=graph-rest-beta&preserve-view=true) можно разделить на более удобные для обработки подзадачи меньшего размера. Каждая подзадача представлена ресурсом [checklistItem](/graph/api/resources/checklistitem?view=graph-rest-beta&preserve-view=true).
- [Перемещение](/graph/api/basetask-move?view=graph-rest-beta&preserve-view=true) задачи между списками.
- В [этой публикации в блоге](https://devblogs.microsoft.com/microsoft365dev/announcing-the-public-preview-of-to-do-tasks-api/) содержатся дополнительные сведения и инструкции по переносу существующих приложений, использующих [более раннюю версию API To Do](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true), на [последнюю версию API To Do](/graph/api/resources/tasks-overview?view=graph-rest-beta&preserve-view=true).


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
