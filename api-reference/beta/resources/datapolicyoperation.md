---
title: Тип ресурса dataPolicyOperation
description: Представляет операцию политики отправленных данных. Он содержит сведения, необходимые для отслеживания состояния операции. Например администратор компании запрос данных политики операции экспорта данных сотрудника компании и затем отслеживать этот запрос.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4547221c8c1b859d4738a5468603ac6890246263
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570927"
---
# <a name="datapolicyoperation-resource-type"></a>Тип ресурса dataPolicyOperation

Представляет операцию политики отправленных данных. Он содержит сведения, необходимые для отслеживания состояния операции. Например администратор компании запрос данных политики операции экспорта данных сотрудника компании и затем отслеживать этот запрос.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Чтение свойств объекта dataPolicyOperation.|

## <a name="properties"></a>Свойства

> **Примечание:** Все свойства в этом ресурсов доступны только для чтения.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Представляет, когда запрос для этой операции политики данных был выполнен, в формате UTC, в формате ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. NULL до завершения операции.|
|id|Строка| Уникальный ключ для этой операции. |
|status|string| Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|Строка|URL-адрес расположения, в котором выполняется экспорт данных для запросы на экспорт.|
|userId|String|Идентификатор пользователя, для которого выполняется операция.|
|submittedDateTime|DateTimeOffset|Представляет, когда для этой операции с данными был отправлен запрос, в формате UTC, в формате ISO 8601. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

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
  "submittedDateTime": "String (timestamp)"
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
