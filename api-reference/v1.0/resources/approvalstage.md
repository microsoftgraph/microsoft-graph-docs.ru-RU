---
title: Тип ресурса approvalStage
description: Объект approvalStage, связанный с userConsentRequest или запросом на назначение пакета доступа.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2cd51e18cd3d641018c5f0792754cec129392aa6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395855"
---
# <a name="approvalstage-resource-type"></a>Тип ресурса approvalStage

Пространство имен: microsoft.graph

Указывает этап принятия решения в [утверждении](approval.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список утвержденийStages](../api/approval-list-stages.md) | [коллекция approvalStage](approvalstage.md) | Список объектов **approvalStage** , связанных с объектом **утверждения** в управлении правами. |
|[Получить утверждениеStage](../api/approvalstage-get.md) | [approvalStage](approvalstage.md) | Получение свойств объекта **approvalStage** в управлении правами. |
|[Обновление approvalStage](../api/approvalstage-update.md) | Нет | Применить утверждение или отказ в принятии решения по **объекту approvalStage** в управлении правами. |

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedToMe|Boolean|Указывает, назначен ли этап пользователю вызова для проверки. Только для чтения.|
|displayName|String|Метка, предоставленная создателем политики для определения стадии утверждения. Только для чтения.|
|id|String|Идентификатор стадии, связанной с объектом утверждения. Только для чтения.|
|обоснование|String|Обоснование, связанное с решением стадии утверждения.|
|reviewResult|String|Результат этой записи утверждения. Возможные значения: `NotReviewed`, , `Approved``Denied`.|
|reviewedBy|[identity](identity.md) | Идентификатор рецензента. Только для чтения.|
|reviewedDateTime|DateTimeOffset|Дата и время записи решения. Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|status|String|Состояние сцены. Возможные значения: `InProgress`, `Initializing`, `Completed`. `Expired` Только для чтения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approvalStage",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": "Boolean",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
}
```
