---
title: Тип ресурса dataPolicyOperation
description: Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bec2403ca4e1bad13af801b67d95f3ec9b30d4f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049991"
---
# <a name="datapolicyoperation-resource-type"></a>Тип ресурса dataPolicyOperation

Пространство имен: microsoft.graph

Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Чтение свойств объекта dataPolicyOperation.|

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
|progress|Двойное с плавающей точкой|Задает ход выполнения операции.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

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
  "progress": "Double"
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


