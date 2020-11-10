---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: c0399ce4b171224225c570e88b9fbd094e9d2c8d
ms.sourcegitcommit: 4e7830a22b440bbbcfa795937af85d8542e5525b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982697"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](changelog.md). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_ , в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="november-2020-new-and-generally-available"></a>Ноябрь 2020 г.: новые и общедоступные возможности

### <a name="teamwork"></a>Командная работа
- Общая доступность разрешений с согласием для конкретных ресурсов (RSC). Разрешения RSC позволяют владельцам команд предоставлять детальные разрешения рабочим приложениям на доступ и/или изменение конкретных данных команды, например на чтение параметров команды или изменение названий каналов, описаний и других параметров.
- Общая доступность API, применяемых к [каналу](/graph/api/resources/channel) или сообщениям в канале. API включают:
  - [Создание](/graph/api/conversationmember-add) или [удаление](/graph/api/conversationmember-delete) участника беседы из канала.
  - [Обновление роли участника](/graph/api/conversationmember-update) в канале.
  - Получение конкретного сообщения или всех сообщений в канале.
  - Получение конкретного ответа или всех ответов в канале.
  - [Отслеживание новых или обновленных сообщений в канале](/graph/api/chatmessage-delta).

## <a name="november-2020-new-in-preview-only"></a>Ноябрь 2020г.: новые возможности только в предварительной версии

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
[Подписывайтесь на уведомления об изменениях](webhooks.md) в [определении задачи печати](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Поиск
Вы можете объединять числовые или строковые результаты поиска, импортированные [соединителями Microsoft Graph](/microsoftsearch/connectors-overview), которые настроены в качестве уточняемых в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Ознакомьтесь с дополнительными сведениями об [уточнении результатов поиска с помощью агрегирования](search-concept-aggregation.md).

## <a name="october-2020-new-and-generally-available"></a>Октябрь 2020 г.: новые и общедоступные возможности

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
Получайте новые свойства, относящиеся к [пользователю](/graph/api/resources/user), который является корпоративным сотрудником: дата найма, связь с организацией, например отдел и место возникновения затрат, и тип сотрудника, например консультант, подрядчик или поставщик. Для этих свойств требуется указать параметр запроса OData `$select` в операции GET.

## <a name="october-2020-new-in-preview-only"></a>Октябрь 2020 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Собрание по сети
- Определите роль участника в [собрании по сети](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) в качестве участника или выступающего, используя свойство **role** типа [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo?view=graph-rest-beta&preserve-view=true).
- Получайте объект [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) путем [фильтрации по свойству joinWebUrl собрания](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-3-retrieve-an-online-meeting-by-joinweburl).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать

- Прекращение поддержки действия **uploadData** , вместо которого применяется [создание сеанса отправки](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) для [отправки документа](upload-data-to-upload-session.md) на принтер или общий принтер.
- Прекращение поддержки свойства **printDocument** в [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true), вместо которого применяется аналогичное свойство **configuration** в [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Получайте URL-адрес исходного или конечного задания для перенаправляемого объекта **printJob** , используя свойство **redirectedFrom** или **redirectedTo**.
- Получайте текущее состояние **printJob** , используя свойство **state** и новое свойство **details**.
- Получайте коллекцию общих принтеров, связанных с объектом [printer](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), используя связь **shares**. 
- Прекращение поддержки свойства **processingStateReasons** объекта **printer** , вместо которого применяется свойство **status**. Свойство **status** относится к типу [printer status](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) и представляет свойство **details**. Используйте свойство **details** для определения причины текущего состояния принтера.
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
Администраторы могут просмотреть [примеры использования командлетов PowerShell](insights-customize-item-insights-privacy.md#how-to-configure-item-insights-setting-via-powershell), чтобы настроить параметры аналитики элементов для организации.

### <a name="teamwork"></a>Командная работа
- Используйте атрибут **channelCreationMode** экземпляра, чтобы указать, что создается [канал](https://docs.microsoft.com/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true#instance-attributes) для обслуживания миграции данных. Используйте атрибут [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true), чтобы указать на завершение миграции и возможность публикации и чтения сообщений участниками.
- Используйте атрибут **teamCreationMode** экземпляра, чтобы указать, что создается [команда](https://docs.microsoft.com/graph/api/resources/team?view=graph-rest-beta&preserve-view=true#instance-attributes) для обслуживания миграции. Используйте атрибут [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true), чтобы указать на завершение миграции и возможность выполнения операций участников, а также публикации сообщений участниками.


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)** , если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
