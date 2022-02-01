---
title: тип ресурса serviceUpdateMessage
description: Представляет объявления об изменениях в службе.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 81d3524855daf6138baa61388b9d853faefec5f6
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291248"
---
# <a name="serviceupdatemessage-resource-type"></a>тип ресурса serviceUpdateMessage

Пространство имен: microsoft.graph

Представляет объявления об изменениях в службе.

Представляет такие объявления, как основные обновления, новые функции в продукте; например, публикация нового SharePoint.

Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceUpdateMessage](../api/serviceupdatemessage-get.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md)|Извлечение свойств и связей объекта [serviceUpdateMessage](../resources/serviceupdatemessage.md) . |
|[markRead](../api/serviceupdatemessage-markread.md)|Логическое|Пометить список [serviceUpdateMessages](../resources/serviceupdatemessage.md) в качестве чтения для подписанного пользователя.|
|[markUnread](../api/serviceupdatemessage-markunread.md)|Логическое|Пометить список [serviceUpdateMessages](../resources/serviceupdatemessage.md) как непрочитанные **для** подписанного пользователя.|
|[архив](../api/serviceupdatemessage-archive.md)|Логический|Архивировать список [serviceUpdateMessages](../resources/serviceupdatemessage.md) для подписанного пользователя.|
|[unarchive](../api/serviceupdatemessage-unarchive.md)|Логическое|Unarchive a list of [serviceUpdateMessages](../resources/serviceupdatemessage.md) for the signed in user.|
|[избранное](../api/serviceupdatemessage-favorite.md)|Логическое|Измените состояние списка [serviceUpdateMessages](../resources/serviceupdatemessage.md) на избранное для подписанного пользователя.|
|[unfavorite](../api/serviceupdatemessage-unfavorite.md)|Логическое|Удалите любимый статус [serviceUpdateMessages](../resources/serviceupdatemessage.md) для подписанного пользователя.|
|[Список вложений](../api/serviceupdatemessage-list-attachments.md)|[коллекция serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md)|Получите список вложений, связанных с сообщением службы.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionRequiredByDateTime|DateTimeOffset|Ожидаемый крайний срок действия для сообщения.|
|attachmentsArchive|Stream|Файл zip, содержащий все вложения для сообщения.|
|body|[itemBody](../resources/itembody.md)|Тип контента и содержимое тела сообщения службы.|
|category|serviceUpdateCategory|Категория сообщений службы. Возможные значения: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.|
|details|Коллекция ([keyValuePair](../resources/keyvaluepair.md))|Дополнительные сведения о сообщении службы. Это свойство не поддерживает фильтры. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|Конечное время сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|hasAttachments|Boolean|Указывает, есть ли у сообщения какие-либо вложения.|
|id|String|Id сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|isMajorChange|Логическое|Указывает, описывает ли сообщение крупное обновление для службы.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|службы|Коллекция (строка)|Затронутые службы сообщением службы.|
|severity|serviceUpdateSeverity|Серьезность сообщения службы. Возможные значения: `normal`, `high`, `critical`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|Время начала сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|tags|Коллекция (строка)|Коллекция тегов для сообщения службы. Теги предоставляются командой службы/службой поддержки, которая вывешит сообщение, чтобы сообщить, содержит ли это сообщение данные конфиденциальности, или это сообщение для обновления новых функций службы и так далее.|
|title|String|Название сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|viewPoint|[serviceUpdateMessageViewpoint](../resources/serviceupdatemessageviewpoint.md)|Представляет пользовательские точки зрения данных сообщения службы. Эти данные включают состояние сообщения, например, имеет ли пользователь архив, чтение или помеченное сообщение как любимое. Это свойство является null при доступе с разрешениями приложений.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|attachments|Collection([serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md))|Коллекция [serviceAnnouncementAttachments](../resources/serviceannouncementattachment.md).|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "baseType": "microsoft.graph.serviceAnnouncementBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessage",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "category": "String",
  "severity": "String",
  "tags": [
    "String"
  ],
  "isMajorChange": "Boolean",
  "actionRequiredByDateTime": "String (timestamp)",
  "services": [
    "String"
  ],
  "viewPoint": {
    "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
  },
  "hasAttachments": "Boolean",
  "attachmentsArchive": "Stream"
}
```

