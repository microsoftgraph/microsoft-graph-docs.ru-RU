---
title: Тип ресурса printTaskDefinition
description: Представляет задачу, которую можно запускать при различных событиях в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bbffceb08be336cd816d80f03236078b39348339
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934865"
---
# <a name="printtaskdefinition-resource-type"></a>Тип ресурса printTaskDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет абстрактное определение задачи, которое может запускаться при различных событиях в универсальной печати.

Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати с потягивом в универсальную печать, см. в подстройки "Расширение универсальной печати [для поддержки печати потягив".](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

Этот ресурс поддерживает:
* [Подписка на уведомления об изменениях.](/graph/universal-print-webhook-notifications)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/print-list-taskdefinitions.md) | [Коллекция printTaskDefinition](printtaskdefinition.md) | Получите полный список printTaskDefinitions, созданных в универсальной печати. |
| [Создание](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создайте новый printTaskDefinition. |
| [обновление](../api/print-update-taskdefinition.md). | [printTaskDefinition](printtaskdefinition.md) | Обновление printTaskDefinition. |
| [удаление](../api/print-delete-taskdefinition.md); | Нет | Удаление printTaskDefinition. |
| [Перечисление задач](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Получите список задач, созданных на основе этого определения. Список включает в себя задачи, которые в настоящее время запущены, и недавно завершенные задачи. |
| [Вывод задачи](../api/printtask-get.md) | [printTask](printtask.md) | Получает задачу, созданную на основе этого определения. |
| [Обновление задачи](../api/printtaskdefinition-update-task.md) | Нет | Обновление задачи, созданной на основе этого определения. **Приложения, регистрющие триггеры задач, отвечают за обновление состояния задачи после завершения обработки, если связанная задача printJob не была перенаправлена на другой принтер.** Если не сообщить о завершении, связанное задание печати будет заблокировано и удалено. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор printTaskDefinition. Только для чтения.|
|displayName|String|Имя printTaskDefinition.|
|createdBy|[appIdentity](appidentity.md)|Приложение, созда которое создало printTaskDefinition. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|tasks|[Коллекция printTask](printtask.md)|Список задач, созданных на основе этого определения. Список включает в себя задачи, которые в настоящее время запущены, и недавно завершенные задачи. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {"@odata.type": "microsoft.graph.appIdentity"},
  "tasks": [{"@odata.type": "microsoft.graph.printTask"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

