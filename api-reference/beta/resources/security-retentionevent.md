---
title: Тип ресурса retentionEvent
description: Представляет триггер для меток хранения на основе событий, где начало периода хранения основано на возникновении определенного типа события.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f44ac532720497888a151776b823884a11782009
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447735"
---
# <a name="retentionevent-resource-type"></a>Тип ресурса retentionEvent

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет триггер для меток хранения на основе событий, где начало периода хранения основано на возникновении определенного типа события.
Дополнительные сведения об этом см. в [разделе "Запуск хранения при возникновении события"](/microsoft-365/compliance/event-driven-retention).


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление retentionEvents](../api/security-retentionevent-list.md)|[Коллекция microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)|Получение списка объектов [retentionEvent](../resources/security-retentionevent.md) и их свойств.|
|[Создание retentionEvent](../api/security-retentionevent-post.md)|[microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)|Создайте объект [retentionEvent](../resources/security-retentionevent.md) .|
|[Получение retentionEvent](../api/security-retentionevent-get.md)|[microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md)|Чтение свойств и связей объекта [retentionEvent](../resources/security-retentionevent.md) .|
|[Удаление retentionEvent](../api/security-retentionevent-delete.md)|Нет|Удаление объекта [retentionEvent](../resources/security-retentionevent.md) .|
|[List retentionEventType](../api/security-retentioneventtype-list.md)|[Коллекция microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Получение ресурсов retentionEventType из свойства навигации exapnd eventType.|
|[Создание retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Добавьте eventType, добавив соответствующее свойство odata при создании события.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Пользователь, создавший retentionEvent.|
|createdDateTime|DateTimeOffset|Дата создания события retentionEvent.|
|description|String|Необязательные сведения о событии.|
|displayName|String|Имя события.|
|eventPropagationResult|[microsoft.graph.security.eventPropagationResult](../resources/security-eventpropagationresult.md)|Представляет состояние успешности созданного события и дополнительные сведения.|
|eventQueries|[Коллекция microsoft.graph.security.eventQueries](../resources/security-eventqueries.md)| Представляет рабочую нагрузку (SharePoint Online, OneDrive для бизнеса, Exchange Online) и идентификационные данные, связанные с событием хранения.|
|retentionEventStatus|[Коллекция microsoft.graph.security.retentionEventStatus](../resources/security-retentioneventstatus.md)|Состояние свойства события для расположений с заданной областью после создания события.|
|eventTriggerDateTime|DateTimeOffset|Необязательное время запуска события.|
|id|String|Представляет уникальный идентификатор пользователя, создавшего retentionEvent. [entity](/graph/api/resources/entity).|
|lastModifiedBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Пользователь, который последним изменил параметр retentionEvent.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения параметра retentionEvent.|
|lastStatusUpdateDateTime|DateTimeOffset|Время последнего обновления состояния события.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|retentionEventType|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Указывает событие, которое будет запускать период хранения меток, использующих этот тип события при создании события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "eventQueries": [
    {
      "@odata.type": "microsoft.graph.security.eventQueries"
    }
  ],
  "eventTriggerDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "eventPropagationResults": [
    {
      "@odata.type": "microsoft.graph.security.eventPropagationResult"
    }
  ],
  "eventStatus": {
    "@odata.type": "microsoft.graph.security.retentionEventStatus"
  },
  "lastStatusUpdateDateTime": "String (timestamp)"
}
```