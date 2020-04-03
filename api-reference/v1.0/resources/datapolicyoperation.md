---
title: Тип ресурса dataPolicyOperation
description: Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8a67d1833a56bb8e1fc1a7c5f5716d165c755f41
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123170"
---
# <a name="datapolicyoperation-resource-type"></a>Тип ресурса dataPolicyOperation

Пространство имен: microsoft.graph

Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Получение свойств объекта **dataPolicyOperation** .|
|[Экспорт личных данных](../api/user-exportpersonaldata.md) | Нет |Отправить запрос операции политики данных для экспорта данных пользователя организации, которые впоследствии можно прочитать с помощью [Get dataPolicyOperation](../api/datapolicyoperation-get.md)|

## <a name="properties"></a>Свойства

> **Примечание:** Все свойства этого ресурса доступны только для чтения.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Представляет время завершения запроса для этой операции политики данных в формате UTC с использованием формата ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Значение null до завершения операции.|
|id|Строка| Уникальный ключ для этой операции. |
|status|string| Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|сторажелокатион|Строка|URL-адрес, по которому выполняется экспорт данных для запросов на экспорт.|
|userId|String|Идентификатор пользователя, для которого выполняется операция.|
|субмиттеддатетиме|DateTimeOffset|Представляет время отправки запроса для этой операции с данными в формате UTC с использованием формата ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|progress|Строка|Задает ход выполнения операции.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
