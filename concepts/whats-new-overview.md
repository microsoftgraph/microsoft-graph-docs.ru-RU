---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 79d281a04cf4ae1dc683efa93da394e59bdc9149
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333836"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.


## <a name="february-2022-new-and-generally-available"></a>Февраль 2022 г.: новые и общедоступные возможности

### <a name="teamwork"></a>Teamwork
Получение [сведений о виртуальном собрании](/graph/api/resources/teamworkOnlineMeetingInfo), связанном с [чатом](/graph/api/resources/chat), с помощью свойства **onlineMeetingInfo**.

## <a name="february-2022-new-in-preview-only"></a>Февраль 2022 г.: новое только в предварительной версии

### <a name="change-notifications"></a>Уведомления об изменениях
Подписка на изменения контактов, событий или сообщений Outlook для получения уведомлений, в полезные данные которых включены данные ресурсов. Дополнительные сведения см. в статье [Уведомления об изменениях, связанных с ресурсами Outlook, в Microsoft Graph](outlook-change-notifications-overview.md).

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Использование прав доступа приложений для `CustomSecAttributeAssignment.Read.All` чтения [пользовательских определений атрибутов безопасности](/graph/api/resources/customsecurityattributedefinition?view=graph-rest-beta&preserve-view=true) для организации без пользователя, выполнившего вход.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Настройка [параметров](/graph/api/resources/accessreviewstagesettings?view=graph-rest-beta&preserve-view=true) каждого [этапа](/graph/api/resources/accessreviewstage?view=graph-rest-beta&preserve-view=true) в многоступенчатой проверке доступа. Помимо [получения](/graph/api/accessreviewstage-get?view=graph-rest-beta&preserve-view=true) или [обновления](/graph/api/accessreviewstage-update?view=graph-rest-beta&preserve-view=true) этапа проверки доступа, вам доступны следующие действия: 
  - [Остановка](/graph/api/accessreviewstage-stop?view=graph-rest-beta&preserve-view=true) предоставления проверяющими дополнительной информации на некотором этапе и переход к следующему этапу (если применимо). 
  - [Фильтрация](/graph/api/accessreviewstage-filterbycurrentuser?view=graph-rest-beta&preserve-view=true) и получение всех этапов [экземпляра проверки доступа](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true), для которого вызывающий пользователь является проверяющим
  - [Составление списка решений](/graph/api/accessreviewstage-list-decisions?view=graph-rest-beta&preserve-view=true) из многоступенчатой проверки доступа.
