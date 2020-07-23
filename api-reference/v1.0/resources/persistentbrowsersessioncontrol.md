---
title: Тип ресурса Персистентбровсерсессионконтрол
description: Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a747f2d51d43b30da7dd7566a767cfb5f8c3fcd5
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384886"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a>Тип ресурса Персистентбровсерсессионконтрол

Пространство имен: microsoft.graph

Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie. Наследуется от [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включен ли элемент управления сеансом. |
|mode|String| Возможные значения: `always`, `never`.|

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
