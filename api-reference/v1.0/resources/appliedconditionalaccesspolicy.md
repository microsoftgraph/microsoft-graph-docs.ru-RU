---
title: тип ресурса appliedConditionalAccessPolicy
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 140402be929fc6d0d906b084251e21bab80f1a24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078968"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>тип ресурса appliedConditionalAccessPolicy

Пространство имен: microsoft.graph

Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Ссылается на имя политики условного доступа (например: "Require MFA for Salesforce").|
|enforcedGrantControls|Коллекция String|Относится к средствам управления грантами, которые применяются в политике условного доступа (пример: "Требуется многофакторная проверка подлинности").|
|enforcedSessionControls|Коллекция String|Относится к средствам управления сеансами, которые применяются в политике условного доступа (пример: "Требуется принудительное управление приложениями").|
|id|String|Идентификатор политики условного доступа.|
|result|appliedConditionalAccessPolicyResult| Указывает результат срабатываемой политики ЦС. Возможные значения: , ( Политика не применяется, так как условия политики не были выполнены), (Это связано с политикой в состоянии `success` `failure` `notApplied` `notEnabled` отключения), `unknown` , `unknownFutureValue` .|

## <a name="json-representation"></a>Представление в формате JSON

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

