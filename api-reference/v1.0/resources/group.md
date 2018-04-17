# <a name="group-resource-type"></a>Тип ресурса group

Представляет группу Azure Active Directory (Azure AD), которая может быть группой Office 365, группой безопасности или динамической группой. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам с помощью [расширений](../../../concepts/extensibility_overview.md);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](../../../concepts/delta_query_overview.md) (функция [delta](../api/user_delta.md)).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Управление группами**| | |
|[Создание группы](../api/group_post_groups.md) | [group](group.md) |Создание группы. Это может быть группа Office 365, группа безопасности или динамическая группа.|
|[Получение группы](../api/group_get.md) | [group](group.md) |Считывание свойств объекта group.|
|[Список групп](../api/group_list.md) |Коллекция [group](group.md) |Список объектов group и их свойств.|
|[Обновление группы](../api/group_update.md) | Нет |Обновление свойств объекта group. |
|[Удаление группы](../api/group_delete.md) | Нет |Удаление объекта group. |
|[delta](../api/group_delta.md)|Коллекция групп| Получение добавочных изменений для групп. |
|[Перечисление groupLifecyclePolicies](../api/group_list_grouplifecyclepolicies.md) |Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)| Перечисление политик жизненного цикла для групп. |
|[Renew](../api/group_renew.md)|Boolean|Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.|
|[Добавление владельца](../api/group_post_owners.md) |Нет| Добавление владельца группы путем помещения в свойство навигации **owners** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты).|
|[Список владельцев](../api/group_list_owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение владельцев группы из свойства навигации **owners**.|
|[Удаление владельца](../api/group_delete_owners.md) | Нет |Удаление владельца из группы Office 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **owners**.|
|[Добавление члена](../api/group_post_members.md) |Нет| Добавление пользователя или группы в данную группу путем помещения в свойство навигации **members** (поддерживается только для групп безопасности, в том числе с включенной поддержкой почты).|
|[Список членов](../api/group_list_members.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей и групп, являющихся непосредственными членами этой группы, из свойства навигации **members**.|
|[Удаление члена](../api/group_delete_members.md) | Нет |Удаление члена из группы Office 365 или группы безопасности (в том числе с включенной поддержкой почты) с помощью свойства навигации **members**. Вы можете удалять пользователей или другие группы. |
|[checkMemberGroups](../api/group_checkmembergroups.md)|Коллекция строк|Проверка данной группы на членство в списке групп. Это транзитивная функция.|
|[getMemberGroups](../api/group_getmembergroups.md)|Коллекция строк|Возврат всех групп, в которых состоит эта группа. Это транзитивная функция.|
|[getMemberObjects](../api/group_getmemberobjects.md)|Коллекция строк|Возврат всех групп, в которых состоит эта группа. Это транзитивная функция. |
|[Создание параметра](../api/groupsetting_post_groupsettings.md) | [groupSetting](groupsetting.md) |Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. В случае этой операции могут использоваться только шаблоны специально для групп.|
|[Получение параметра](../api/groupsetting_get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта параметра. |
|[Перечисление параметров](../api/groupsetting_list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов параметра. |
|[Обновление параметра](../api/groupsetting_update.md) | [groupSetting](groupsetting.md) | Обновление объекта параметра. |
|[Удаление параметра](../api/groupsetting_delete.md) | Нет | Удаление объекта параметра. |
|**Calendar**| | |
|[Создание события](../api/group_post_events.md) |[event](event.md)| Создание объекта event путем публикации в коллекции объектов event.|
|[Получение события](../api/group_get_event.md) |[event](event.md)|Считывание свойств объекта event.|
|[Перечисление событий](../api/group_list_events.md) |Коллекция [event](event.md)| Получение коллекции объектов event.|
|[Обновление события](../api/group_update_event.md) |Нет|Обновление свойств объекта event.|
|[Удаление события](../api/group_delete_event.md) |Нет|Удаление объекта event.|
|[Список calendarView](../api/group_list_calendarview.md) |Коллекция [event](event.md)| Получение коллекции событий за указанный интервал времени.|
|**Беседы**| | |
|[Создание беседы](../api/group_post_conversations.md) |[conversation](conversation.md)| Создание беседы путем публикации в коллекции объектов conversation.|
|[Получение беседы](../api/group_get_conversation.md) |[conversation](conversation.md)| Считывание свойств объекта conversation.|
|[Перечисление бесед](../api/group_list_conversations.md) |Коллекция [conversation](conversation.md)| Получение коллекции объектов conversation.|
|[Удаление беседы](../api/group_delete_conversation.md) |Нет|Удаление объекта conversation.|
|[Получение цепочки](../api/group_get_thread.md) |[conversationThread](conversationthread.md)| Считывание свойств объекта thread.|
|[Перечисление цепочек](../api/group_list_threads.md) |Коллекция [conversationThread](conversationthread.md)| Получение всех цепочек группы.|
|[Обновление цепочки](../api/group_update_thread.md) |Нет| Обновление свойств объекта thread.|
|[Удаление цепочки](../api/group_delete_thread.md) |Нет| Удаление объекта thread.|
|[Вывод acceptedSenders](../api/group_list_acceptedsenders.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей или групп из списка acceptedSenders для данной группы.|
|[Добавление acceptedSender](../api/group_post_acceptedsenders.md) |[directoryObject](directoryobject.md)| Добавление User или Group в коллекцию acceptedSenders.|
|[Удаление acceptedSender](../api/group_delete_acceptedsenders.md) |[directoryObject](directoryobject.md)| Удаление User или Group из коллекции acceptedSenders.|
|[Список rejectedSenders](../api/group_list_rejectedsenders.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей или групп из списка rejectedSenders для данной группы.|
|[Добавление rejectedSender](../api/group_post_rejectedsenders.md) |[directoryObject](directoryobject.md)| Добавление User или Group в коллекцию rejectedSenders.|
|[Удаление rejectedSender](../api/group_delete_rejectedsenders.md) |[directoryObject](directoryobject.md)| Удаление нового объекта User или Group из коллекции объектов rejectedSender.|
|[Создание параметра](../api/groupsetting_post_groupsettings.md) | [groupSetting](groupsetting.md) |Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне. В случае этой операции могут использоваться только шаблоны специально для групп.|
|[Получение параметра](../api/groupsetting_get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта параметра. |
|[Перечисление параметров](../api/groupsetting_list.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов параметра. |
|[Обновление параметра](../api/groupsetting_update.md) | Нет | Обновление объекта параметра. |
|[Удаление параметра](../api/groupsetting_delete.md) | Нет | Удаление объекта параметра. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension_get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](../../../concepts/extensibility_schema_groups.md) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Другие ресурсы групп**| | |
|[Перечисление фотографий](../api/group_list_photos.md) |Коллекция объектов [profilePhoto](photo.md)| Получение коллекции фотографий профиля для группы.|
|[Перечисление планов](../api/plannergroup_list_plans.md) |Коллекция объектов [plannerPlan](plannerPlan.md)| Получение планов, принадлежащих группе.|
|**Параметры пользователя**| | |
|[addFavorite](../api/group_addfavorite.md)|Нет|Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.|
|[removeFavorite](../api/group_removefavorite.md)|Нет|Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для групп Office 365.|
|[Перечисление memberOf](../api/group_list_memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп и административных единиц, непосредственным участником которых является пользователь, из свойства навигации **memberOf**.|
|[subscribeByMail](../api/group_subscribebymail.md)|Нет|Задает для свойства isSubscribedByMail значение **true**. Позволяет текущему пользователю получать беседы по электронной почте. Поддерживается только для групп Office 365.|
|[unsubscribeByMail](../api/group_unsubscribebymail.md)|Нет|Задает для свойства isSubscribedByMail значение **false**. Отключает получение бесед по электронной почте для текущего пользователя. Поддерживается только для групп Office 365.|
|[resetUnseenCount](../api/group_resetunseencount.md)|Нет|Сброс значений unseenCount до 0 для всех записей, которые текущий пользователь не просматривал со времени последнего посещения. Поддерживается только для групп Office 365.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowExternalSenders|Логическое|Значение по умолчанию: **false**. Указывает, могут ли пользователи за пределами организации отправлять сообщения в группу.|
|autoSubscribeNewMembers|Логическое|Значение по умолчанию: **false**. Указывает, будут ли новые члены группы автоматически подписаны на получение уведомлений по электронной почте. Это свойство можно задать в запросе PATCH для группы. Не задавайте его в первоначальном запросе POST, создающем группу.|
|classification|String|Описывает классификацию для группы (например, незначительное, среднее или значительное влияние на бизнес). Допустимые значения для этого свойства определяются созданием значения [setting](groupsetting.md) ClassificationList на базе [определения шаблона](groupsettingtemplate.md).|
|createdDateTime|DateTimeOffset| Метка времени создания группы. Значение не может изменяться и автоматически заполняться, когда создается группа. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|description|String|Необязательное описание для группы. |
|displayName|String|Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.|
|groupTypes|Коллекция строк| Указывает тип создаваемой группы. Возможные значения: **Unified** для создания группы Office 365 или **DynamicMembership** для создания динамических групп.  Для остальных типов групп, таких как группы с включенной поддержкой безопасности и группы безопасности с включенной поддержкой электронной почты, это свойство не задается. Поддерживает параметр $filter.|
|id|String|Уникальный идентификатор группы. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|isSubscribedByMail|Логическое|Значение по умолчанию: **true**. Указывает, подписан ли текущий пользователь на получение бесед по электронной почте.|
|почта|String|SMTP-адрес группы, например "serviceadmins@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailEnabled|Boolean|Указывает, включена ли для этой группы поддержка почты. Если для свойства **securityEnabled** также задано значение **true**, это группа безопасности с включенной поддержкой почты. В противном случае это группа рассылки Microsoft Exchange.|
|mailNickname|String|Почтовый псевдоним для группы, уникальный в организации. Это свойство должно быть указано при создании группы. Поддерживает параметр $filter.|
|onPremisesLastSyncDateTime|DateTimeOffset|Указывает время последней синхронизации группы с локальным каталогом. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Поддерживает параметр $filter.|
|onPremisesSecurityIdentifier|String|Содержит локальный идентификатор безопасности (SID) для локальной группы, синхронизированной с облаком. Только для чтения. |
|onPremisesSyncEnabled|Логическое|Значение **true** указывает, что эта группа синхронизируется из локального каталога. Значение **false** указывает, что эта группа ранее синхронизировалась из локального каталога, но синхронизация больше не выполняется. Значение **null** указывает, что этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения. Поддерживает параметр $filter.|
|proxyAddresses|Коллекция строк| Для выражений фильтра в случае использования многозначных свойств требуется оператор **any**. Только для чтения. Значение NULL не допускается. Поддерживает параметр $filter. |
|renewedDateTime|DateTimeOffset| Метка времени последнего обновления группы. Не может изменяться непосредственно. Обновляется только при выполнении [действия обновления](../api/group_renew.md). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|securityEnabled|Логическое|Указывает, является ли эта группа группой безопасности. Если для свойства **mailEnabled** также задано значение true, это группа безопасности с включенной поддержкой почты. В противном случае это обычная группа безопасности. Для групп Office 365 должно быть задано значение **false**. Поддерживает параметр $filter.|
|unseenCount|Int32|Количество записей, не просмотренных текущим пользователем с момента его последнего посещения.|
|visibility|String| Определяет видимость группы Office 365. Возможные значения: **Private** (частная), **Public** (общедоступная) или пустое значение (оно обрабатывается как **Public**).|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|acceptedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым разрешено создавать записи или события календаря в этой группе. Если этот список не пуст, то добавлять записи разрешено только перечисленным в нем пользователям и группам.|
|calendar|[calendar](calendar.md)|Календарь группы. Только для чтения.|
|calendarView|Коллекция [event](event.md)|Представление календаря. Только для чтения.|
|conversations|Коллекция [conversation](conversation.md)|Беседы группы.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Пользователь или приложение, создавшие группу. ПРИМЕЧАНИЕ. Это значение не задается, если пользователь является администратором. Только для чтения.|
|drive|[drive](drive.md)|Диск группы. Только для чтения.|
|events|Коллекция [event](event.md)|События в календаре группы.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для группы. Только для чтения. Допускает значение null.|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы, в которых состоит эта группа. Методы HTTP: GET (поддерживается для всех групп). Только для чтения. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)| Пользователи и группы, состоящие в этой группе. Методы HTTP: GET (поддерживается для всех групп), POST (поддерживается для групп Office 365 и групп безопасности, в том числе с включенной поддержкой почты), DELETE (поддерживается для групп Office 365 и групп безопасности). Допускается значение null.|
|onenote|[OneNote](onenote.md)| Только для чтения.|
|owners|Коллекция [directoryObject](directoryobject.md)|Владельцы группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект. Максимальное количество владельцев: 10. Методы HTTP: GET (поддерживается для всех групп), POST (поддерживается для групп Office 365 и групп безопасности, в том числе с включенной поддержкой почты), DELETE (поддерживается для групп Office 365 и групп безопасности). Допускается значение null.|
|photo|[profilePhoto](profilephoto.md)| Фотография профиля группы. |
|photos|Коллекция объектов [profilePhoto](profilephoto.md)| Фотографии профиля, принадлежащие группе. Только для чтения. Допускается значение null.|
|planner|[planner](planner.md)| Точка входа в ресурс Planner, который может существовать для единой группы.|
|rejectedSenders|Коллекция [directoryObject](directoryobject.md)|Список пользователей или групп, которым запрещено создавать записи или события календаря в этой группе. Допускается значение null.|
|settings|Коллекция объектов [groupSetting](groupsetting.md)| Только для чтения. Допускается значение null.|
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
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
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
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
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

- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](../../../concepts/extensibility_open_users.md)
- [Добавление пользовательских данных в группы с помощью расширений схемы](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
