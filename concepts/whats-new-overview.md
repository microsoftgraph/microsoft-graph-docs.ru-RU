---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 6104775b7e5f73785f013c55f3bbc07352ec02b0
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645334"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.

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