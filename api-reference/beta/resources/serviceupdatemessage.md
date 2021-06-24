---
title: тип ресурса serviceUpdateMessage
description: Представляет объявления об изменениях в службе.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: e8bea9b3c44f99d5be0d87b01d47db4505873681
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109226"
---
# <a name="serviceupdatemessage-resource-type"></a>тип ресурса serviceUpdateMessage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объявления об изменениях в службе.

Представляет такие объявления, как основные обновления, новые функции в продукте; например, публикация нового Windows.

Наследует от [serviceAnnouncementBase](../resources/serviceannouncementbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceUpdateMessage](../api/serviceupdatemessage-get.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md)|Извлечение свойств и связей объекта [serviceUpdateMessage.](../resources/serviceupdatemessage.md) |
|[markRead](../api/serviceupdatemessage-markread.md)|Boolean|Пометить список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s в качестве чтения для подписанного пользователя. |
|[markUnread](../api/serviceupdatemessage-markunread.md)|Boolean|Пометить список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s как непрочитанные для подписанного пользователя. |
|[архив](../api/serviceupdatemessage-archive.md)|Boolean|Архивировать список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s для подписанного пользователя.|
|[unarchive](../api/serviceupdatemessage-unarchive.md)|Boolean|Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.|
|[избранное](../api/serviceupdatemessage-favorite.md)|Boolean|Измените состояние списка [serviceUpdateMessage](../resources/serviceupdatemessage.md)s на избранное для подписанного пользователя.|
|[unfavorite](../api/serviceupdatemessage-unfavorite.md)|Boolean|Удалите любимый статус [serviceUpdateMessage](../resources/serviceupdatemessage.md)s для подписанного пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionRequiredByDateTime|DateTimeOffset|Ожидаемый крайний срок действия для сообщения.|
|body|[itemBody](../resources/itembody.md)|Тип контента и содержимое тела сообщения службы.|
|category|serviceUpdateCategory|Категория сообщений службы. Возможные значения: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.|
|подробности|[Коллекция(keyValuePair)](../resources/keyvaluepair.md)|Дополнительные сведения о сообщении службы. Это свойство не поддерживает фильтры. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|endDateTime|DateTimeOffset|Конечное время сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|id|Строка|Id сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|isMajorChange|Boolean|Указывает, описывает ли сообщение крупное обновление для службы.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|службы|Коллекция (строка)|Затронутые службы сообщением службы.|
|severity|serviceUpdateSeverity|Серьезность сообщения службы. Возможные значения: `normal`, `high`, `critical`, `unknownFutureValue`.|
|startDateTime|DateTimeOffset|Время начала сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|tags|Коллекция (строка)|Коллекция тегов для сообщения службы.|
|title|Строка|Название сообщения службы. Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).|
|viewPoint|[serviceUpdateMessageViewpoint](../resources/serviceupdatemessageviewpoint.md)|Представляет данные точек представления пользователей сообщения службы.|

## <a name="relationships"></a>Отношения
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

