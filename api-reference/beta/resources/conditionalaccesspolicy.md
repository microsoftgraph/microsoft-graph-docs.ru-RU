---
title: Тип ресурса conditionalAccessPolicy
description: Указывает, что атрибуты, связанные с условного доступа политики или политики запускаются с соответствующей операции регистрации
ms.openlocfilehash: 56a06d6b5fcba96dc472eb63fe24ba3920b0dd09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082542"
---
# <a name="conditionalaccesspolicy-resource-type"></a>Тип ресурса conditionalAccessPolicy
Указывает, что атрибуты, связанные с условного доступа политики или политики запускаются с соответствующей операции регистрации



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|— Это имя политики условного доступа (пример: «Требовать многофакторной проверкой Подлинности для Salesforce»).|
|enforcedGrantControls|Коллекция String|Относится к элементам управления grant, определяемое политики условного доступа (пример: «Требовать многофакторной проверки подлинности»).|
|enforcedSessionControls|Коллекция String|Относится к элементам управления сеанса, определяемое политики условного доступа (пример: «Требовать применения приложения элементы управления»).|
|id|String|Уникальный идентификатор GUID политики условного доступа|
|result|String| Указывает результат политики центра сертификации, который был активирован. Возможными значениями являются:<br/> `success` <br/> `failure` <br/> `notApplied`-Политики не применяется, так как не были выполнены условия политики. <br/> `notEnabled`— Это из-за политики в отключенном состоянии.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->