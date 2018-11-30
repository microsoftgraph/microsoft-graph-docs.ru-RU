---
title: Тип ресурса convertIdResult
description: Результат преобразования формата код выполняется с помощью функции translateExchangeIds.
ms.openlocfilehash: 3a17399ffe44c43c78f7b50933b2e847a3e64f32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076140"
---
# <a name="convertidresult-resource-type"></a>Тип ресурса convertIdResult

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Результат преобразования формата код выполняется с помощью функции [translateExchangeIds](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:---------|:-----|:------------|
| sourceId | String | Идентификатор, который был преобразован. Это значение является идентификатором исходного, без преобразованные. |
| targetId | String | Преобразованные идентификатор. Это значение не задано, если не удалось выполнить преобразование. |
| errorDetails | [Общая ошибка](genericerror.md) | Объект error, которое указывает причину сбоя преобразования. Это значение не задано, если преобразование выполнено успешно. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```