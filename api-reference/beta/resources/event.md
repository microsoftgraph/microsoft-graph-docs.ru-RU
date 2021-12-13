---
title: Тип ресурса event
description: Событие в календаре.
author: harini84
ms.localizationpriority: high
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8f4b7b53ef18e5e777b0b154b00e4473ba0cce49
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424730"
---
# <a name="event-resource-type"></a>Тип ресурса event

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление событий](../api/user-list-events.md)|Коллекция [Event](event.md) |Получение списка объектов [event](../resources/event.md) в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих рядах.|
|[Создание события](../api/user-post-events.md) |[event](event.md)| Создание события путем записи в коллекцию экземпляров.|
|[Получение события](../api/event-get.md) | [event](event.md) |Считывание свойств и отношений объекта event.|
|[Обновление](../api/event-update.md) | [event](event.md)   |Обновление объекта event. |
|[Удаление](../api/event-delete.md) | Нет |Удаление объекта event. |
|[delta](../api/event-delta.md)|Коллекция объектов [event](event.md)|Получение списка событий, которые были добавлены в **calendarView** (диапазон событий) основного календаря пользователя, обновлены в нем или удалены из него.|
|[forward](../api/event-forward.md)|Нет|Позволяет организатору или участнику собрания пересылать приглашение на собрание новому получателю.|
|[cancel](../api/event-cancel.md) | Нет | Отправка сообщения об отмене от организатора всем участникам и отмена указанного собрания. |
|[accept](../api/event-accept.md)|Нет|Принятие указанного события в календаре пользователя.|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|Нет|Принятие под вопросом указанного события в календаре пользователя.|
|[decline](../api/event-decline.md)|Нет|Отклонение приглашения на указанное событие в календаре пользователя.|
|[dismissReminder](../api/event-dismissreminder.md)|Нет|Отключение напоминания для указанного события в календаре пользователя.|
|[snoozeReminder](../api/event-snoozereminder.md)|Нет|Откладывание напоминания для указанного события в календаре пользователя на другое время.|
|[Перечисление экземпляров](../api/event-list-instances.md) |Коллекция [Event](event.md)| Получение коллекции объектов Event.|
|**Вложения**| | |
|[Список вложений](../api/event-list-attachments.md) |Коллекция [Attachment](attachment.md)| Получение всех вложений, добавленных к данным о событии.|
|[Добавление вложения](../api/event-post-attachments.md) |[Attachment](attachment.md)| Добавление нового вложения к данным о событии путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[event](event.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем событии.   |
|[Получение события с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [event](event.md) | Получение событий, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [event](event.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем событии.  |
|[Получение события с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [event](event.md) | Получение события, которое содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowNewTimeProposals| Boolean | Значение `true`, если организатор собрания разрешает приглашенным предлагать новое время при ответе, в противном случае — `false`. Необязательный аргумент. Значение по умолчанию: `true`. |
|attendees|Коллекция [Attendee](attendee.md)|Коллекция участников события.|
|body|[ItemBody](itembody.md)|Текст сообщения, связанного с событием. В формате HTML или текстовом формате.|
|bodyPreview|Строка|Предварительный просмотр сообщения, связанного с событием. В текстовом формате.|
|cancelledOccurrences|Коллекция String|Содержит значения свойства **occurrenceId** отмененных экземпляров в повторяющемся ряду, если событие является основным в этом ряду. Отмененные экземпляры в повторяющемся ряду называются cancelledOccurences.<br><br>Возвращается только для $select в операции [Get](../api/event-get.md), в которой указывается идентификатор основного события в ряду (т. е. значение свойства seriesMasterId).|
|categories|Коллекция String|Категории, связанные с событием. Каждая категория соответствует свойству **displayName** объекта [outlookCategory](outlookcategory.md), определенного для пользователя.|
|changeKey|String|Указывает версию объекта события. При каждом изменении события также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|end|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс завершения события. По умолчанию время завершения указано в формате UTC.|
|exceptionOccurrences|Коллекция [event](event.md)|Содержит значения свойства **id** экземпляров событий, которые являются исключениями в повторяющемся ряду.<br>Исключения могут отличаться от других вхождений в повторяющемся ряду, таких как тема, время начала или окончания и участники. Исключения не включают отмененные вхождения.<br><br>Возвращается только для $select и $expand в операции [GET](../api/event-get.md), в которой указывается идентификатор основного события в ряду (т. е. значение свойства seriesMasterId).|
|hasAttachments|Boolean|Задайте значение true, если у события есть вложения.|
|hideAttendees|Boolean|Если присвоено значение `true`, каждый участник видит только себя в приглашении на собрание и списке собрания **Отслеживание**. Значение по умолчанию: false.|
|id|String| Уникальный идентификатор события. [!INCLUDE [outlook-beta-id](../../includes/outlook-immutable-id.md)] С учетом регистра и только для чтения.|
|importance|String|Важность события. Возможные значения: `low`, `normal`, `high`.|
|isAllDay|Boolean|Задайте значение true, если событие длится весь день. Если присвоено значение true, независимо от длительности события (один или несколько дней) время его начала и окончания должно быть установлено на полночь в одном часовом поясе.|
|isCancelled|Boolean|Задайте значение true, если событие отменено.|
|isDraft|Логический|Присвоено значение true, если пользователь обновил собрание в Outlook, но не отправил обновления участникам. Присвоено значение false, если все изменения отправлены или событие является встречей без участников.|
|isOnlineMeeting|Boolean| `True`, если событие содержит информацию о собрании по сети (т. е. **onlineMeeting** указывает на ресурс [onlineMeetingInfo](onlinemeetinginfo.md)), в противном случае — `false`. Значение по умолчанию `false` (**onlineMeeting** со значением `null`). Необязательный аргумент.<br> После настройки **isOnlineMeeting** на `true` Microsoft Graph инициализирует **onlineMeeting**. Outlook будет игнорировать любые последующие изменения **isOnlineMeeting**, и собрание останется доступным по сети. |
|isOrganizer|Boolean|Присвоено значение true, если владелец календаря (указанный свойством **owner** объекта [calendar](calendar.md)) является организатором события (определятся свойством **organizer** объекта **event**). Это также применимо, если делегат организовал событие от имени владельца.|
|isReminderOn|Boolean|Задайте значение true, если установлено напоминание пользователю о событии.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|location|[Location](location.md)|Место проведения события.|
|locations|Коллекция [Location](location.md)|Места проведения события или участия в нем. Свойства **location** и **locations** всегда совпадают друг с другом. Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**. |
|occurrenceId|String|Идентификатор вхождения в повторяющемся ряду событий. Значение NULL, если событие не является частью повторяющегося ряда.<br><br>Формат значения свойства — OID.{seriesMasterId-value}.{occurrence-start-date}. Часовым поясом для {occurrence-start-date} является свойство recurrenceTimeZone, определенное для соответствующего [recurrenceRange](recurrencerange.md).<br><br>Это свойство может определять вхождение в повторяющемся ряду, в том числе измененное или отмененное. Это свойство можно использовать для выполнения всех операций, которые поддерживаются вхождениями в повторяющемся ряду.|
|onlineMeeting|[OnlineMeetingInfo](onlinemeetinginfo.md)| Сведения, необходимые участнику, чтобы присоединиться к собранию по сети. Значение по умолчанию — NULL. Только для чтения. <br>После настройки свойств **isOnlineMeeting** и **onlineMeetingProvider** для разрешения собрания по сети Microsoft Graph инициализирует **onlineMeeting**. После завершения настройки собрание останется доступным по сети, и вы не сможете изменить свойства **isOnlineMeeting**, **onlineMeetingProvider** и **onlneMeeting**.|
|onlineMeetingProvider|onlineMeetingProviderType| Представляет поставщика службы собраний по сети. По умолчанию **onlineMeetingProvider** — `unknown`. Возможные значения: `unknown`, `teamsForBusiness`, `skypeForBusiness` и `skypeForConsumer`. Необязательное свойство. <br> После настройки **onlineMeetingProvider** Microsoft Graph инициализирует **onlineMeeting**. После этого вы не сможете изменить **onlineMeetingProvider** и собрание останется доступным по сети. |
|onlineMeetingUrl|String|URL-адрес собрания. Свойство будет задано только в том случае, если организатор определяет в Outlook, что событие является собранием по сети, например в Skype. Только для чтения.<br>Чтобы получить доступ к URL-адресу и присоединиться к собранию по сети, воспользуйтесь **joinUrl**, который предоставляется через свойство **event**, **onlineMeeting**. В будущем свойство **onlineMeetingUrl** будет упразднено. |
|organizer|[Recipient](recipient.md)|Организатор события.|
|originalEndTimeZone|String|Часовой пояс завершения события, указанный при его создании. Значение `tzone://Microsoft/Custom` указывает, что в классическом приложении Outlook задан традиционный пользовательский часовой пояс.|
|originalStart|DateTimeOffset|Представляет время начала события, когда оно изначально создается как вхождение или исключение в повторяющемся ряду. Это свойство не возвращается для событий, которые являются одиночными экземплярами. Сведения времени и даты представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|originalStartTimeZone|Строка|Часовой пояс начала события, указанный при его создании. Значение `tzone://Microsoft/Custom` указывает, что в классическом приложении Outlook задан традиционный пользовательский часовой пояс.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|Расписание повторения события.|
|reminderMinutesBeforeStart|Int32|Позволяет указать, за сколько минут до начала события появляется напоминание.|
|responseRequested|Логический|По умолчанию используется значение true, означающее, что организатор запрашивает у приглашенного отправку ответа для события.|
|responseStatus|[ResponseStatus](responsestatus.md)|Указывает тип отклика, отправленного в ответ на сообщение о событии.|
|sensitivity|String| Возможные значения: `normal`, `personal`, `private`, `confidential`.|
|seriesMasterId|String|Идентификатор для элемента образца повторяющегося ряда, если это событие входит в повторяющийся ряд.|
|showAs|String|Отображаемое состояние. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|start|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс начала события. По умолчанию время начала указано в формате UTC.|
|subject|String|Текст в строке темы сообщения о событии.|
|transactionId|Строка|Настраиваемый идентификатор, указанный клиентским приложением серверу во избежание лишних операций [POST](../api/calendar-post-events.md) в том случае, если клиент попробует снова создать одно и то же событие. Это полезно в тех случаях, когда из-за плохого сетевого подключения клиент отключается, не успев получить от сервера ответ на предыдущий запрос клиента на создание события. После того, как при создании события вы настроили **transactionId**, вы можете изменить **transactionId** в последующем обновлении. Это свойство возвращается только в полезных данных ответа, если такая настройка была сделана в приложении. Необязательное свойство.|
|type|String|Тип события. Возможные значения: `singleInstance`, `occurrence`, `exception`, `seriesMaster`. Только для чтения|
|uid|String|Уникальный идентификатор для событий календаря. В случае повторяющихся событий для главного события серии и всех его повторений (в том числе исключений) используется одно и то же значение. Это свойство заменит текущее свойство iCalUid, определенное в [ресурсе event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), для которого в каждом экземпляре серии задавались разные значения.|
|webLink|String|URL-адрес для открытия события в Outlook в Интернете.<br/><br/>Outlook в Интернете открывает это событие в браузере, если выполнен вход в почтовый ящик. В противном случае Outlook в Интернете предлагает выполнить вход.<br/><br/>Доступ к этому URL-адресу невозможно получить из элемента iFrame.|

> [!NOTE]
> Свойство **webLink** указывает URL-адрес, по которому можно открыть событие только в более ранних версиях Outlook в Интернете. Ниже представлен формат URL-адреса, где _{event-id}_ — это _**зашифрованное в виде URL-адреса**_ значение свойства **id**.
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
|attachments|Коллекция [Attachment](attachment.md)|Коллекция вложений [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md) и [referenceAttachment](referenceattachment.md)для события. Свойство навигации. Только для чтения. Допускается значение null.|
|calendar|[Calendar](calendar.md)|Календарь, который содержит событие. Свойство навигации. Только для чтения.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для события. Допускается значение null.|
|instances|Коллекция [Event](event.md)|Вхождения в повторяющемся ряду, если событие является основным в ряду. Это свойство включает вхождения, которые являются частью расписания повторения, и исключения, которые были изменены, но не включает повторения, которые были отменены в ряду. Свойство навигации. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для события. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для события. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
   "keyProperty": "id",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.event"
}-->

```json
{
  "allowNewTimeProposals": "Boolean",
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "cancelledOccurrences":["string"],
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "exceptionOccurrences":["microsoft.graph.event"],
  "hasAttachments": true,
  "hideAttendees": false,
  "uid": "string",
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
  "occurrenceId":"string",
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
  "type": "String",
  "webLink": "string",

  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }]
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
<!--
{
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
