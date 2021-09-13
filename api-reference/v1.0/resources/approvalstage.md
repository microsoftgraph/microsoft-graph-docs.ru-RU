---
title: Тип ресурса approvalStage
description: Объект approvalStage, связанный с userConsentRequest.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 69e90233a5b9ae0221e7016ebdd255058ea95cad
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067607"
---
# <a name="approvalstage-resource-type"></a>Тип ресурса approvalStage

Пространство имен: microsoft.graph

Указывает этапы принятия решений в утверждении.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedToMe|Логический|Указывает, назначен ли этап пользователю вызова для проверки. Только для чтения.|
|displayName|Строка|Метка, предоставленная создателем политики для определения стадии утверждения. Только для чтения.|
|id|String|Идентификатор стадии, связанной с объектом утверждения. Только для чтения.|
|обоснование|Строка|Обоснование, связанное с решением стадии утверждения.|
|reviewResult|Строка|Результат этой записи утверждения. Возможные значения: `NotReviewed` , `Approved` , `Denied` .|
|reviewedBy|[userIdentity](useridentity.md) | Идентификатор рецензента. Только для чтения.|
|reviewedDateTime|DateTimeOffset|Дата и время записи решения. Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|status|String|Состояние сцены. Возможные значения: `InProgress` `Initializing` , , `Completed` `Expired` . Только для чтения.|

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
