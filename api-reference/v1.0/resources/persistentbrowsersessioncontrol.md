---
title: тип ресурса persistentBrowserSessionControl
description: Управление сеансом, чтобы определить, следует ли сохранять файлы cookie или нет.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 440285b790e64af5c7a4764baf3176ac464fb7beedec848af444de55c432ef1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124222"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a>тип ресурса persistentBrowserSessionControl

Пространство имен: microsoft.graph

Управление сеансом, чтобы определить, следует ли сохранять файлы cookie или нет. Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включено ли управление сеансом. |
|mode|persistentBrowserSessionMode| Возможные значения: `always`, `never`.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "mode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persistentBrowserSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

