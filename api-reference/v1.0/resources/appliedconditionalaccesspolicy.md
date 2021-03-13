---
title: тип ресурса appliedConditionalAccessPolicy
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3aa114c23888ccc6852314e2274b8a89ca440344
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761530"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>тип ресурса appliedConditionalAccessPolicy

Пространство имен: microsoft.graph

Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|displayName|String|Ссылается на имя политики условного доступа (например: "Require MFA for Salesforce").|
|enforcedGrantControls|Коллекция строк|Относится к средствам управления грантами, которые применяются в политике условного доступа (пример: "Требуется многофакторная проверка подлинности").|
|enforcedSessionControls|Коллекция строк|Относится к средствам управления сеансами, которые применяются в политике условного доступа (пример: "Требуется принудительное управление приложениями").|
|id|String|Уникальный GUID политики условного доступа.|
|result|String| Указывает результат срабатываемой политики ЦС. Возможные значения:<br/>`success`<br/>`failure`<br/>`notApplied` - Политика не применяется, так как условия политики не были выполнены.<br/>`notEnabled` - Это связано с политикой в состоянии отключения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
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
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

