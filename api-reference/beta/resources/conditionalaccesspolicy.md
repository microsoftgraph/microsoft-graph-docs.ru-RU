---
title: Тип ресурса Кондитионалакцессполици
description: Указывает атрибуты, связанные с политикой условного доступа или политиками, активируемыми соответствующими действиями при входе.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2c45be8ee32c26187ccf42154ba6c06b60f5efc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973218"
---
# <a name="conditionalaccesspolicy-resource-type"></a>Тип ресурса Кондитионалакцессполици
Указывает атрибуты, связанные с политикой условного доступа или политиками, активируемыми соответствующими действиями при входе.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Указывает имя политики условного доступа (пример: "требовать MFA для Salesforce").|
|Енфорцедгрантконтролс|Коллекция строк|Указывает на элементы управления предоставлением, принудительно примененные политикой условного доступа (пример: "требовать многофакторную проверку подлинности").|
|Енфорцедсессионконтролс|Коллекция строк|Указывает на элементы управления сеансом, принудительно примененные политикой условного доступа (пример: "требовать принудительно заданное приложением элементов управления").|
|id|String|Уникальный идентификатор GUID политики условного доступа|
|result|String| Указывает результат политики ЦС, который был активирован. Возможные значения:<br/> `success` <br/> `failure` <br/> `notApplied`-Политика не применяется, так как условия политики не выполнены. <br/> `notEnabled`— Это связано с тем, что в отключенном состоянии политика отключена.|

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
