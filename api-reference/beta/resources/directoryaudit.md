---
title: Тип ресурса directoryAudit
description: Этот ресурс представляет элементы аудита каталогов и ее коллекцию
author: lleonard-msft
localization_priority: Priority
ms.openlocfilehash: f3b1aa12c18205379220a924be81b53bf6014900
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820512"
---
# <a name="directoryaudit-resource-type"></a>Тип ресурса directoryAudit
Этот ресурс представляет элементы аудита каталогов и ее коллекцию


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Список элементов аудита каталога в коллекции и их свойства.|
|[Получение directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Получение элемента аудита конкретного каталога и его свойства.|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|activityDateTime|DateTimeOffset|Указывает дату и время выполнения операции. Тип метки времени — всегда в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|activityDisplayName|Строка|Указывает имя действия или имя операции (например: «Создание пользователя», «Добавить члена в группу»). Список действий вход можно получить [список активности Azure Ad](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).|
|additionalDetails|Коллекция [keyValue](keyvalue.md)|Указывает Дополнительные сведения для действия.|
|category|String|Показывает, какая категория ресурсов, целевым с помощью этого действия. (Например: управление пользователей, группы управления и т.д..)|
|correlationId|GUID|Указывает уникальный идентификатор, и приводятся рекомендации по их действия, охватывающих различных служб. Можно использовать для журналов трассировки в службах.|
|id|Строка| Указывает уникальный идентификатор для действия. Это идентификатор GUID.|
|initiatedBy|[auditActivityInitiator](auditactivityinitiator.md)|Указывает, что сведения о пользователе или приложение инициировал действие.|
|loggedByService|Строка|Указывает сведения, на котором служба инициировал действие (например: управление средствами самостоятельного создания пароля, основная служба каталогов, B2C, приглашение пользователей, Microsoft Identity Manager, привилегированной управления удостоверениями.|
|result|string| Указывает результат операции. Возможные значения: `success`, `failure`, `timeout`, `unknownFutureValue`.||
|resultReason|Строка|Указывает причину сбоя, если результат является «Ошибка» или «время ожидания».|
|targetResources|[targetResource](targetresource.md) коллекции|Указывает на данные, на котором был изменен ресурсов из-за загрузки. Тип ресурса конечного может быть пользователя, устройства, каталог, приложение, роли, группы, политики или другое.

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
