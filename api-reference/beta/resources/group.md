---
title: Тип ресурса group
description: Представляет группу Azure Active Directory (Azure AD), которая может быть группой Office 365, командой в Microsoft Teams, группой безопасности или динамической группой.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: b9f4e249c763b7617e946432d10f33166173dd84
ms.sourcegitcommit: d9d8b908061b3680e8a52790a6c9aaf8e51ceea0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2019
ms.locfileid: "28328015"
---
# <a name="group-resource-type"></a>Тип ресурса group

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет группу Azure Active Directory (Azure AD), которая может быть группой Office 365, командой в Microsoft Teams, группой безопасности или динамической группой.
Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).

> **Группы Microsoft Teams и Office 365 поддерживают совместную работу групп**. С Microsoft Teams можно использовать большинство API групп Office 365. Чтобы создать [команду](team.md), сначала [создайте группу](../api/group-post-groups.md), а затем [добавьте к ней команду](../api/team-put-teams.md). Дополнительные сведения см. в [обзоре Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Управление группами**| | |
|[Создание группы](../api/group-post-groups.md) | [group](group.md) |Создание указанной группы. Это может быть группа Office 365, группа безопасности, динамическая группа или команда.|
|[Получение группы](../api/group-get.md) | [group](group.md) |Чтение свойств и связей объекта group.|
|[Обновление группы](../api/group-update.md) | Нет |Обновление свойств объекта group. |
|[Удаление группы](../api/group-delete.md) | Нет |Удаление объекта group. |
|[delta](../api/group-delta.md)|Коллекция group| Получение добавочных изменений для групп. |
|[Перечисление groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)| Перечисление политик жизненного цикла для групп. |
|[Перечисление владельцев](../api/group-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение владельцев группы из свойства навигации **owners**.|
|[Добавление владельца](../api/group-post-owners.md) |[directoryObject](directoryobject.md)| Добавление владельца группы путем помещения в свойство навигации **owners** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты).|
|[Удаление владельца](../api/group-delete-owners.md) | Нет |Удаление владельца из группы Office 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **owners**.|
|[Перечисление участников](../api/group-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей и групп, являющихся непосредственными участниками этой группы, из свойства навигации **members**.|
|[Перечисление транзитивных участников](../api/group-list-transitivemembers.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, групп, устройств и субъектов-служб, являющихся участниками, включая вложенных участников этой группы|
|[Добавление участника](../api/group-post-members.md) |[directoryObject](directoryobject.md)| Добавление пользователя или группы в данную группу путем помещения в свойство навигации **members** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты).|
|[Удаление участника](../api/group-delete-members.md) | Нет |Удаление члена из группы Office 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **members**. Вы можете удалять пользователей или другие группы. |
|[Список memberOf](../api/group-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп и административных единиц, непосредственным участником которых является группа, из свойства навигации memberOf.|
|[Перечисление транзитивных свойств memberOf](../api/group-list-transitivememberof.md) |Коллекция [directoryObject](directoryobject.md)| Перечисление групп и административных единиц, в которых состоит пользователь. Эта операция является транзитивной и включает группы, в которых состоит группа. |
|[checkMemberGroups](../api/group-checkmembergroups.md)|Коллекция String|Проверка участия в списке групп. Это транзитивная функция.|
|[getMemberGroups](../api/group-getmembergroups.md)|Коллекция String|Возврат всех групп, в которых состоит эта группа. Это транзитивная функция.|
|[getMemberObjects](../api/group-getmemberobjects.md)|Коллекция String|Возвращение всех групп и административных единиц, в которых состоит группа. Это транзитивная функция. |
|[Создание параметра](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Создание объекта setting на основе directorySettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. В случае этой операции могут использоваться только шаблоны специально для групп.|
|[Получение параметра](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Считывание свойств определенного объекта setting.|
|[Перечисление параметров](../api/directorysetting-list.md) | Коллекция [directorySetting](directorysetting.md) |Перечисление свойств всех объектов setting.|
|[Обновление параметра](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Обновление объекта setting. |
|[Удаление параметра](../api/directorysetting-delete.md) | Нет |Удаление объекта setting. |
|[Перечисление конечных точек](../api/group-list-endpoints.md) |Коллекция [endpoint](endpoint.md)| Получение коллекции объектов endpoint. |
|[Получение конечной точки](../api/endpoint-get.md) | [endpoint](endpoint.md) | Чтение свойств и связей объекта endpoint. |
|[delta](../api/group-delta.md)|Коллекция group| Получение добавочных изменений для групп. |
|[validateProperties](../api/group-validateproperties.md)|JSON| Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования. | 
|**Календарь**| | |
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
|[Удаление цепочки](../api/group-delete-thread.md) |Нет| Удаление объекта thread
|[Перечисление acceptedSenders](../api/group-list-acceptedsenders.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей или групп из списка acceptedSenders для данной группы.|
|[Добавление acceptedSender](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| Добавление User или Group в коллекцию acceptedSenders.|
|[Удаление acceptedSender](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| Удаление User или Group из коллекции acceptedSenders.|
|[Список rejectedSenders](../api/group-list-rejectedsenders.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей или групп из списка rejectedSenders для данной группы.|
|[Добавление rejectedSender](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| Добавление User или Group в коллекцию rejectedSenders.|
|[Удаление rejectedSender](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| Удаление новых User или Group из коллекции rejectedSenders.|
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
|[removeFavorite](../api/group-removefavorite.md)|Нет|Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для групп Office 365.|
|[Перечисление memberOf](../api/group-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп и административных единиц, непосредственным участником которых является пользователь, из свойства навигации **memberOf**.|
|[Перечисление объектов joinedTeams](../api/user-list-joinedteams.md) |Коллекция [group](group.md)| Получение команд Microsoft Teams, непосредственным участником которых является пользователь.|
|[subscribeByMail](../api/group-subscribebymail.md)|Нет|Задает для свойства isSubscribedByMail значение **true**. Позволяет текущему пользователю получать беседы по электронной почте. Поддерживается только для групп Office 365.|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|Нет|Задает для свойства isSubscribedByMail значение **false**. Отключает получение бесед по электронной почте для текущего пользователя. Поддерживается только для групп Office 365.|
|[resetUnseenCount](../api/group-resetunseencount.md)|Нет|Сброс значений unseenCount до 0 для всех записей, которые текущий пользователь не просматривал со времени последнего посещения. Поддерживается только для групп Office 365.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowExternalSenders|Логическое|Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.|
|assignedLicenses|Коллекция [assignedLicense](assignedlicense.md)|Лицензии, назначенные группе. Только для чтения.|
|autoSubscribeNewMembers|Логическое|Значение по умолчанию: **false**. Указывает, будут ли новые члены группы автоматически подписаны на получение уведомлений по электронной почте. Это свойство можно задать в запросе PATCH для группы. Не задавайте его в первоначальном запросе POST, создающем группу.|
|classification|String|Описывает классификацию для группы (например, незначительное, среднее или значительное влияние на бизнес). Допустимые значения для этого свойства определяются созданием значения [setting](directorysetting.md) ClassificationList на базе [определения шаблона](directorysettingtemplate.md).|
|createdDateTime|DateTimeOffset| Метка времени создания группы. Значение не может изменяться и заполняется автоматически, когда создается группа. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|description|String|Необязательное описание для группы.|
|displayName|String|Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.|
|expirationDateTime|DateTimeOffset| Метка времени завершения срока действия группы. Значение не может изменяться и заполняется автоматически, когда создается группа. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|groupTypes|Коллекция String| Указывает тип создаваемой группы. Возможные значения: `Unified` для создания группы Office 365 или `DynamicMembership` для создания динамических групп.  Для остальных типов групп, таких как группы с включенной поддержкой безопасности и группы безопасности с включенной поддержкой электронной почты, это свойство не задается.|
|id|String|Уникальный идентификатор группы. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|isSubscribedByMail|Логическое|Значение по умолчанию: **true**. Указывает, подписан ли текущий пользователь на получение бесед по электронной почте.|
|licenseProcessingState|String|Указывает состояние назначения лицензии группы для всех участников группы. Только для чтения. Возможные значения: `QueuedForProcessing`, `ProcessingInProgress` и `ProcessingComplete`.|
|mail|String|SMTP-адрес группы, например "serviceadmins@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailEnabled|Boolean|Указывает, включена ли для этой группы поддержка почты. Если для свойства **securityEnabled** также задано значение **true**, это группа безопасности с включенной поддержкой почты. В противном случае это группа рассылки Microsoft Exchange.|
|mailNickname|String|Почтовый псевдоним для группы, уникальный в организации. Это свойство должно быть указано при создании группы. Поддерживает параметр $filter.|
|membershipRule|String|Правило, определяющее участников этой группы, если группа является динамической (groupTypes содержит `DynamicMembership`). Дополнительные сведения о синтаксисе правила членства см. в [здесь](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)|
|membershipRuleProcessingState|String|Указывает, включена или приостановлена динамическая обработка членства. Возможные значения: On или Paused|
|onPremisesLastSyncDateTime|DateTimeOffset|Указывает время последней синхронизации объекта с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Поддерживает параметр $filter.|
|onPremisesProvisioningErrors|Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md)| Ошибки при использовании продукта синхронизации Майкрософт во время подготовки. |
|onPremisesSecurityIdentifier|String|Содержит локальный идентификатор безопасности (SID) для локальной группы, синхронизированной с облаком. Только для чтения. |
|onPremisesSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения. Поддерживает параметр $filter.|
|preferredDataLocation|String|Предпочитаемое расположение данных для группы. Дополнительные сведения см. в статье [OneDrive Online с поддержкой нескольких регионов](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|Предпочитаемый язык для группы Office 365. Он должен быть представлен в формате ISO 639-1, например "ru-RU".|
|proxyAddresses|Коллекция String| Например: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` для выражений фильтра в случае многозначных свойств требуется оператор **any**. Только для чтения. Значение null не допускается. Поддерживает параметр $filter. |
|renewedDateTime|DateTimeOffset| Метка времени последнего обновления группы. Не может изменяться непосредственно. Обновляется только при выполнении [действия обновления](../api/grouplifecyclepolicy-renewgroup.md). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|securityEnabled|Логическое|Указывает, является ли эта группа группой безопасности. Если для свойства **mailEnabled** также задано значение true, это группа безопасности с включенной поддержкой почты. В противном случае это обычная группа безопасности. Для групп Office 365 должно быть задано значение **false**. Поддерживает параметр $filter.|
|theme|String|Указывает цветовую тему группы Office 365. Возможные значения: `Teal`, `Purple`, `Green`, `Blue`, `Pink`, `Orange` или `Red`.|
|unseenConversationsCount|Int32|Количество бесед, в которых было опубликовано одно или несколько сообщений с момента последнего посещения группы вошедшим в систему пользователем. Это свойство совпадает с **unseenCount**.|
|unseenCount|Int32|Количество бесед, в которых было опубликовано одно или несколько сообщений с момента последнего посещения группы вошедшим в систему пользователем. Это свойство совпадает с **unseenConversationsCount**.|
|unseenMessagesCount|Int32|Количество новых записей, опубликованных в беседах группы с момента последнего посещения группы вошедшим в систему пользователем.|
|visibility|String| Определяет видимость группы Office 365. Возможные значения: `private`, `public` или `hiddenmembership`. Пустые значения считаются общедоступными.  Дополнительные сведения см. в разделе [Параметры видимости группы](#group-visibility-options).<br>Видимость можно настроить только при создании группы. Ее нельзя изменить.<br>Видимость поддерживается только для единых групп. Она не поддерживается для групп безопасности.|

### <a name="group-visibility-options"></a>Параметры видимости группы

Ниже показано значение каждого свойства **видимости**.
 
|Значение|Описание|
|:----|-----------|
| `public` | К группе может присоединиться любой пользователь без необходимости разрешения владельца.<br>Любой пользователь может просматривать содержимое группы.|
| `private` | Чтобы присоединиться к группе, требуется разрешение владельца.<br>Пользователи, не являющиеся участниками группы, не могут просматривать ее содержимое.|
| `hiddenmembership` | Чтобы присоединиться к группе, требуется разрешение владельца.<br>Пользователи, не являющиеся участниками группы, не могут просматривать ее содержимое.<br>Пользователи, не являющиеся участниками группы, не могут просматривать ее участников.<br>Администраторы (глобальные, организации, пользователей и службы поддержки) могут просматривать список участников группы.<br>Группа отображается в глобальной адресной книге (глобальном списке адресов).|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|acceptedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым разрешено создавать записи или события календаря в этой группе. Если этот список не пуст, то добавлять записи разрешено только перечисленным в нем пользователям и группам.|
|calendar|[calendar](calendar.md)|Календарь группы. Только для чтения.|
|calendarView|Коллекция [event](event.md)|Представление календаря. Только для чтения.|
|conversations|Коллекция [conversation](conversation.md)|Беседы группы.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Пользователь или приложение, создавшие группу. ПРИМЕЧАНИЕ. Это значение не задается, если пользователь является администратором. Только для чтения.|
|drive|[drive](drive.md)|Используемый по умолчанию диск группы. Только для чтения.|
|drives|Коллекция [drive](drive.md)|Диск группы. Только для чтения.|
|endpoints|Коллекция [Endpoint](endpoint.md)| Конечные точки для группы. Только для чтения. Допускается значение null.|
|events|Коллекция [event](event.md)|События группы.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для группы. Только для чтения. Допускается значение null.|
|groupLifecyclePolicies|Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)|Коллекция политик жизненного цикла для этой группы. Только для чтения. Допускается значение null.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы и административные единицы, в которых состоит группа. Методы HTTP: GET (поддерживается для всех групп). Только для чтения. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)| Пользователи, контакты и группы, состоящие в этой группе. Методы HTTP: GET (поддерживается для всех групп), POST (поддерживается для групп безопасности, в том числе с включенной поддержкой почты), DELETE (поддерживается только для групп безопасности). Только для чтения. Допускается значение null.|
|membersWithLicenseErrors|Коллекция [User](user.md)|Список участников группы с ошибками лицензий после группового назначения лицензий. Только для чтения.|
|onenote|[OneNote](onenote.md)| Только для чтения.|
|owners|Коллекция [directoryObject](directoryobject.md)|Владельцы группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект. Методы HTTP: GET (поддерживается для всех групп), POST (поддерживается для групп безопасности, в том числе с включенной поддержкой почты), DELETE (поддерживается только для групп безопасности). Только для чтения. Допускается значение null.|
|photo|[profilePhoto](profilephoto.md)| Фотография профиля группы. |
|photos|Коллекция объектов [profilePhoto](profilephoto.md)| Фотографии профиля, принадлежащие группе. Только для чтения. Допускается значение null.|
|planner|[plannerGroup](plannergroup.md)| Выборочные службы Планировщика, доступные для группы. Только для чтения. Допускается значение null. |
|rejectedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым запрещено создавать записи или события календаря в этой группе. Допускается значение null.|
|settings|Коллекция [directorySetting](directorysetting.md)| Параметры, управляющие поведением группы, например, могут ли участники приглашать гостевых пользователей в группу. Допускается значение null.|
|sites|Коллекция объектов [site](site.md)|Список сайтов SharePoint в этой группе. Для доступа к сайту по умолчанию используйте путь /sites/root.|
|threads|Коллекция [conversationThread](conversationthread.md)| Цепочки бесед группы. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.

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
  "expirationDateTime": "String (timestamp)",
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
