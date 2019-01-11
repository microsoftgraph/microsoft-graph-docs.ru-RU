---
title: Тип ресурса conditionalAccessPolicy
description: Указывает, что атрибуты, связанные с условного доступа политики или политики запускаются с соответствующей операции регистрации
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820645"
---
# <a name="conditionalaccesspolicy-resource-type"></a>Тип ресурса conditionalAccessPolicy
Указывает, что атрибуты, связанные с условного доступа политики или политики запускаются с соответствующей операции регистрации



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|— Это имя политики условного доступа (пример: «Требовать многофакторной проверкой Подлинности для Salesforce»).|
|enforcedGrantControls|Коллекция String|Относится к элементам управления grant, определяемое политики условного доступа (пример: «Требовать многофакторной проверки подлинности»).|
|enforcedSessionControls|Коллекция String|Относится к элементам управления сеанса, определяемое политики условного доступа (пример: «Требовать применения приложения элементы управления»).|
|id|Строка|Уникальный идентификатор GUID политики условного доступа|
|result|Строка| Указывает результат политики центра сертификации, который был активирован. Возможными значениями являются:<br/> `success` <br/> `failure` <br/> `notApplied`-Политики не применяется, так как не были выполнены условия политики. <br/> `notEnabled`— Это из-за политики в отключенном состоянии.|

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
