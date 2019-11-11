---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 9ebdbcccff19f5c5a099efa3c0228392276a3cc3
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37968467"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

Знаете ли вы, что некоторые новые возможности Microsoft Graph реализуются на основе распространенных запросов сообщества разработчиков? 

Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 

Ниже представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API см. в [ноябрьском](changelog.md#november-2019) и [октябрьском](changelog.md#october-2019) разделах журнала изменений API. 


## <a name="november-2019-new-and-generally-available"></a>Ноябрь 2019 г.: новые и общедоступные возможности

### <a name="identity-and-access"></a>Идентификация и доступ

Регистрация [приложений](/graph/api/resources/application?view=graph-rest-1.0), проходящих проверку подлинности в Azure Active Directory (Azure AD).


## <a name="november-2019-new-in-preview"></a>Ноябрь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="calendar"></a>Календарь

[Настройка свойств](/graph/api/place-update?view=graph-rest-beta) для расширенных типов расположений [комната](/graph/api/resources/room?view=graph-rest-beta) и [список комнат](/graph/api/resources/roomlist?view=graph-rest-beta).


### <a name="people-and-workplace-intelligence"></a>Люди и рабочая аналитика

Первое появление ресурса [профиль](/graph/api/resources/profile?view=graph-rest-beta), который является расширенным представлением нового поколения записей людей в службах Майкрософт. Этот ресурс связан с распространенными и удобными атрибутами людей, включая информацию о всех важных датах, таких как [годовщины](/graph/api/resources/personanniversary?view=graph-rest-beta), а также об [образовании](/graph/api/resources/educationalactivity?view=graph-rest-beta), [должностях](/graph/api/resources/workposition?view=graph-rest-beta) и [интересах](/graph/api/resources/personinterest?view=graph-rest-beta), уровнях владения [языками](/graph/api/resources/languageproficiency?view=graph-rest-beta) и [навыками](/graph/api/resources/skillproficiency?view=graph-rest-beta), об [участии в проектах](/graph/api/resources/projectparticipation?view=graph-rest-beta) и [связи с веб-сайтами](/graph/api/resources/personwebsite?view=graph-rest-beta), а также прочие сведения об [учетной записи](/graph/api/resources/useraccountinformation?view=graph-rest-beta) и контактные данные.


### <a name="search"></a>Поиск
Первое появление [API Microsoft Search](search-concept-overview.md), с помощью которого пользователи приложений могут получать индивидуально адаптированные, более актуальные и релевантные результаты поиска с использованием возможностей Microsoft Graph. Можно использовать функцию [запроса](/graph/api/search-query?view=graph-rest-beta), которая по умолчанию выполняет поиск в сообщениях и событиях Outlook, а также в файлах OneDrive и SharePoint в облаке Майкрософт. Можно использовать [соединители](/microsoftsearch/connectors-overview), доступные в [коллекции соединителей Microsoft Graph](/microsoftsearch/connectors-gallery), чтобы задействовать поисковые данные за пределами облака Майкрософт. Также можно [создавать собственные соединители](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), индексировать внешние настраиваемые элементы и файлы, а также отправлять запросы к определенным внешним источникам данных.


## <a name="october-2019-new-and-generally-available"></a>Октябрь 2019 г.: новые и общедоступные возможности

### <a name="identity-and-access"></a>Идентификация и доступ
- Использование [контактов организации](/graph/api/resources/orgcontact?view=graph-rest-1.0) в рабочих приложениях. Контакты организации находятся под управлением администраторов организации и синхронизируются из локальной службы каталогов Active Directory или из Exchange Online.
- Настройка [проверки подлинности на основе сертификатов](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) в [организации](/graph/api/resources/organization?view=graph-rest-1.0).
- Добавление и удаление [учетных данных с паролем](/graph/api/resources/passwordcredential?view=graph-rest-1.0) для [приложений](/graph/api/resources/application?view=graph-rest-1.0).

### <a name="mail"></a>Почта
Использование нового параметра **message** для обновления любых записываемых свойств [message](/graph/api/resources/message?view=graph-rest-1.0) при [ответе](/graph/api/message-reply?view=graph-rest-1.0) на сообщение, например [для добавления получателя в ответ](/graph/api/message-reply#example?view=graph-rest-1.0).

### <a name="microsoft-graph-data-connect"></a>Подключение к данным Microsoft Graph
Разработчики и исследователи данных теперь могут использовать [инструменты для преобразования данных Office 365 в формат общей модели данных](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md). В этом случае обеспечивается согласование схемы данных с другими наборами данных, совместимыми с Open Data Initiative (ODI). 


### <a name="microsoft-graph-sdks"></a>Пакеты SDK Microsoft Graph
- Использование обработчиков хаоса в SDK JavaScript для проверки устойчивости приложения к сбоям серверов, возникающим в трудновоспроизводимых условиях.
- Прочтите о [создании вызовов API с помощью пакетов SDK](/graph/sdks/create-requests).

### <a name="users"></a>Пользователи
- [Получение](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0) или [настройка](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0) параметров предпочитаемого пользователем формата даты и времени [для почтового ящика пользователя](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). 
- Отслеживание даты и времени последнего изменения пароля [пользователя](/graph/api/resources/user?view=graph-rest-1.0).

## <a name="october-2019-new-in-preview"></a>Октябрь 2019 г.: новые возможности в предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="calendar"></a>Календарь
- Организаторы собраний могут [разрешить приглашенным предлагать другое время собраний](outlook-calendar-meeting-proposals.md). При получении ответа на приглашение, содержащего предложение другого времени, организатор может принять предложение и [обновить](/graph/api/event-update?view=graph-rest-beta) время собрания.
- Программное предоставление доступа к календарю с более тесным взаимодействием с использованием пользовательского интерфейса Outlook. Поддерживается отслеживание разрешений текущего пользователя и состояния общего доступа к календарю, а также следующие возможности:
  - Для каждого [календаря](/graph/api/resources/calendar?view=graph-rest-beta) теперь можно управлять [разрешениями](/graph/api/resources/calendarpermission?view=graph-rest-beta) каждого пользователя, которому предоставлен доступ к календарю. 
  - Для каждого [почтового ящика](/graph/api/resources/mailboxsettings?view=graph-rest-beta) теперь можно указать, кто получает сообщения о собраниях и ответы на эти сообщения: делегат, владелец почтового ящика или и тот, и другой. 
- Дополнительная поддержка собраний по сети:
  - В каждом **календаре** можно указать разрешенных и используемых по умолчанию поставщиков собраний по сети.
  - Можно создать или обновить [мероприятие](/graph/api/resources/event?view=graph-rest-beta), доступное по сети, и предоставить участникам сведения для присоединения к собранию по сети. 
  - В частности, можно использовать **onlineMeetingProvider** и **onlineMeeting** — это новые свойства **мероприятий**, с помощью которых можно задать или указать Microsoft Teams в качестве поставщика собраний по сети. Это временное решение [известной проблемы](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) со свойством **onlineMeetingUrl**.

### <a name="devices-and-apps"></a>Устройства и приложения
В [октябрьском](changelog.md#october-2019) выпуске Intune обновлены правила доступа для определенных сценариев

### <a name="graph-explorer"></a>Песочница Graph
Попробуйте [следующую версию песочницы Graph](https://developer.microsoft.com/graph/graph-explorer/preview) и воспользуйтесь полезной контекстной информацией, включая разрешения, маркеры доступа и фрагменты кода SDK, на новых вкладках **Разрешения**, **Проверка подлинности** и **Фрагменты кода**. С помощью ползунка **просмотра** можно переключаться между [рабочей](https://developer.microsoft.com/graph/graph-explorer) и новой предварительной версией песочницы Graph.

### <a name="groups"></a>Группы
- Управление видимостью [групп](/graph/api/resources/group?view=graph-rest-beta) в определенных частях пользовательского интерфейса Outlook или в клиенте Outlook с помощью свойств **hideFromAddressLists** и **hideFromOutlookClients**.
- [Назначение](/graph/api/group-assignlicense?view=graph-rest-beta) и удаление лицензий пользователям в [группе](/graph/api/resources/group?view=graph-rest-beta).

### <a name="identity-and-access"></a>Идентификация и доступ
- Использование [политик условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta) для настройки правил доступа для организации. Эти правила учитывают сигналы о пользователях или об удостоверениях устройств, включая членство пользователей или групп, расположение IP-адреса, а также поведение, включая попытки доступа к определенным приложениям и опасное поведение при входе.
- [Управление правами](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta) можно использовать для управления доступом к группам, приложениям и сайтам SharePoint Online для пользователей внутри организации и вне ее.
- Добавление и удаление [учетных данных с паролем](/graph/api/resources/passwordcredential?view=graph-rest-beta) для [приложений](/graph/api/resources/application?view=graph-rest-beta) и [субъектов-служб](/graph/api/resources/serviceprincipal?view=graph-rest-beta).
- Управление [ключами политики инфраструктуры доверия](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta) Azure AD B2C.
- Можно определить политики [пользовательского процесса](/graph/api/resources/identityuserflow?view=graph-rest-beta) Azure AD B2C для входа, регистрации, объединенной процедуры регистрации и входа, сброса пароля и обновления профиля.
- Настройка [меток защиты информации](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta), чтобы классифицировать конфиденциальность данных для пользователя или клиента.
- Существующие приложения, использующие API для [событий с риском для идентификации](/graph/api/resources/identityriskevent?view=graph-rest-beta), должны перейти на использование функций [обнаружения риска](/graph/api/resources/riskdetection?view=graph-rest-beta) в службе защиты идентификации Azure AD. Дополнительные сведения и график прекращения использования прежнего решения см. в [публикации в блоге](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/).


### <a name="mail"></a>Почта
[Вложение больших файлов размером до 150 МБ](outlook-large-attachments.md) в экземпляр [сообщения](/graph/api/resources/message?view=graph-rest-beta) путем создания [сеанса отправки](/graph/api/resources/uploadsession?view=graph-rest-beta) и итерационной отправки диапазонов файла, пока не отправятся все байты файла. 

### <a name="microsoft-graph-security-api"></a>Microsoft Graph Security API
- Предварительная версия интеграции с RSA NetWitness, ServiceNow и Splunk для сопоставления и синхронизации [оповещений](/graph/api/resources/security-api-overview?view=graph-rest-beta#alerts), улучшения защиты от угроз и реагирования.
- Новые переключатели добавлены в [соединитель безопасности Microsoft Graph](https://docs.microsoft.com/connectors/microsoftgraphsecurity/) и в [сборники схем](https://docs.microsoft.com/azure/security-center/security-center-playbooks) для логических приложений и потоков. См. [примеры сборников схем](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Поддержка отправки [индикаторов угроз](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) в Microsoft Defender ATP для блокирования или отправки оповещений об угрозах с использованием собственных источников аналитики. Интеграция с партнерами, такими как ThreatConnect, дает заказчикам возможность отправлять индикаторы непосредственно из решений аналитики угроз и автоматизации. 

### <a name="notifications"></a>Уведомления
- [Создание и отправка уведомлений](/graph/api/user-post-notifications?view=graph-rest-beta) всем клиентам приложения во всех конечных точках устройств, где пользователи могли войти в систему, без необходимости управлять разрешениями, делегированными пользователями.
- [Целевые конечные точки политики](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta) в [уведомлениях](/graph/api/resources/notification?view=graph-rest-beta) пользователей позволяют целенаправленно управлять уведомлениями на платформах Windows, iOS, Android или WebPush.
- Можно указать [политику отката](/graph/api/resources/fallbackpolicy?view=graph-rest-beta) для уведомлений для конечных точек iOS, чтобы отправлять высокоприоритетные необработанные уведомления, доставка которых на устройства другими способами может быть невозможной из-за ограничений, действующих для конкретной платформы, например, из-за использования режима экономии заряда аккумулятора.
- Можно использовать новые компактные SDK уведомлений для Windows, iOS, Android и JavaScript вместо [SDK Project Rome](https://github.com/Microsoft/project-rome), чтобы воспользоваться улучшенной моделью проверки подлинности и поддержкой веб-приложений с push-уведомлениями.
 
### <a name="powershell-sdk"></a>Пакет SDK для PowerShell 
Разработчики и ИТ-специалисты могут обратить внимание на выпуск [пакета SDK Microsoft Graph для Powershell](https://github.com/microsoftgraph/msgraph-sdk-powershell). Этот пакет будет формировать модули, содержащие командлеты для создания запросов API REST Microsoft.

## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?
- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Office 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Office 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

