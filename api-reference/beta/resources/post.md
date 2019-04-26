---
title: Тип ресурса Post
description: Представляет отдельный элемент POST в объекте Конверстаионсреад.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: abfd2b19681b9821377830f1696fa6f754afd711
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344242"
---
# <a name="post-resource-type"></a>Тип ресурса Post

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельный элемент POST в объекте [конверстаионсреад](conversationthread.md) .

Хотя явно создать экземпляр post невозможно, он будет создан в результате выполнения любого из указанных ниже действий.

* [Добавление ответа к существующей публикации](../api/post-reply.md). 
* [Добавление ответа к существующей цепочке](../api/conversationthread-reply.md). 
* [Создание цепочки в новой беседе](../api/group-post-threads.md).
* [Создание беседы](../api/group-post-conversations.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.post"
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|Содержимое публикации. Это свойство используется по умолчанию. Это свойство может иметь значение null.|
|categories|Коллекция String|Категории, сопоставленные с публикацией. Каждая категория соответствует свойству **DisplayName** объекта [outlookCategory](outlookcategory.md) , определенного для пользователя.|
|changeKey|Строка|Указывает версию публикации. При каждом изменении публикации также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|conversationId|String|Уникальный идентификатор беседы. Только для чтения.|
|conversationThreadId|String|Уникальный идентификатор цепочки беседы. Только для чтения.|
|createdDateTime|DateTimeOffset|Указывает, когда была создана публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|from|[recipient](recipient.md)|Используется в сценариях делегированного доступа. Указывает, кто опубликовал сообщение от имени другого пользователя. Это свойство используется по умолчанию.|
|hasAttachments|Boolean|Указывает, есть ли в публикации хотя бы одно вложение. Это свойство используется по умолчанию.|
|id|String| Только для чтения.|
|importance | String | Важность записи группы: `low`, `normal`,. `high` |
|lastModifiedDateTime|DateTimeOffset|Указывает дату и время последнего изменения публикации. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|НевпартиЦипантс|Коллекция объектов [recipient](recipient.md)|Участники беседы, которые были добавлены в цепочку в рамках этой публикации.|
|receivedDateTime|DateTimeOffset|Указывает, когда была получена публикация. Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|sender|[recipient](recipient.md)|Содержит электронный адрес отправителя. Если получатель не указан, то в качестве значения Sender используется адрес пользователя, прошедшего проверку подлинности. Это свойство используется по умолчанию.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [Attachment](attachment.md)|Коллекция вложений [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md)и [referenceAttachment](referenceattachment.md) для POST. Только для чтения. Допускает значение null.|
|extensions|Коллекция [Extension](extension.md)|Коллекция открытых расширений, определенных для записи. Только для чтения. Допускает значение null.|
|Инреплито|[Post](post.md)|Предыдущая запись, на которую отвечает эта запись, находится в [conversationThread](conversationthread.md). Только для чтения.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для публикации. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для публикации. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Вывод списка публикаций](../api/conversationthread-list-posts.md) | [post](post.md) |Получение публикаций из указанной цепочки. |
|[Получение публикации](../api/post-get.md) | [post](post.md) |Получение свойств и связей публикации в указанной цепочке.|
|[Ответ](../api/post-reply.md)|Нет|Ответ на публикацию и добавление новой публикации в указанную цепочку беседы группы.|
|[Переадресация](../api/post-forward.md)|Нет|Переадресация публикации получателю.|
|**Вложения**| | |
|[Список вложений](../api/post-list-attachments.md) |Коллекция [attachment](attachment.md) | Получает все вложения для экземпляра post.|
|[Добавление вложения](../api/post-post-attachments.md) |[attachment](attachment.md)| Добавление вложения в публикацию. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[post](post.md)  |Создание одного или нескольких расширенных свойств с одним значением в новой или существующей публикации.   |
|[Получение публикации с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [post](post.md) | Получение публикаций, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [post](post.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новой или существующей публикации.  |
|[Получение публикации с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [post](post.md) | Получение публикации, которая содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
