---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: e5e8e8ba5c67e81abe9bf108be5f72bacfe2739f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921933"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="april-2021-new-and-generally-available"></a>Апрель 2021 г.: новые и общедоступные возможности

### <a name="teamwork"></a>Командная работа
- Определяйте канал по свойству **channelIdentity**, если [chatMessage](/graph/api/resources/chatmessage) находится в [канале](/graph/api/resources/channel).
- Определяйте чат по свойству **chatId**, если **[chatMessage](/graph/api/resources/chatmessage)** находится в [чате](/graph/api/resources/chat).
- Используйте связь **messages**, чтобы получить все ресурсы [chatMessage](/graph/api/resources/chatmessage) в [чате](/graph/api/resources/chat).

## <a name="april-2021-new-in-preview-only"></a>Апрель 2021 г.: новые возможности только в предварительной версии

### <a name="teamwork"></a>Командная работа
Используйте [предоставление разрешения для определенных ресурсов](/graph/api/resources/resourcespecificpermissiongrant?view=graph-rest-beta&preserve-view=true), чтобы перечислять приложения с доступом к указанной [группе ](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) или [чату](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).

## <a name="march-2021-new-and-generally-available"></a>Март 2021 г.: новые и общедоступные возможности

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
- Переносите журнал сообщений и данные пользователей из внешней системы в канал Teams, позволяя пользователям легко продолжать общение. Используйте следующие методы, поддерживающие сценарий миграции.
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
Применение новой модели [проверок доступа](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) для участия в группах и всех других поддерживаемых типов ресурсов. Прекращение поддержки [устаревшей модели проверок доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true).

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

## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на сайте [сообщества Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
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