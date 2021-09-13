---
title: Тип ресурса инициатора
description: Описывает, кто и что инициировал событие подготовка.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5a00be289964c749adcea2b7f4df80dd477c1a99
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129861"
---
# <a name="initiator-resource-type"></a>Тип ресурса инициатора

Пространство имен: microsoft.graph

Описывает, кто и что инициировал событие подготовка. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Имя лица или службы, которая инициировала событие подготовка.|
|id|String|Уникально идентифицирует человека или службу, которая инициировала событие подготовка.|
|initiatorType|initiatorType| Тип инициатора. Возможные значения: `user`, `application`, `system`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