- Приложения могут использовать разрешение приложения `EntitlementManagement.ReadWrite.All` в целях [создания запроса пакета доступа для ресурса](/graph/api/entitlementmanagement-post-accesspackageresourcerequests?view=graph-rest-beta&preserve-view=true), чтобы добавить ресурс в [каталог пакетов доступа](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true) или удалить его из каталога.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход
- Использование ряда новых свойств для настройки [фирменного стиля организации](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). Например, варианта логотипа компании в виде баннера для страницы входа, настраиваемой пиктограммы сайта с URL-адресом на основе CDN, а также нескольких других настраиваемых свойств, которые пользователи могут применять для управления учетными записями.
- Включение или исключение Linux как одного из [условий платформы](/graph/api/resources/conditionalaccessplatforms?view=graph-rest-beta&preserve-view=true) в [политике условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Выявление [субъектов-служб, с которыми связан риск](/graph/api/resources/riskyserviceprincipal?view=graph-rest-beta&preserve-view=true), в организации с помощью службы Azure AD, которая постоянно [определяет и оценивает риски](/graph/api/resources/serviceprincipalriskdetection?view=graph-rest-beta&preserve-view=true) на основе различных сигналов и машинного обучения. Вы можете [подтвердить](/graph/api/riskyserviceprincipal-confirmcompromised?view=graph-rest-beta&preserve-view=true), что субъект-служба действительно скомпрометирован, после чего корпорация Майкрософт отключит объект этого субъекта-службы. Вы можете [отклонить](/graph/api/riskyserviceprincipal-dismiss?view=graph-rest-beta&preserve-view=true) риск, связанный с субъектом-службой. Кроме того, вы можете [создать журнал рисков](/graph/api/riskyserviceprincipal-list-history?view=graph-rest-beta&preserve-view=true), связанных с субъектом-службой.
- Использование [параметров межклиентского доступа](/graph/api/resources/crosstenantaccesspolicy-overview?view=graph-rest-beta&preserve-view=true) для контроля над взаимодействием между пользователями в вашей и других организациях и управления этим взаимодействием. Эти параметры детализированы и позволяют определять пользователей, группы и приложения как в вашей, так и во внешних организациях, которые могут участвовать во взаимодействии в рамках Azure AD B2B и прямом подключении Azure AD B2B. 
- Разрешение или запрещение пользователям и группам в организации применять [встроенную в Azure AD проверку подлинности на основе сертификатов (CBA)](/graph/api/resources/x509CertificateAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true).

## <a name="january-2022-new-and-generally-available"></a>Январь 2022 г.: новые и общедоступные возможности

### <a name="devices-and-apps--service-health-and-communications"></a>Устройства и приложения | Работоспособность и взаимодействие служб
Получите [вложение с уведомлением о службе](/graph/api/resources/serviceAnnouncementAttachment), добавленное в [сообщение об обновлении службы](/graph/api/resources/serviceupdatemessage).

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Получите коллекцию ресурсов [проверки доступа и проверяющих](/graph/api/resources/accessreviewreviewer), где определены проверяющие, с которыми будет установлена связь для [экземпляра проверки доступа](/graph/api/resources/accessReviewInstance).
- Дифференцируйте 3 типа ресурсов, доступ к которым представлен через [решение о проверке доступа](/graph/api/resources/accessreviewinstancedecisionitem):
  - [Политика назначения пакета для доступа](/graph/api/resources/accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource), для которой доступ определяется решением о проверке доступа.
  - [Роль ресурса Azure](/graph/api/resources/accessReviewInstanceDecisionItemAzureRoleResource), для которой доступ определяется решением о проверке доступа.
  - [Субъект-служба](/graph/api/resources/accessReviewInstanceDecisionItemServicePrincipalResource), для которой доступ к ресурсу определяется решением о проверке доступа.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход
Примените [элемент управления сеансом](/graph/api/resources/conditionalAccessSessionControls) (путем настройки свойства **disableResilienceDefaults**), чтобы определить, следует ли Azure AD расширять существующие сеансы на основе сведений, собранных до сбоя.

### <a name="teamwork"></a>Teamwork
[Создайте чат](/graph/api/chat-post) с помощью разрешений приложений.

## <a name="january-2022-new-in-preview-only"></a>Январь 2022 г.: новое только в предварительной версии

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
Получение URL-адреса сайта OneDrive для бизнеса хранителя (свойство **siteWebUrl** ресурса [userSource](/graph/api/resources/ediscovery-userSource?view=graph-rest-beta&preserve-view=true)).

### <a name="devices-and-apps--cloud-pc"></a>Устройства и приложения | Облачный ПК
- Получите или обновите [параметры для организации](/graph/api/resources/cloudpcorganizationsettings?view=graph-rest-beta&preserve-view=true), включая версию операционной системы Windows для предоставления на облачных компьютерах, а также тип учетной записи пользователя на предоставленных облачных компьютерах.
- [Измените тип учетной записи](/graph/api/cloudPC-changeUserAccountType?view=graph-rest-beta&preserve-view=true) пользователя на указанном облачном компьютере.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Рецензенты проверки доступа могут [записывать](/graph/api/accessreviewinstancedecisionitem-recordalldecisions?view=graph-rest-beta&preserve-view=true) решения, для которых текущий пользователь является рецензентом.
- Настройте [дату и время последнего входа пользователя в качестве информации](/graph/api/resources/userLastSignInRecommendationInsightSetting?view=graph-rest-beta&preserve-view=true), чтобы помочь рецензентам принимать решения для [определения расписания проверки доступа](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true).
- Настройте [дату и время последнего входа пользователя в качестве информации](/graph/api/resources/userSignInInsight?view=graph-rest-beta&preserve-view=true) для [принятия решения о доступе пользователя или субъекта в экземпляре проверки доступа](/graph/api/resources/accessreviewinstancedecisionitem?view=graph-rest-beta&preserve-view=true).
- Инициатор запроса пакета для доступа может предоставить пользовательские сведения в составе [ресурса пакета для доступа](/graph/api/resources/accesspackageresource?view=graph-rest-beta&preserve-view=true), который может использоваться для принятия решений об утверждении пакета для доступа.
- Инициатор запроса может изменить ответ на [вопрос](/graph/api/resources/accessPackageQuestion?view=graph-rest-beta&preserve-view=true) в [политике назначения пакета для доступа](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
- Получите сведения о [методах проверки подлинности, зарегистрированных для пользователя](/graph/api/resources/userRegistrationDetails?view=graph-rest-beta&preserve-view=true), таких как многофакторная проверка подлинности, самостоятельный сброс пароля и проверка подлинности без пароля.
- Получите следующие свойства для события [входа в систему](/graph/api/resources/signIn?view=graph-rest-beta&preserve-view=true) пользователя или приложения в организации: 
  - Любой [контекст проверки подлинности](/graph/api/resources/authenticationContext?view=graph-rest-beta&preserve-view=true) условного доступа.
  - Любая [политика времени существования сеанса](/graph/api/resources/sessionLifetimePolicy?view=graph-rest-beta&preserve-view=true)условного доступа.
  - Идентификатор ресурса Azure, доступ к которому осуществляется при входе.
  - Идентификатор учетных данных федеративного удостоверения приложения, если он использовался для входа.
  - Идентификатор субъекта-службы, представляющего целевой ресурс в событии входа.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
Получение отчетов об использовании, относящихся к Outlook, OneDrive и SharePoint для облака Microsoft для государственных организаций США. См. сводку по [облачным развертываниям](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true#cloud-deployments).

### <a name="sites-and-lists"></a>Сайты и списки
- Добавьте или синхронизируйте тип контента из концентратора типов контента на [сайт](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) или в [список](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true) с помощью действия [addCopyFromContentTypeHub](/graph/api/contenttype-addcopyfromcontenttypehub?view=graph-rest-beta&preserve-view=true). Это делает тип контента или его обновление доступными для определенного сайта или списка, где это необходимо. Это улучшение по сравнению с устаревшей инфраструктурой синхронизации, которая распространяет тип контента на все сайты в организации, сокращая время ожидания распространения публикации. 
- Получение одной или нескольких [многофункциональных длительных операций](/graph/api/resources/richlongrunningoperation?view=graph-rest-beta&preserve-view=true), выполняемых на сайте или в списке, что может происходить при синхронном добавлении типа контента.
- Получите коллекцию совместимых ресурсов [типа контента](/graph/api/resources/contentType?view=graph-rest-beta&preserve-view=true) из концентратора типов контента, совместимых с помощью действия [getCompatibleHubContentTypes](/graph/api/contenttype-getcompatiblehubcontenttypes?view=graph-rest-beta&preserve-view=true). 

### <a name="teamwork"></a>Teamwork
- Разрешите пользователям выбирать **LastModifiedDateTime** или **CreatedDateTime** в качестве порядка сортировки при [перечислении сообщений в чате](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true).
- Укажите атрибуцию пользователя (в свойстве **onBehalfOf**), когда бот отправляет [сообщение чата](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) от имени пользователя.
- Добавьте в [чат](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) следующие типы участников:
  - [Анонимный гость](/graph/api/resources/anonymousGuestConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Пользователь учетной записи Майкрософт](/graph/api/resources/microsoftAccountUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Пользователь Skype для бизнеса](/graph/api/resources/skypeForBusinessUserConversationMember?view=graph-rest-beta&preserve-view=true)
  - [Пользователь Skype](/graph/api/resources/skypeUserConversationMember?view=graph-rest-beta&preserve-view=true)
- Использование делегированного разрешения `TeamworkTag.Read` для чтения [тегов](/graph/api/resources/teamworktag?view=graph-rest-beta&preserve-view=true) и [присвоения тегов участникам](/graph/api/resources/teamworktagmember?view=graph-rest-beta&preserve-view=true) в Teams от имени пользователя, выполнившего вход.

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
