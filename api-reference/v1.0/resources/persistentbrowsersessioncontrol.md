---
title: тип ресурса persistentBrowserSessionControl
description: Управление сеансом, чтобы определить, следует ли сохранять файлы cookie или нет.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 52c4efd5d7a3bfb87c34ab07ba84349c6d392af3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117825"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a>тип ресурса persistentBrowserSessionControl

Пространство имен: microsoft.graph

Управление сеансом, чтобы определить, следует ли сохранять файлы cookie или нет. Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включено ли управление сеансом. |
|mode|persistentBrowserSessionMode| Возможные значения: `always`, `never`.|

## <a name="relationships"></a>Отношения

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

