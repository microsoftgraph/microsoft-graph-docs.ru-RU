---
title: Тип ресурса historyItem
description: Представляет элемент журнала для действия в приложении. Действия пользователя представляют одну целевую в вашем приложении -, например Показать TV, документа или текущей кампании в игру. Когда пользователь подключает с помощью этого действия, деловые регистрируются как элемента журнала, которое указывает время начала и окончания для этого действия. Как пользователь повторно массовых с этой операции со временем, несколько элементов журнала записываются действия одного пользователя.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 168587aa54446aeee78107deaa9087c6bffb8586
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976956"
---
# <a name="historyitem-resource-type"></a>Тип ресурса historyItem

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет элемент журнала для [действия](projectrome-activity.md) в приложении. Действия пользователя представляют одну целевую в вашем приложении -, например Показать TV, документа или текущей кампании в игру. Когда пользователь подключает с помощью этого действия, деловые регистрируются как элемента журнала, которое указывает время начала и окончания для этого действия. Как пользователь повторно массовых с этой операции со временем, несколько элементов журнала записываются действия одного пользователя.

Когда приложение создает сеанс, объект **historyItem** следует добавить объект **активности** в соответствии с период участия пользователя. Каждый раз, пользователь снова подключает с действием, новые **historyItem** добавляется активности начисления участия пользователя.

## <a name="methods"></a>Методы

|Метод | Возвращаемый тип | Описание|
|:------|:------------|:-----------|
|[Создать или заменить historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | Создает или заменяет существующий **historyItem** для этого действия (upsert). Идентификатор должен быть идентификатор GUID.|
|[Удаление historyItem](../api/projectrome-delete-historyitem.md) | Нет содержимого | Удаляет указанный **historyItem** для этого действия.|

## <a name="properties"></a>Свойства

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|status | EnumType | Установка с сервера. Код состояния, используемое для идентификации допустимый объекты. Значения: активный, обновления, удаления, игнорируются.|
|userTimezone | Строка | Необязательный параметр. Часовой пояс, в котором устройством пользователя, используемый для создания операции находился во время создания активности. Значения, указанные как Олсон идентификаторы для поддержки различных платформах представление.|
|createdDateTime | DateTimeOffset | Установка с сервера. Дата и время в формате UTC, когда объект был создан на сервере.|
|lastModifiedDateTime | DateTimeOffset | Установка с сервера. Дата и время в формате UTC, когда объект был изменен на сервере.|
|id | Строка | Обязательный. Идентификатор GUID набора клиента для объекта **historyItem** .|
|startedDateTime | DateTimeOffset | Обязательный. При запуске **historyItem** (активности сеанса) UTC даты и времени. Требуется для журнал временной шкалы.|
|lastActiveDateTime | DateTimeOffset | Необязательное. При **historyItem** (активности сеанса) последнего был распознан как активных, так и по завершении работы — Если значение null, **historyItem** состояние UTC даты и времени должны быть Ongoing.|
|expirationDateTime | DateTimeOffset | Необязательное. Даты-времени UTC при **historyItem** подвергнется окончательного удаления. Можно задать клиентом.|
|activeDurationSeconds | int | Необязательное. Продолжительность сотрудничества активных пользователей. Если не указано, отсчитывается от **startedDateTime** и **lastActiveDateTime**.|

## <a name="relationships"></a>Связи

|Связь | Тип | Описание|
|:------------|:-----|:-----------|
|activity| [действии](../resources/projectrome-activity.md) | Необязательное. NavigationProperty/вложенности; свойство навигации для связанного действия.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
