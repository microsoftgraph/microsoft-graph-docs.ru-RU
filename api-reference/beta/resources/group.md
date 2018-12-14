---
title: Тип ресурса group
description: Представляет группу Azure Active Directory (Azure AD), который может быть группы с Office 365, группе в группами Майкрософт, динамические группы или группы безопасности.
ms.openlocfilehash: d48448991b75946f9ac60a037fee3b083601954a
ms.sourcegitcommit: 5747eb595bf0c7c391b2a5219c3ae9b6a48df26b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/14/2018
ms.locfileid: "27265236"
---
# <a name="group-resource-type"></a>Тип ресурса group

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет группу Azure Active Directory (Azure AD), который может быть группы с Office 365, группе в группами Майкрософт, динамические группы или группы безопасности.
Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- Добавление настраиваемых свойств данные как [расширения](/graph/extensibility-overview).
- Подписка на [уведомления об изменении](/graph/webhooks).
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).

> **Поддержка совместной работы групп группами Майкрософт и группы Office 365**. Можно использовать большинство функций API группы Office 365 с группами Майкрософт. Создание [группы](team.md), первый [Создать группу](../api/group-post-groups.md) , а затем [Добавить группы на него](../api/team-put-teams.md). Дополнительные сведения см [Обзор групп Майкрософт](teams-api-overview.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Управление группами**| | |
|[Создание группы](../api/group-post-groups.md) | [group](group.md) |Создание новой группы, как указано. Она может быть группы Office 365, динамическая группа, группы безопасности или групп.|
|[Получение группы](../api/group-get.md) | [group](group.md) |Чтение свойства и связи объекта группы.|
|[Обновление группы](../api/group-update.md) | Нет |Обновление свойств объекта group. |
|[Удаление группы](../api/group-delete.md) | Нет |Удаление объекта group. |
|[delta](../api/group-delta.md)|Коллекция групп| Получение добавочных изменений для групп. |
|[Перечисление groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)| Перечисление политик жизненного цикла для групп. |
|[Список владельцев](../api/group-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение владельцев группы из свойства навигации **owners**.|
|[Добавление владельца](../api/group-post-owners.md) |[directoryObject](directoryobject.md)| Добавление владельца группы путем помещения в свойство навигации **owners** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты).|
|[Удаление владельца](../api/group-delete-owners.md) | Нет |Удаление владельца из группы Office 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **owners**.|
|[Список членов](../api/group-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей и групп, являющихся непосредственными членами этой группы, из свойства навигации **members**.|
|[Доверия транзитивных членов списка](../api/group-list-transitivemembers.md) |Коллекция [directoryObject](directoryobject.md)| Получите пользователей, групп, устройств и субъектов-служб, которые являются участниками, включая вложенные участниками этой группы.|
|[Добавление элемента](../api/group-post-members.md) |[directoryObject](directoryobject.md)| Добавление пользователя или группы в данную группу путем помещения в свойство навигации **members** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты).|
|[Удаление члена](../api/group-delete-members.md) | Нет |Удаление члена из группы Office 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **members**. Вы можете удалять пользователей или другие группы. |
|[Перечисление memberOf](../api/group-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получите групп и административные единицы, которым будет прямого членом из свойства навигации член этой группы.|
|[Доверия транзитивных член списка](../api/group-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Список групп и административных единиц измерения, которые входит этот пользователь. Эта операция доверия транзитивных и включает в себя группы, которым будет вложенных членом этой группы. |
|[checkMemberGroups](../api/group-checkmembergroups.md)|Коллекция String|Проверьте наличие членства в список групп. Функция транзитивное.|
|[getMemberGroups](../api/group-getmembergroups.md)|Коллекция String|Возврат всех групп, в которых состоит эта группа. Это транзитивная функция.|
|[getMemberObjects](../api/group-getmemberobjects.md)|Коллекция String|Возвращает все группы и административных единиц измерения, которые должна быть членом группы. Функция транзитивное. |
|[Создание параметра](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Создайте объект параметр на основании directorySettingTemplate. Запрос POST необходимо задать settingValues для всех параметров, определенных в шаблоне. Только определенные шаблоны группы могут быть использованы для этой операции.|
|[Получение параметра](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Считывание свойств определенного объекта параметра.|
|[Перечисление параметров](../api/directorysetting-list.md) | [directorySetting](directorysetting.md) коллекции |Перечисление свойств всех объектов параметра.|
|[Обновление параметра](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Обновление объекта параметра. |
|[Удаление параметра](../api/directorysetting-delete.md) | Нет |Удаление объекта параметра. |
|[Список конечных точек](../api/group-list-endpoints.md) |Коллекция [конечных точек](endpoint.md)| Получение коллекции объектов конечной точки. |
|[Получение конечной точки](../api/endpoint-get.md) | [Конечная точка](endpoint.md) | Чтение свойства и связи объекта конечной точки. |
|[delta](../api/group-delta.md)|Коллекция групп| Получение добавочных изменений для групп. |
|[validateProperties](../api/group-validateproperties.md)|JSON| Проверить группу Office 365 отображаемое имя или псевдоним почты стандарту именования политик. | 
|**Calendar**| | |
|[Создание события](../api/group-post-events.md) |[event](event.md)| Создание объекта event путем публикации в коллекции объектов event.|
|[Получение события](../api/group-get-event.md) |[event](event.md)|Считывание свойств объекта event.|
|[Перечисление событий](../api/group-list-events.md) |Коллекция [event](event.md)| Получение коллекции объектов event.|
|[Обновление события](../api/group-update-event.md) |Нет|Обновление свойств объекта event.|
|[Удаление события](../api/group-delete-event.md) |Нет|Удаление объекта event.|
|[Список calendarView](../api/group-list-calendarview.md) |Коллекция [event](event.md)| Получение коллекции событий за указанный интервал времени.|
|**Беседы**| | |
|[Создание беседы](../api/group-post-conversations.md) |[conversation](conversation.md)| Создание беседы путем публикации в коллекции объектов conversation.|
|[Получение беседы](../api/group-get-conversation.md) |[conversation](conversation.md)| Считывание свойств объекта conversation.|
|[Перечисление бесед](../api/group-list-conversations.md) |Коллекция [conversation](conversation.md)| Получение коллекции объектов conversation.|
|[Удаление беседы](../api/group-delete-conversation.md) |Нет|Удаление объекта conversation.|
|[Получение цепочки](../api/group-get-thread.md) |[conversationThread](conversationthread.md)| Считывание свойств объекта thread.|
|[Перечисление цепочек](../api/group-list-threads.md) |Коллекция [conversationThread](conversationthread.md)| Получение всех цепочек группы.|
|[Обновление цепочки](../api/group-update-thread.md) |Нет| Обновление свойств объекта thread.|
|[Удаление цепочки](../api/group-delete-thread.md) |Нет| Удаление объекта потока
|[Вывод acceptedSenders](../api/group-list-acceptedsenders.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей или групп из списка acceptedSenders для данной группы.|
|[Добавление acceptedSender](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| Добавление User или Group в коллекцию acceptedSenders.|
|[Удаление acceptedSender](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| Удаление User или Group из коллекции acceptedSenders.|
|[Список rejectedSenders](../api/group-list-rejectedsenders.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей или групп из списка rejectedSenders для данной группы.|
|[Добавление rejectedSender](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| Добавление User или Group в коллекцию rejectedSenders.|
|[Удаление rejectedSender](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| Удаление нового объекта User или Group из коллекции объектов rejectedSender.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Другие ресурсы групп**| | |
|[Перечисление фотографий](../api/group-list-photos.md) |Коллекция объектов [profilePhoto](photo.md)| Получение коллекции фотографий профиля для группы.|
|[Перечисление планов](../api/plannergroup-list-plans.md) |Коллекция объектов [plannerPlan](plannerplan.md)| Получение планов, принадлежащих группе.|
|**Параметры пользователя**| | |
|[addFavorite](../api/group-addfavorite.md)|Нет|Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.|
|[removeFavorite](../api/group-removefavorite.md)|Нет|Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для Групп Office 365.|
|[Перечисление memberOf](../api/group-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп и административных единиц, непосредственным участником которых является пользователь, из свойства навигации **memberOf**.|
|[Перечисление объектов joinedTeams](../api/user-list-joinedteams.md) |Коллекция объектов [group](group.md)| Получите группами Майкрософт, который пользователь является непосредственным членом.|
|[subscribeByMail](../api/group-subscribebymail.md)|Нет|Присвойте свойству isSubscribedByMail значение **true**. Включение текущего пользователя на получение электронной почты бесед. Поддерживается только в Office 365 группы.|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|Нет|Присвойте свойству isSubscribedByMail значение **false**. Отключение текущего пользователя из бесед получения электронной почты. Поддерживается только в Office 365 группы.|
|[resetUnseenCount](../api/group-resetunseencount.md)|Нет|Сброс unseenCount 0 все сообщения, которые текущий пользователь не с момента их последнего посетить. Поддерживается только в Office 365 группы.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.|
|assignedLicenses|Коллекция [assignedLicense](assignedlicense.md)|Лицензии, назначенные в группу. Только для чтения.|
|autoSubscribeNewMembers|Логическое|Значение по умолчанию: **false**. Указывает, будут ли новые члены группы автоматически подписаны на получение уведомлений по электронной почте. Это свойство можно задать в запросе PATCH для группы. Не задавайте его в первоначальном запросе POST, создающем группу.|
|classification|String|Описывает классификацию для группы (например, незначительное, среднее или значительное влияние на бизнес). Допустимые значения для этого свойства определяются созданием значения [setting](directorysetting.md) ClassificationList на базе [определения шаблона](directorysettingtemplate.md).|
|createdDateTime|DateTimeOffset| Метка времени создания группы. Значение не может изменяться и автоматически заполняться, когда создается группа. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|описание|String|Необязательное описание для группы.|
|displayName|String|Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.|
|groupTypes|Коллекция String| Указывает тип создаваемой группы. Возможные значения: `Unified` Создание группы Office 365, или `DynamicMembership` для динамических групп.  Для всех других группы типов, таких как группы с включенной поддержкой безопасности и групп безопасности с включенной поддержкой электронной почты, это свойство не задано.|
|id|String|Уникальный идентификатор группы. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|isSubscribedByMail|Boolean|Значение по умолчанию: **true**. Указывает, подписан ли текущий пользователь на получение бесед по электронной почте.|
|licenseProcessingState|String.|Указывает состояние лицензии назначения группы всем членам группы. Только для чтения. Возможные значения: `QueuedForProcessing`, `ProcessingInProgress`, и `ProcessingComplete`.|
|mail|String|SMTP-адрес группы, например "serviceadmins@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailEnabled|Boolean|Указывает, включена ли для этой группы поддержка почты. Если для свойства **securityEnabled** также задано значение **true**, это группа безопасности с включенной поддержкой почты. В противном случае это группа рассылки Microsoft Exchange.|
|mailNickname|String|Почтовый псевдоним для группы, уникальный в организации. Это свойство должно быть указано при создании группы. Поддерживает параметр $filter.|
|membershipRule|String.|Правило, которое определяет элементы для этой группы, если группа является динамическая группа (содержит groupTypes `DynamicMembership`). Дополнительные сведения о синтаксисе правила членства можно [Синтаксис правила](https://azure.microsoft.com/en-us/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)|
|membershipRuleProcessingState|String.|Указывает, находится на обработку динамическое членство или приостановлено. Возможные значения: «На» или «Приостановлено»|
|onPremisesLastSyncDateTime|DateTimeOffset|Указывает время последнего, в котором объект был синхронизирован с локального каталога. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Поддерживает параметр $filter.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) коллекции| Ошибки при использовании продуктов Майкрософт синхронизации во время подготовки. |
|onPremisesSecurityIdentifier|String|Содержит локальный идентификатор безопасности (SID) для локальной группы, синхронизированной с облаком. Только для чтения. |
|onPremisesSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения. Поддерживает параметр $filter.|
|preferredDataLocation|String.|Расположение предпочитаемый данных для группы. Для получения дополнительных сведений см [OneDrive Online Multi-географически](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|Предпочитаемый язык для группы с Office 365. Необходимо соблюдать код ISO 639-1; Например, «en US».|
|proxyAddresses|Коллекция String| Например: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **любой** оператор для фильтра выражений на многозначные свойства. Только для чтения. Значение NULL не допускается. Поддерживает параметр $filter. |
|renewedDateTime|DateTimeOffset| Метка времени последнего обновления группы. Не может изменяться непосредственно. Обновляется только при выполнении [действия обновления](../api/grouplifecyclepolicy-renewgroup.md). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|securityEnabled|Логическое|Указывает, является ли эта группа группой безопасности. Если для свойства **mailEnabled** также задано значение true, это группа безопасности с включенной поддержкой почты. В противном случае это обычная группа безопасности. Для групп Office 365 должно быть задано значение **false**. Поддерживает параметр $filter.|
|темы|String.|Указывает группу Office 365 цвета темы. Возможные значения: `Teal`, `Purple`, `Green`, `Blue`, `Pink`, `Orange` или `Red`.|
|unseenConversationsCount|Int32|Количество бесед, которые были доставлены один или несколько новых сообщений с момента последнего посетить пользователь выполнил вход в группу. Это свойство соответствует **unseenCount**.|
|unseenCount|Int32|Количество бесед, которые были доставлены один или несколько новых сообщений с момента последнего посетить пользователь выполнил вход в группу. Это свойство соответствует **unseenConversationsCount**.|
|unseenMessagesCount|Int32|Количество новых сообщений, которые были доставлены групповой беседы с момента последнего посетить пользователь выполнил вход в группу.|
|visibility|String| Задает видимость группы с Office 365. Возможные значения: `private`, `public`, или `hiddenmembership`; пустые значения обрабатываются в открытом виде.  Просмотрите [параметры видимости группы](#group-visibility-options) для получения дополнительных сведений.<br>Видимость может устанавливаться только в том случае, если группа создается; нередактируемая.<br>Видимость поддерживается только для объединенных групп; не поддерживается для групп безопасности.|

### <a name="group-visibility-options"></a>Параметры видимости групп

Вот что каждое значение свойства **видимости** означает, что:
 
|Значение|Описание|
|:----|-----------|
| `public` | Для присоединения к группе без применения какого разрешение владельца.<br>Любой пользователь может просматривать содержимое группы.|
| `private` | Требуется разрешение владельца для присоединения к группе.<br>Не члены не могут просматривать содержимое группы.|
| `hiddenmembership` | Требуется разрешение владельца для присоединения к группе.<br>Не члены не могут просматривать содержимое группы.<br>Элементы не будут видны членов группы.<br>Администраторы (глобальная, компании, пользователь и служба технической поддержки) можно просмотреть состав группы.<br>Группа отображается в глобальный список адресов (GAL).|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|acceptedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым разрешено создавать записи или события календаря в этой группе. Если этот список не пуст, то добавлять записи разрешено только перечисленным в нем пользователям и группам.|
|календарь|[calendar](calendar.md)|Календарь группы. Только для чтения.|
|calendarView|Коллекция [event](event.md)|Представление календаря. Только для чтения.|
|conversations|Коллекция [conversation](conversation.md)|Беседы группы.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Пользователь или приложение, создавшие группу. ПРИМЕЧАНИЕ. Это значение не задается, если пользователь является администратором. Только для чтения.|
|drive|[drive](drive.md)|Диск группы по умолчанию. Только для чтения.|
|drives|Коллекция объектов [drive](drive.md)|Группа дисков. Только для чтения.|
|конечные точки|Коллекция [конечных точек](endpoint.md)| Конечные точки для группы. Только для чтения. Допускается значение null.|
|events|Коллекция [event](event.md)|События группы.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для группы. Только для чтения. Допускает значение null.|
|groupLifecyclePolicies|Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)|Коллекция жизненного цикла политик для этой группы. Только для чтения. Допускается значение null.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы и административных единиц измерения, которые должна быть членом этой группы. Методы HTTP: Получение (поддерживается для всех групп). Только для чтения. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)| Пользователи, контакты и группы, которые являются участниками этой группы. Методы HTTP: Получение (поддерживается для всех групп), POST (поддерживается для групп безопасности и групп безопасности с включенной поддержкой почты), DELETE (поддерживается только для групп безопасности) только для чтения. Допускается значение null.|
|membersWithLicenseErrors|Коллекция [пользователей](user.md)|Список членов группы с ошибками лицензии из данного назначения лицензий на основе группы. Только для чтения.|
|onenote|[OneNote](onenote.md)| Только для чтения.|
|owners|Коллекция [directoryObject](directoryobject.md)|Владельцев группы. Владельцы — это набор пользователей без прав администратора, которые могут изменять этот объект. Методы HTTP: Получение (поддерживается для всех групп), POST (поддерживается для групп безопасности и групп безопасности с включенной поддержкой почты), DELETE (поддерживается только для групп безопасности) только для чтения. Допускается значение null.|
|photo|[profilePhoto](profilephoto.md)| Группа фотографий профиля. |
|photos|Коллекция объектов [profilePhoto](profilephoto.md)| Фотографии профиля, принадлежащие группе. Только для чтения. Допускается значение null.|
|planner|[plannerGroup](plannergroup.md)| Выборочный планировщик работы службы, доступные в группу. Только для чтения. Допускается значение null. |
|rejectedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым запрещено создавать записи или события календаря в этой группе. Допускается значение null.|
|settings|[directorySetting](directorysetting.md) коллекции| Параметры, которые можно управлять поведением этой группы, например ли члены можно пригласить гостевых пользователей в группу. Допускается значение null.|
|sites|Коллекция объектов [site](site.md)|Список сайтов SharePoint в этой группе. Для доступа к сайту по умолчанию используйте путь /sites/root.|
|threads|Коллекция [conversationThread](conversationthread.md)| Цепочки бесед группы. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлена JSON ресурса

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "extensions",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",    
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "accessType": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isFavorite": true,  
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": ["string"],
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "unseenConversationsCount": 1024,
  "unseenCount": 1024,
  "unseenMessagesCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
