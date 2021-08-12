---
title: тип ресурса controlScore
description: Этот ресурс содержит оценку клиента и описание для отдельного управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be1da81848b5669f66735e4288dccd09ccc30ac0384cc66897fb0a501907f031
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202513"
---
#  <a name="controlscore-resource-type"></a>тип ресурса controlScore

Пространство имен: microsoft.graph

Содержит оценку клиента и описание для отдельного управления.

## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|controlName|String|Управление уникальным именем.|
|оценка|Двойное с плавающей точкой|Клиент достиг показателей для управления (он меняется день ото дня в зависимости от операций клиента на контроле).|
|controlCategory|String|Категория действия управления (Identity, Data, Device, Apps, Infrastructure).|
|description|String| Описание управления.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

