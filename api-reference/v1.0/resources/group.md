---
title: Тип ресурса group
description: Представляет группу Azure Active Directory (Azure AD), который может быть группы с Office 365, динамические группы или группы безопасности.
localization_priority: Priority
ms.openlocfilehash: f4d4de207cdc8e3f9fbd312ad08639b85cbc87a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828016"
---
# <a name="group-resource-type"></a>Тип ресурса group

Представляет группу Azure Active Directory (Azure AD), которая может быть группой Office 365, группой безопасности или динамической группой. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- Добавление настраиваемых свойств данные как [расширения](/graph/extensibility-overview).
- Подписка на [уведомления об изменении](/graph/webhooks).
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/user-delta.md)).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Управление группами**| | |
|[Создание группы](../api/group-post-groups.md) | [group](group.md) |Создание группы. Это может быть группа Office 365, группа безопасности или динамическая группа.|
|[Получение группы](../api/group-get.md) | [group](group.md) |Считывание свойств объекта group.|
|[Список групп](../api/group-list.md) |Коллекция [group](group.md) |Список объектов group и их свойств.|
|[Обновление группы](../api/group-update.md) | Нет |Обновление свойств объекта group. |
|[Удаление группы](../api/group-delete.md) | Нет |Удаление объекта group. |
|[delta](../api/group-delta.md)|Коллекция групп| Получение добавочных изменений для групп. |
|[Перечисление groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)| Перечисление политик жизненного цикла для групп. |
|[Renew](../api/group-renew.md)|Boolean|Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.|
|[Добавление владельца](../api/group-post-owners.md) |Нет| Добавление владельца группы путем помещения в свойство навигации **owners** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты).|
|[Список владельцев](../api/group-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение владельцев группы из свойства навигации **owners**.|
|[Удаление владельца](../api/group-delete-owners.md) | Нет |Удаление владельца из группы Office 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **owners**.|
|[Добавление члена](../api/group-post-members.md) |Нет| Добавление пользователя или группы в данную группу путем помещения в свойство навигации **members** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты).|
|[Список членов](../api/group-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей и групп, являющихся непосредственными членами этой группы, из свойства навигации **members**.|
|[Удаление члена](../api/group-delete-members.md) | Нет |Удаление члена из группы Office 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **members**. Вы можете удалять пользователей или другие группы. |
|[checkMemberGroups](../api/group-checkmembergroups.md)|Коллекция String|Проверка данной группы на членство в списке групп. Это транзитивная функция.|
|[getMemberGroups](../api/group-getmembergroups.md)|Коллекция String|Возврат всех групп, в которых состоит эта группа. Это транзитивная функция.|
|[getMemberObjects](../api/group-getmemberobjects.md)|Коллекция String|Возврат всех групп, в которых состоит эта группа. Это транзитивная функция. |
|[Создание параметра](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. В случае этой операции могут использоваться только шаблоны специально для групп.|
|[Получение параметра](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта параметра. |
|[Перечисление параметров](../api/groupsetting-list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов параметра. |
|[Обновление параметра](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Обновление объекта параметра. |
|[Удаление параметра](../api/groupsetting-delete.md) | Нет | Удаление объекта параметра. |
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
|[Удаление цепочки](../api/group-delete-thread.md) |Нет| Удаление объекта thread.|
|[Вывод acceptedSenders](../api/group-list-acceptedsenders.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей или групп из списка acceptedSenders для данной группы.|
|[Добавление acceptedSender](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| Добавление User или Group в коллекцию acceptedSenders.|
|[Удаление acceptedSender](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| Удаление User или Group из коллекции acceptedSenders.|
|[Список rejectedSenders](../api/group-list-rejectedsenders.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей или групп из списка rejectedSenders для данной группы.|
|[Добавление rejectedSender](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| Добавление User или Group в коллекцию rejectedSenders.|
|[Удаление rejectedSender](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| Удаление нового объекта User или Group из коллекции объектов rejectedSender.|
|[Создание параметра](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. В случае этой операции могут использоваться только шаблоны специально для групп.|
|[Получение параметра](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта параметра. |
|[Перечисление параметров](../api/groupsetting-list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов параметра. |
|[Обновление параметра](../api/groupsetting-update.md) | Нет | Обновление объекта параметра. |
|[Удаление параметра](../api/groupsetting-delete.md) | Нет | Удаление объекта параметра. |
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
|[removeFavorite](../api/group-removefavorite.md)|Нет|Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для групп Office 365.|
|[Перечисление memberOf](../api/group-list-memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп и административных единиц, непосредственным участником которых является пользователь, из свойства навигации **memberOf**.|
|[subscribeByMail](../api/group-subscribebymail.md)|Нет|Задает для свойства isSubscribedByMail значение **true**. Позволяет текущему пользователю получать беседы по электронной почте. Поддерживается только для групп Office 365.|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|Нет|Задает для свойства isSubscribedByMail значение **false**. Отключает получение бесед по электронной почте для текущего пользователя. Поддерживается только для групп Office 365.|
|[resetUnseenCount](../api/group-resetunseencount.md)|Нет|Сброс значений unseenCount до 0 для всех записей, которые текущий пользователь не просматривал со времени последнего посещения. Поддерживается только для групп Office 365.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.|
|autoSubscribeNewMembers|Логическое|Значение по умолчанию: **false**. Указывает, будут ли новые члены группы автоматически подписаны на получение уведомлений по электронной почте. Это свойство можно задать в запросе PATCH для группы. Не задавайте его в первоначальном запросе POST, создающем группу.|
|classification|String|Описывает классификацию для группы (например, незначительное, среднее или значительное влияние на бизнес). Допустимые значения для этого свойства определяются созданием значения [setting](groupsetting.md) ClassificationList на базе [определения шаблона](groupsettingtemplate.md).|
|createdDateTime|DateTimeOffset| Метка времени создания группы. Значение не может изменяться и автоматически заполняться, когда создается группа. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|описание|String|Необязательное описание для группы. |
|displayName|String|Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.|
|groupTypes|Коллекция String| Указывает тип создаваемой группы. Возможные значения: `Unified` Создание группы Office 365, или `DynamicMembership` для динамических групп.  Для всех других группы типов, таких как группы с включенной поддержкой безопасности и групп безопасности с включенной поддержкой электронной почты, это свойство не задано. Поддерживает параметр $filter.|
|id|String|Уникальный идентификатор группы. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|isSubscribedByMail|Boolean|Значение по умолчанию: **true**. Указывает, подписан ли текущий пользователь на получение бесед по электронной почте.|
|mail|String|SMTP-адрес группы, например "serviceadmins@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailEnabled|Boolean|Указывает, включена ли для этой группы поддержка почты. Если для свойства **securityEnabled** также задано значение **true**, это группа безопасности с включенной поддержкой почты. В противном случае это группа рассылки Microsoft Exchange.|
|mailNickname|String|Почтовый псевдоним для группы, уникальный в организации. Это свойство должно быть указано при создании группы. Поддерживает параметр $filter.|
|onPremisesLastSyncDateTime|DateTimeOffset|Указывает время последней синхронизации группы с локальным каталогом. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Поддерживает параметр $filter.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) коллекции| Ошибки при использовании продуктов Майкрософт синхронизации во время подготовки. |
|onPremisesSecurityIdentifier|String|Содержит локальный идентификатор безопасности (SID) для локальной группы, синхронизированной с облаком. Только для чтения. |
|onPremisesSyncEnabled|Логическое|Значение **true** указывает, что эта группа синхронизируется из локального каталога. Значение **false** указывает, что эта группа ранее синхронизировалась из локального каталога, но синхронизация больше не выполняется. Значение **null** указывает, что этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения. Поддерживает параметр $filter.|
|preferredDataLocation|Строка|Расположение предпочитаемый данных для группы. Для получения дополнительных сведений см [OneDrive Online Multi-географически](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|proxyAddresses|Коллекция String| Для выражений фильтра в случае использования многозначных свойств требуется оператор **any**. Только для чтения. Значение NULL не допускается. Поддерживает параметр $filter. |
|renewedDateTime|DateTimeOffset| Метка времени последнего обновления группы. Не может изменяться непосредственно. Обновляется только при выполнении [действия обновления](../api/group-renew.md). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|securityEnabled|Логическое|Указывает, является ли эта группа группой безопасности. Если для свойства **mailEnabled** также задано значение true, это группа безопасности с включенной поддержкой почты. В противном случае это обычная группа безопасности. Для групп Office 365 должно быть задано значение **false**. Поддерживает параметр $filter.|
|unseenCount|Int32|Количество бесед, которые были доставлены один или несколько новых сообщений с момента последнего посетить пользователь выполнил вход в группу.|
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
|events|Коллекция [event](event.md)|События в календаре группы.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для группы. Только для чтения. Допускает значение null.|
|groupLifecyclePolicies|Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)|Коллекция жизненного цикла политик для этой группы. Только для чтения. Допускается значение null.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы, в которых состоит эта группа. Методы HTTP: GET (поддерживается для всех групп). Только для чтения. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)| Пользователи и группы, состоящие в этой группе. Методы HTTP: GET (поддерживается для всех групп), POST (поддерживается для групп Office 365 и групп безопасности, в том числе с включенной поддержкой почты), DELETE (поддерживается для групп Office 365 и групп безопасности). Допускается значение null.|
|onenote|[OneNote](onenote.md)| Только для чтения.|
|owners|Коллекция [directoryObject](directoryobject.md)|Владельцы группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект. Максимальное количество владельцев: 10. Методы HTTP: GET (поддерживается для всех групп), POST (поддерживается для групп Office 365 и групп безопасности, в том числе с включенной поддержкой почты), DELETE (поддерживается для групп Office 365 и групп безопасности). Допускается значение null.|
|photo|[profilePhoto](profilephoto.md)| Фотография профиля группы. |
|photos|Коллекция объектов [profilePhoto](profilephoto.md)| Фотографии профиля, принадлежащие группе. Только для чтения. Допускается значение null.|
|planner|[plannerGroup](plannergroup.md)| Точка входа в ресурс Planner, который может существовать для единой группы.|
|rejectedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым запрещено создавать записи или события календаря в этой группе. Допускается значение null.|
|settings|Коллекция объектов [groupSetting](groupsetting.md)| Только для чтения. Допускается значение null.|
|sites|Коллекция объектов [site](site.md)|Список сайтов SharePoint в этой группе. Для доступа к сайту по умолчанию используйте путь /sites/root.|
|threads|Коллекция [conversationThread](conversationthread.md)| Цепочки бесед группы. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
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
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "acceptedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "conversations",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "rejectedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "classification": "string",
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "string",
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "unseenCount": 1024,
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
