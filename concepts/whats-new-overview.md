---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 7d1fa2979084ac901c26b1f4e5da5994b9c39874
ms.sourcegitcommit: f26428bce3034e206b901e9c747cffcf64b55882
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47651309"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](changelog.md). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="september-2020-new-and-generally-available"></a>Сентябрь 2020г.: новые и общедоступные возможности

### <a name="reports"></a>Отчеты
[Получите отчет, включающий количество уникальных пользователей](/graph/api/reportroot-getemailappusageversionsusercounts) для Outlook 2019 и Outlook в Microsoft 365.

### <a name="users"></a>Пользователи
Помимо получения SMTP-адреса [пользователя](/graph/api/resources/user) с помощью свойства **mail**, теперь вы можете установить это свойство и обновить адрес электронной почты пользователя. 

## <a name="september-2020-new-in-preview-only"></a>Сентябрь 2020г.: новые возможности только в предварительной версии

### <a name="cloud-communications"></a>Коммуникации из облака
- Не рекомендуется использовать свойства**autoAdmittedUsers** из[onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta). Вместо этого следует использовать новое свойство **lobbyBypassSettings** и его [значения](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta#lobbybypassscope-values).
- Используйте дополнительные параметры, связанные для объявления звонящим о присоединении или выходе из собрания по сети (свойство **isEntryExitAnnounced**), и разрешения конкретных выступающих доступа к собранию (свойство **allowedPresenters**).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- [Получите документы для каждого задания печати, связанного с принтером](/graph/api/printer-list-jobs?view=graph-rest-beta), применив `$expand` [параметр запроса системы OData](/graph/api/printer-list-jobs?view=graph-rest-beta#optional-query-parameters). 
- Отфильтруйте задания печати по пользователю, который их создал, применив `$filter` [параметр системного запроса OData](/graph/api/printer-list-jobs?view=graph-rest-beta#optional-query-parameters).

### <a name="identity-and-access"></a>Удостоверение и доступ
Вы можете включить [расписание](/graph/api/resources/requestschedule?view=graph-rest-beta) при запросе или удалении [назначения пользователя на пакет доступа](/graph/api/resources/accesspackageassignment?view=graph-rest-beta), который определяет доступ к группам, приложениям или сайтам SharePoint.

### <a name="teamwork"></a>Командная работа
Узнайте о дате и времени создания [канала](/graph/api/resources/channel?view=graph-rest-beta) или [команды](/graph/api/resources/team?view=graph-rest-beta) Teams.

## <a name="august-2020-new-and-generally-available"></a>Август 2020 г.: новые и общедоступные возможности

### <a name="change-notifications"></a>Уведомления об изменениях
[Отслеживание изменений](delta-query-overview.md) поддерживаемых ресурсов в национальном облаке Microsoft Graph для государственных организаций США.

### <a name="cloud-communications"></a>Коммуникации из облака
- [Отмените](/graph/api/call-cancelmediaprocessing) любые действия интерактивного голосового ответа (IVR), выполняемые или находящиеся в очереди, которые [воспроизводят звуковой сигнал](/graph/api/call-playprompt) или [записывают ответ](/graph/api/call-record).
- Получите [сведения о расшифровке звонка](/graph/api/resources/calltranscriptioninfo) с помощью свойства **transcription**.

### <a name="teamwork"></a>Командная работа
- Используйте альтернативный способ [создания группы](/graph/api/team-post) без предварительного создания группы.
- Используйте свойство навигации **участники**, чтобы добавить участников в команду с большей надежностью и меньшей задержкой.
- Узнайте, в каком состоянии находится публикация [приложения](/graph/api/resources/teamsapp) Microsoft Teams с помощью свойства **publishingState** [определения приложения](/graph/api/resources/teamsappdefinition). Возможные значения состояния публикации: `submitted`, `published` и `rejected`. См. [пример](/graph/api/teamsapp-list?view=graph-rest-1.0&tabs=http#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state).
- Воспользуйтесь делегированным разрешением `AppCatalog.Submit`, чтобы позволить пользователю [отправить приложение](/graph/api/teamsapp-publish) и оформить запрос на его проверку администратором. С помощью этого же разрешения пользователь может [отменить](/graph/api/teamsapp-delete) отправленное ранее приложение, которое не было опубликовано. 


## <a name="august-2020-new-in-preview-only"></a>Август 2020 г.: новые возможности только в предварительной версии

### <a name="applications"></a>Приложения
Поддержка единого входа на основе паролей в ресурсах приложения [субъекта-службы](/graph/api/resources/serviceprincipal?view=graph-rest-beta) и указание таких [параметров](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta) в свойстве **passwordSingleSignOnSettings**. Сведения о едином входе на основе паролей в Azure AD см. в статье [Настройка единого входа на основе пароля](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).

### <a name="calendar"></a>Календарь
Улучшенная программная поддержка сценариев, в которых используется повторяющееся [событие](/graph/api/resources/event?view=graph-rest-beta):
- надежный поиск экземпляра события в повторяющемся ряду, в том числе измененного или отмененного, с помощью свойства **occurrenceId**;
- поиск любых исключений в ряду повторяющихся экземпляров события с помощью свойства **exceptionOccurrences**;
- поиск любых отмен в ряду повторяющихся экземпляров события с помощью свойства **cancelledOccurrences**.

### <a name="change-notifications"></a>Уведомления об изменениях
- Используйте свойство **includeResourceData** ресурса [subscription](/graph/api/resources/subscription?view=graph-rest-beta) для [настройки уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md). Не используйте свойство **includeProperties**.
- Получение [уведомлений об изменениях, доставляемых через концентратор событий](change-notifications-delivery.md).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Предоставление всем пользователям и группам возможности [совместного использования принтера](/graph/api/resources/printershare?view=graph-rest-beta) с помощью свойства **allowAllUser**.
- С помощью новых делегированных разрешений и разрешений для приложений можно пользоваться и управлять [печатью документа](/graph/api/resources/printDocument?view=graph-rest-beta), [заданием на печать](/graph/api/resources/printjob?view=graph-rest-beta), [принтером](/graph/api/resources/printer?view=graph-rest-beta), [предоставлением общего доступа к принтеру](/graph/api/resources/printershare?view=graph-rest-beta) и [определением операции печати](/graph/api/resources/printtaskdefinition?view=graph-rest-beta). Дополнительные сведения см. в статье об обновлениях в сфере облачной печати [за август](changelog.md#august-2020).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune в бета-версии за [август](changelog.md#august-2020).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Настройка [условий соглашения об использовании](/graph/api/resources/agreement?view=graph-rest-beta) для поддержки срока действия и периодичности соглашения с обязательным принятием пользователем соглашения на отдельных устройствах или повторным принятием соглашения с установленной периодичностью. 
- Используйте свойство **file** для перехода к [настраиваемому соглашению](/graph/api/resources/agreementfile?view=graph-rest-beta) условий. Не используйте свойство **files**.
- Добавление, удаление и перечисление внутренних или внешних кураторов, которые могут утверждать запросы от [подключенной организации](/graph/api/resources/connectedorganization?view=graph-rest-beta) на доступ к группе, приложению или сайту SharePoint Online. Дополнительные сведения см. в статье [Управление правами](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
- Разрешите дальнейшую настройку [политики авторизации](/graph/api/resources/authorizationpolicy?view=graph-rest-beta) для клиента, например разрешите [роли пользователя по умолчанию](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta) создавать приложения или группы безопасности или читать других пользователей, разрешите пользователям возможность подписываться на подписки через электронную почту или присоединяться к клиенту через проверку электронной почты, а также предоставьте пользователям возможность самостоятельного сброса пароля.
- Управляйте [предопределенными, настраиваемыми политиками как пользовательскими потоками в клиенте Azure Active Directory B2C](/graph/api/resources/b2cuserflows?view=graph-rest-beta). См. Дополнительные сведения о [пользовательских потоках B2C](/azure/active-directory-b2c/user-flow-overview).
- Включите [возможность самостоятельной регистрации в качестве пользовательских потоков B2X в клиенте Azure Active Directory](/graph/api/resources/b2xuserflows?view=graph-rest-beta). См. Дополнительные сведения о [самостоятельной регистрации](/azure/active-directory/external-identities/self-service-sign-up-overview).

### <a name="people-and-workplace-intelligence--profile"></a>Люди и рабочая аналитика | Профиль
Добавление следующих дополнительных свойств пользовательского [профиля](/graph/api/resources/profile?view=graph-rest-beta) и управление ими. Их можно отображать в общих для пользователей интерфейсах в Microsoft 365 и сторонних приложениях:
- [addresses](/graph/api/resources/itemAddress?view=graph-rest-beta)
- [anniversaries](/graph/api/resources/personAnniversary?view=graph-rest-beta)
- [awards](/graph/api/resources/personAward?view=graph-rest-beta)
- [certifications](/graph/api/resources/personCertification?view=graph-rest-beta)
- [notes](/graph/api/resources/personAnnotation?view=graph-rest-beta)
- [patents](/graph/api/resources/itemPatent?view=graph-rest-beta)
- [publications](/graph/api/resources/itemPublication?view=graph-rest-beta)


### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Получение [отчетов об использовании приложений Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta), в частности сведений о пользователе, количества пользователей и количества используемых платформ.

### <a name="teamwork"></a>Командная работа
Получение [контента, размещенного в сообщении чата](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta), например изображений или фрагментов кода. См. [пример](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&branch=master#example-2-get-hosted-content-bytes-for-an-image), чтобы получить количество байтов содержимого для изображения.

### <a name="to-do-tasks"></a>Задачи To-Do
- Появление нового набора API для [Microsoft To Do](todo-concept-overview.md), позволяющего пользователям приложения упорядочивать и отслеживать личные задачи в клиентских приложениях Microsoft 365. Дополнительные сведения см. в статье [Использование API Microsoft To Do](/graph/api/resources/todo-overview?view=graph-rest-beta).
- Прекращение поддержки [API задач Outlook](/graph/api/resources/outlooktask?view=graph-rest-beta).


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

