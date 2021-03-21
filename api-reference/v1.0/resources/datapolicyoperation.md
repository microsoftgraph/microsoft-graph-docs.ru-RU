---
title: тип ресурса dataPolicyOperation
description: Представляет собой операцию по отправке политики данных. Он содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.
author: dkershaw10
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7b07cb2906eb1a3d01d6c24ca5b91fec35ec7c8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962002"
---
# <a name="datapolicyoperation-resource-type"></a>тип ресурса dataPolicyOperation

Пространство имен: microsoft.graph

Представляет собой операцию по отправке политики данных. Он содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Извлечение свойств **объекта dataPolicyOperation.**|
|[Экспорт личных данных](../api/user-exportpersonaldata.md) | Нет |Отправка запроса на операцию политики данных для экспорта данных пользователя организации, которые можно прочитать с помощью [Get dataPolicyOperation](../api/datapolicyoperation-get.md)|

## <a name="properties"></a>Свойства

> **Примечание:** Все свойства этого ресурса являются только для чтения.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Представляет, когда запрос на эту операцию политики данных был выполнен во время UTC с помощью формата ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Null до завершения операции.|
|id|String| Уникальный ключ для этой операции. |
|status|dataPolicyOperationStatus| Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String|Расположение URL-адреса, куда экспортируются данные для запросов на экспорт.|
|userId|String|ID для пользователя, на котором выполняется операция.|
|submittedDateTime|DateTimeOffset|Представляет при отправке запроса на эту операцию данных во время UTC с помощью формата ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|progress|String|Указывает ход операции.|

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

