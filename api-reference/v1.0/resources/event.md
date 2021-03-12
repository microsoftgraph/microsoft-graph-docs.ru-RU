---
title: Тип ресурса event
description: Событие в календаре.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c06c2db99189303572e48017469b5511a2fd592b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722071"
---
# <a name="event-resource-type"></a>Тип ресурса event

Пространство имен: microsoft.graph

Событие в календаре ресурса [user](user.md) или стандартный календарь для ресурса [group](group.md), представляющего группу Microsoft 365.

Максимальное количество участников в ресурсе **event** и максимальное количество получателей в ресурсе [eventMessage](eventmessage.md), отправленном из почтового ящика Exchange Online, составляет 500. Дополнительные сведения см. в разделе [Ограничения на отправку](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/event-delta.md)).

> **Примечание.** Существует несколько незначительных различий в способе взаимодействия с календарями пользователей, календарями групп и их событиями:

- В ресурсе [calendarGroup](calendargroup.md) можно упорядочить только календари пользователей.
- Объекты [attachment](attachment.md) можно добавлять только в события календарей пользователей, но не в события календарей групп.
- Outlook автоматически принимает все приглашения на собрания от имени группы. Приглашения на собрания можно [принять](../api/event-accept.md), [принять под вопросом](../api/event-tentativelyaccept.md) или [отклонить](../api/event-decline.md) только в календарях _пользователя_.
- Outlook не поддерживает напоминания о событиях группы. [Напоминание](reminder.md) можно [отложить](../api/event-snoozereminder.md) или [отключить](../api/event-dismissreminder.md) только для календарей _пользователя_.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление событий](../api/user-list-events.md)|Коллекция [event](event.md) |Получение списка объектов [event](../resources/event.md) в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих сериях.|
|[Создание события](../api/user-post-events.md) |[event](event.md)| Создание события путем записи в коллекцию экземпляров.|
|[Получение события](../api/event-get.md) | [event](event.md) |Считывание свойств и отношений объекта event.|
|[Обновление](../api/event-update.md) | [event](event.md) |Обновление объекта event. |
|[Удаление](../api/event-delete.md) | Нет |Удаление объекта event. |
|[delta](../api/event-delta.md)|Коллекция объектов [event](event.md)|Получение списка событий, которые были добавлены в **calendarView** (диапазон событий) основного календаря пользователя, обновлены в нем или удалены из него.|
|[forward](../api/event-forward.md)| Нет |Позволяет организатору или участнику собрания пересылать приглашение на собрание новому получателю.|
|[cancel](../api/event-cancel.md) | Нет | Отправка сообщения об отмене от организатора всем участникам и отмена указанного собрания. |
|[accept](../api/event-accept.md)|Нет|Принятие указанного события в календаре пользователя.|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|Нет|Принятие под вопросом указанного события в календаре пользователя.|
|[decline](../api/event-decline.md)|Нет|Отклонение приглашения на указанное событие в календаре пользователя.|
|[dismissReminder](../api/event-dismissreminder.md)|Нет|Отключение напоминания для указанного события в календаре пользователя.|
|[snoozeReminder](../api/event-snoozereminder.md)|Нет|Откладывание напоминания для указанного события в календаре пользователя на другое время.|
|[Перечисление экземпляров](../api/event-list-instances.md) |Коллекция [event](event.md)| Получение экземпляров (повторов) события для заданного диапазона времени. Если событие относится к типу `SeriesMaster`, возвращаются экземпляры и исключения события для указанного диапазона времени.|
|**Вложения**| | |
|[Список вложений](../api/event-list-attachments.md) |Коллекция [attachment](attachment.md) | Получение всех вложений, добавленных к данным о событии.|
|[Добавление вложения](../api/event-post-attachments.md) |[attachment](attachment.md)| Добавление нового вложения к данным о событии путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объекта или объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[event](event.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем событии.   |
|[Получение события с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [event](event.md) | Получение событий, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [event](event.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем событии.  |
|[Получение события с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [event](event.md) | Получение события, которое содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowNewTimeProposals| Boolean | Значение `True`, если организатор собрания разрешает приглашенным предлагать новое время при ответе, в противном случае — `false`. Необязательный параметр. Значение по умолчанию: `true`. |
|attendees|Коллекция объектов [attendee](attendee.md)|Коллекция участников события.|
|body|[itemBody](itembody.md)|Текст сообщения, связанного с событием. В формате HTML или текстовом формате.|
|bodyPreview|String|Предварительный просмотр сообщения, связанного с событием. В текстовом формате.|
|categories|Коллекция String|Категории, связанные с событием.|
|changeKey|String|Указывает версию объекта события. При каждом изменении события также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс завершения события. По умолчанию время завершения указано в формате UTC.|
|hasAttachments|Boolean|Задайте значение true, если у события есть вложения.|
|hideAttendees|Boolean|Если присвоено значение `true`, каждый участник видит только себя в приглашении на собрание и списке собрания **Отслеживание**. Значение по умолчанию: false.|
|iCalUId|String|Уникальный идентификатор для события в календарях. Этот идентификатор отличается для каждого вхождения повторяющегося ряда. Только для чтения.|
|id|String| Только для чтения.|
|importance|importance|Важность события. Допустимые значения: `low`, `normal`, `high`.|
|isAllDay|Boolean|Задайте значение true, если событие длится весь день.|
|isCancelled|Boolean|Задайте значение true, если событие отменено.|
|isDraft|Логический|Присвоено значение true, если пользователь обновил собрание в Outlook, но не отправил обновления участникам. Присвоено значение false, если все изменения отправлены или событие является встречей без участников.|
|isOnlineMeeting|Boolean| `True`, если это событие содержит информацию о собраниях по сети; в противном случае — `false`. Значение по умолчанию: false. Необязательный.|
|isOrganizer|Boolean|Присвоено значение true, если владелец календаря (указанный свойством **owner** объекта [calendar](calendar.md)) является организатором события (определятся свойством **organizer** объекта **event**). Это также применимо, если делегат организовал событие от имени владельца.|
|isReminderOn|Boolean|Задайте значение true, если установлено напоминание пользователю о событии.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|location|[location](location.md)|Место проведения события.|
|locations|Коллекция [location](location.md)|Места проведения мероприятия или участия в нем. Свойства **location** и **locations** всегда совпадают друг с другом. Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**. |
|onlineMeeting|[OnlineMeetingInfo](onlinemeetinginfo.md)| Сведения, необходимые участнику, чтобы присоединиться к собранию по сети. Только для чтения.|
|onlineMeetingProvider|onlineMeetingProviderType| Представляет поставщика службы собраний по сети. Возможные значения: `teamsForBusiness`, `skypeForBusiness` и `skypeForConsumer`. Необязательный. |
|onlineMeetingUrl|String|URL-адрес для собрания по сети. Это свойство задается, только если организатор сделал мероприятие собранием по сети, например собранием Skype. Только для чтения.|
|organizer|[recipient](recipient.md)|Организатор события.|
|originalEndTimeZone|String|Часовой пояс завершения, указанный при создании события. Значение `tzone://Microsoft/Custom` указывает, что традиционный часовой пояс был задан в классическом приложении Outlook.|
|originalStart|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|originalStartTimeZone|String|Часовой пояс начала события, указанный при его создании. Значение `tzone://Microsoft/Custom` указывает, что в классическом приложении Outlook задан традиционный пользовательский часовой пояс. |
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Расписание повторения события.|
|reminderMinutesBeforeStart|Int32|Позволяет указать, за сколько минут до начала события появляется напоминание.|
|responseRequested|Логический|По умолчанию используется значение true, означающее, что организатор запрашивает у приглашенного отправку ответа для события.|
|responseStatus|[responseStatus](responsestatus.md)|Указывает тип отклика, отправленного в ответ на сообщение о событии.|
|sensitivity|sensitivity| Допустимые значения: `normal`, `personal`, `private`, `confidential`.|
|seriesMasterId|String|Идентификатор для элемента образца повторяющегося ряда, если это событие входит в повторяющийся ряд.|
|showAs|freeBusyStatus|Отображаемое состояние. Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|начать|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс начала события. По умолчанию время начала указано в формате UTC.|
|subject|String|Текст в строке темы сообщения о событии.|
|transactionId |String |Настраиваемый идентификатор, указанный клиентским приложением серверу во избежание лишних операций POST в том случае, если клиент попробует снова создать одно и то же событие. Это полезно в тех случаях, когда из-за плохого сетевого подключения клиент отключается, не успев получить от сервера ответ на предыдущий запрос клиента на создание события. После того, как при создании события вы настроили **transactionId**, вы можете изменить **transactionId** в последующем обновлении. Это свойство возвращается только в полезных данных ответа, если такая настройка была сделана в приложении. Необязательное свойство.|
|type|eventType|Тип события. Допустимые значения: `singleInstance`, `occurrence`, `exception`, `seriesMaster`. Только для чтения.|
|webLink|String|URL-адрес для открытия события в Outlook в Интернете.<br/><br/>Outlook в Интернете открывает это событие в браузере, если выполнен вход в почтовый ящик. В противном случае Outlook в Интернете предлагает выполнить вход.<br/><br/>Доступ к этому URL-адресу невозможно получить из элемента iFrame.|

> [!NOTE]
> Свойство **webLink** указывает URL-адрес, по которому можно открыть событие только в более ранних версиях Outlook в Интернете. Ниже представлены форматы URL-адреса, где _{event-id}_ — это _**зашифрованное в виде URL-адреса**_ значение свойства **id**.
>
> * Для рабочих или учебных учетных записей: `https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`
>
> * Для учетных записей Майкрософт: `https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`
>
> Чтобы открыть событие в текущей версии Outlook в Интернете, преобразуйте URL-адрес в один из следующих форматов и используйте этот URL-адрес для открытия события:
>
> * Для рабочих или учебных учетных записей: `https://outlook.office365.com/calendar/item/{event-id}`
>
> * Для учетных записей Майкрософт: `https://outlook.live.com/calendar/item/{event-id}`


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Коллекция вложений [fileAttachment](fileattachment.md) и [itemAttachment](itemattachment.md) для события. Свойство навигации. Только для чтения. Допускается значение null.|
|календарь|[calendar](calendar.md)|Календарь, который содержит событие. Свойство навигации. Только для чтения.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для события. Только для чтения. Допускается значение null.|
|instances|Коллекция [event](event.md)|Экземпляры события. Свойство навигации. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для события. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для события. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.event",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
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
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "instances",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowNewTimeProposals": "Boolean",
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "hideAttendees": false,
  "iCalUId": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isDraft": false,
  "isOnlineMeeting": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "onlineMeeting": {"@odata.type": "microsoft.graph.onlineMeetingInfo"},
  "onlineMeetingProvider": "string",
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "transactionId": "string",
  "type": "String",
  "webLink": "string",

  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```


## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью запроса изменений](/graph/delta-query-overview)
- [Получение добавочных изменений для событий в папке](/graph/delta-query-events)
- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

