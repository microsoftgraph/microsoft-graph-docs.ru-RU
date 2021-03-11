---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: d8478b405804da10e7bad3de647b45751f14ae86
ms.sourcegitcommit: 59df7b4d5098a49403a315d19a0c048013cd592e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50723102"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="march-2021-new-and-generally-available"></a>Март 2021 г.: новые и общедоступные возможности

### <a name="applications"></a>Приложения
Общая доступность ресурса [applicationTemplate](/graph/api/resources/applicationtemplate), поддерживающего [перечисление](/graph/api/applicationtemplate-list) приложений в коллекции приложений Azure AD и [добавление](/graph/api/applicationtemplate-instantiate) экземпляра такого приложения в каталог.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
Общая доступность [API облачной печати](universal-print-concept-overview.md) для универсальной печати! Ознакомьтесь с [объявлением](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/universal-print-is-ready-for-business/ba-p/2176778) и узнайте, как [начать работу с универсальной печатью](https://docs.microsoft.com/universal-print/fundamentals/universal-print-license).

### <a name="teamwork"></a>Командная работа
- Общая доступность дополнительных свойств объекта [teamsAppDefinition](/graph/api/resources/teamsAppDefinition), представляющих сведения о версии приложения в каталоге приложения Microsoft Teams, включая следующие:
  - **createdBy**, **description**, **shortDescription**, **lastModifiedDateTime**
  - свойство **publishingState**, которое может находиться в состоянии `submitted` и проверяться, `published` или `rejected` администратором
  - связь **bot** типа [teamworkBot](/graph/api/resources/teamworkbot), представляющая сведения о боте, указанные в манифесте приложения Teams.
- [Перечисление](/graph/api/chatmessage-list-chatmessagehostedcontents) или [получение](/graph/api/chatmessagehostedcontent-get) форматированного контента, размещенного в [chatMessage](/graph/api/resources/chatmessage), например изображений или фрагментов кода.

## <a name="march-2021-new-in-preview-only"></a>Март 2021 г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
Получение даты и времени (свойство **lastSeenDateTime**), когда принтер в последний раз взаимодействовал с универсальной печатью.

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

### <a name="users"></a>Пользователи
[Получение](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) или [обновление](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) пользовательских [настроек для перевода языков](/graph/api/resources/translationpreferences?view=graph-rest-beta&preserve-view=true). Например, следует ли переводить, переводить автоматически или отображать запрос перед переводом определенных языков в сообщениях, чатах и на веб-страницах, а также любые [переопределения перевода](/graph/api/resources/translationlanguageoverride?view=graph-rest-beta&preserve-view=true).

## <a name="february-2021-new-and-generally-available"></a>Февраль 2021 г.: новые и общедоступные возможности

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Собрание по сети
Использование разрешений приложений `OnlineMeetings.Read.All` или `OnlineMeetings.ReadWrite.All`, основанных на политике, для операций и методов ресурса [onlineMeeting](/graph/api/resources/onlinemeeting). Администраторы могут [настроить политику доступа приложения](cloud-communication-online-meeting-application-access-policy.md), чтобы разрешить приложениям доступ к собраниям по сети от имени пользователя.

### <a name="sites-and-lists"></a>Сайты и списки
Использование ресурса [permission](/graph/api/resources/permission) и его операций CRUD для управления разрешением общего доступа, предоставленным для [driveItem](/graph/api/resources/driveitem). Разрешения с аспектом link представляют ссылки для совместного доступа, созданные в элементе. Разрешения с аспектом invitation представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.

## <a name="february-2021-new-in-preview-only"></a>Февраль 2021 г.: новые возможности только в предварительной версии

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
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](https://developer.microsoft.com/graph/changelog/).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
