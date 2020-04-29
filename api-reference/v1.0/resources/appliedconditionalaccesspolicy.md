---
title: Тип ресурса Апплиедкондитионалакцессполици
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующими действиями при входе.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10fe3898c215955e968171cc16f97617afc9aefa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532114"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>Тип ресурса Апплиедкондитионалакцессполици

Пространство имен: microsoft.graph

Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующими действиями при входе.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Указывает имя политики условного доступа (пример: "требовать MFA для Salesforce").|
|енфорцедгрантконтролс|Коллекция объектов string|Указывает на элементы управления предоставлением, принудительно примененные политикой условного доступа (пример: "требовать многофакторную проверку подлинности").|
|енфорцедсессионконтролс|Коллекция объектов string|Указывает на элементы управления сеансом, принудительно примененные политикой условного доступа (пример: "требовать принудительно заданное приложением элементов управления").|
|id|String|Уникальный идентификатор GUID для условного доступа полик. y|
|result|String| Указывает результат политики ЦС, который был активирован. Возможные значения:<br/>`success`<br/>`failure`<br/>`notApplied`-Политика не применяется, так как условия политики не выполнены.<br/>`notEnabled`— Это связано с тем, что в отключенном состоянии политика отключена.|

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
