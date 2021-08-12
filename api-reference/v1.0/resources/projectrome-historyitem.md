---
title: Тип ресурса historyItem
description: Представляет элемент истории для действий в приложении. Действия пользователей представляют собой одно предназначение в вашем приложении , например, телешоу, документ или текущую кампанию в видеоигре. Когда пользователь участвует в этом действии, взаимодействие запечатлено как элемент истории, который указывает время начала и окончания этого действия. По мере повторного вовлечения пользователя в это действие с течением времени для одного пользователя записывают несколько элементов истории.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 7e845158dce7b8b3d0ea74eff673e179cda19b78e74d5a20512ea2c786fa1796
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246628"
---
# <a name="historyitem-resource-type"></a>Тип ресурса historyItem

Пространство имен: microsoft.graph

Представляет элемент истории для [действий](projectrome-activity.md) в приложении. Действия пользователей представляют собой одно предназначение в вашем приложении , например, телешоу, документ или текущую кампанию в видеоигре. Когда пользователь участвует в этом действии, взаимодействие запечатлено как элемент истории, который указывает время начала и окончания этого действия. По мере повторного вовлечения пользователя в это действие с течением времени для одного пользователя записывают несколько элементов истории.

Когда приложение создает сеанс, объект **historyItem** должен быть  добавлен в объект активности, чтобы отразить период вовлечения пользователей. При каждом повторном взаимодействии пользователя с действием в действие добавляется новая **historyItem** для начисления вовлеченности пользователей.

## <a name="methods"></a>Методы

|Метод | Возвращаемый тип | Описание|
|:------|:------------|:-----------|
|[Создание или замена historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | Создает или заменяет существующую **historyItem** для этого действия (upsert). ID должен быть GUID.|
|[Удаление historyItem](../api/projectrome-delete-historyitem.md) | Содержимое отсутствует | Удаляет указанный **historyItem** для этого действия.|

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|status | status | Набор сервера. Код состояния, используемый для идентификации допустимых объектов. Значения: активные, обновляются, удаляются, игнорируются.|
|userTimezone | String | Необязательный параметр. Часовой пояс, в котором устройство пользователя использовалось для создания активности, находился во время создания активности. Значения, предоставленные в качестве ID Olson для поддержки межплатформеного представления.|
|createdDateTime | DateTimeOffset | Набор сервера. DateTime в UTC, когда объект был создан на сервере.|
|lastModifiedDateTime | DateTimeOffset | Набор сервера. DateTime в UTC, когда объект был изменен на сервере.|
|id | String | Обязательный. GUID, заданный клиентом для **объекта historyItem.**|
|startedDateTime | DateTimeOffset | Обязательный элемент. UTC DateTime при **запусках historyItem** (сеанса активности). Необходимый для истории временной шкалы.|
|lastActiveDateTime | DateTimeOffset | Необязательно. UTC DateTime, когда сеанс **historyItem** (сеанс активности) в последний раз понимался как активный или завершенный , если нет, **состояние historyItem** должно быть текущим.|
|expirationDateTime | DateTimeOffset | Необязательно. UTC DateTime, когда **historyItem** будет проходить жесткое удаление. Может быть установлен клиентом.|
|activeDurationSeconds | int | Необязательный параметр. Продолжительность активного вовлечения пользователей. если не поставляется, это рассчитывается из **startedDateTime** и **lastActiveDateTime**.|

## <a name="relationships"></a>Связи

|Связь | Тип | Описание|
|:------------|:-----|:-----------|
|действие| [userActivity](../resources/projectrome-activity.md) | Необязательно. NavigationProperty/Containment; свойство навигации для связанного действия.|

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

