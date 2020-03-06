---
title: Тип ресурса historyItem
description: Представляет элемент журнала для действия в приложении. Действия пользователей представляют собой одно назначение в вашем приложении (например, телепередачи, документ или текущую кампанию в видеоигре). Когда пользователь наносит это действие, задействование регистрируется в виде элемента журнала, который указывает время начала и окончания для этого действия. По мере того как пользователь повторно перезапускается с этим действием, для одного действия пользователя записываются несколько элементов журнала.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 4053811f1f44621b05830bf40b17d02e0112b455
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533949"
---
# <a name="historyitem-resource-type"></a>Тип ресурса historyItem

Пространство имен: microsoft.graph

Представляет элемент журнала для [действия](projectrome-activity.md) в приложении. Действия пользователей представляют собой одно назначение в вашем приложении (например, телепередачи, документ или текущую кампанию в видеоигре). Когда пользователь наносит это действие, задействование регистрируется в виде элемента журнала, который указывает время начала и окончания для этого действия. По мере того как пользователь повторно перезапускается с этим действием, для одного действия пользователя записываются несколько элементов журнала.

Когда приложение создает сеанс, объект **historyItem** должен быть добавлен в объект **Activity** для отражения периода участия пользователя. Каждый раз, когда пользователь передается с действием, для начисления задействования пользователей добавляется новый **historyItem** .

## <a name="methods"></a>Методы

|Метод | Возвращаемый тип | Описание|
|:------|:------------|:-----------|
|[Создание или замена historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | Создает или заменяет существующий **historyItem** для этого действия (UPSERT). Идентификатор должен быть идентификатором GUID.|
|[Удаление historyItem](../api/projectrome-delete-historyitem.md) | Содержимое отсутствует | Удаляет указанный **historyItem** для этого действия.|

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|status | status | Задается сервером. Код состояния, используемый для идентификации допустимых объектов. Значения: активные, обновленные, удаленные, проигнорированы.|
|усертимезоне | String | Необязательный параметр. Часовой пояс, в котором устройство пользователя, используемое для создания действия, было размещено во время создания действия. Значения, предоставляемые как идентификаторы Олсона для поддержки представления на нескольких платформах.|
|createdDateTime | DateTimeOffset | Задается сервером. Дата и время в формате UTC, когда объект был создан на сервере.|
|lastModifiedDateTime | DateTimeOffset | Задается сервером. Дата и время в формате UTC, когда объект был изменен на сервере.|
|id | Строка | Обязательный. Идентификатор GUID для объекта **historyItem** в клиентском наборе.|
|стартеддатетиме | DateTimeOffset | Обязательный элемент. Дата и время (UTC) при запуске **historyItem** (сеанс активности). Обязательный для журнала временной шкалы.|
|ластактиведатетиме | DateTimeOffset | Необязательный. Дата и время (в формате UTC), когда **historyItem** (сеанс активности) использовался в последний раз как активный или завершенный — если значение равно null, то состояние **HistoryItem** должно быть текущим.|
|expirationDateTime | DateTimeOffset | Необязательный. Дата и время в формате UTC, когда **historyItem** будет окончательно удален. Может быть задано клиентом.|
|активедуратионсекондс | int | Необязательный параметр. Продолжительность активных пользователей. Если этот параметр не указан, вычисляется из **стартеддатетиме** и **ластактиведатетиме**.|

## <a name="relationships"></a>Связи

|Связь | Тип | Описание|
|:------------|:-----|:-----------|
|activity| [userActivity](../resources/projectrome-activity.md) | Необязательный. Свойство NavigationProperty/вложение; свойство навигации для связанного действия.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
