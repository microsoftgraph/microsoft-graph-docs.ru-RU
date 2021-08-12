---
title: тип ресурса serviceUpdateMessage
description: Представляет объявления об изменениях в службе.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: a786df683a23eed6e1c340331e30b905dd27d8340c608644c65fa4ca5706f891
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253804"
---
# <a name="serviceupdatemessage-resource-type"></a>тип ресурса serviceUpdateMessage

Пространство имен: microsoft.graph

Представляет объявления об изменениях в службе.

Представляет такие объявления, как основные обновления, новые функции в продукте; например, публикация нового Windows.

Наследует от [serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceUpdateMessage](../api/serviceupdatemessage-get.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md)|Извлечение свойств и связей объекта [serviceUpdateMessage.](../resources/serviceupdatemessage.md) |
|[markRead](../api/serviceupdatemessage-markread.md)|Логический|Пометить список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s в качестве чтения для подписанного пользователя. |
|[markUnread](../api/serviceupdatemessage-markunread.md)|Логическое|Пометить список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s как непрочитанные для подписанного пользователя. |
|[архив](../api/serviceupdatemessage-archive.md)|Логический|Архивировать список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s для подписанного пользователя.|
|[unarchive](../api/serviceupdatemessage-unarchive.md)|Логическое|Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.|
|[избранное](../api/serviceupdatemessage-favorite.md)|Логическое|Измените состояние списка [serviceUpdateMessage](../resources/serviceupdatemessage.md)s на избранное для подписанного пользователя.|
|[unfavorite](../api/serviceupdatemessage-unfavorite.md)|Логическое|Удалите любимый статус [serviceUpdateMessage](../resources/serviceupdatemessage.md)s для подписанного пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionRequiredByDateTime|DateTimeOffset|Ожидаемый крайний срок действия для сообщения.|
|body|[itemBody](../resources/itembody.md)|Тип контента и содержимое тела сообщения службы.|
|category|serviceUpdateCategory|Категория сообщений службы. Возможные значения: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.|
|подробности|[Коллекция(keyValuePair)](../resources/keyvaluepair.md)|Дополнительные сведения о сообщении службы. Это свойство не поддерживает фильтры. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|Конечное время сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|id|String|Id сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|isMajorChange|Логическое|Указывает, описывает ли сообщение крупное обновление для службы.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|службы|Коллекция (строка)|Затронутые службы сообщением службы.|
|severity|serviceUpdateSeverity|Серьезность сообщения службы. Возможные значения: `normal`, `high`, `critical`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|Время начала сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|tags|Коллекция (строка)|Коллекция тегов для сообщения службы.|
|title|String|Название сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|viewPoint|[serviceUpdateMessageViewpoint](../resources/serviceupdatemessageviewpoint.md)|Представляет данные точек представления пользователей сообщения службы. Эти данные включают состояние сообщения, например, имеет ли пользователь архив, чтение или помеченное сообщение как любимое. Это свойство является null при доступе с разрешениями приложений.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
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
  }
}
```

