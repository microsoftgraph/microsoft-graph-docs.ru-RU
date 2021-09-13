---
title: тип ресурса controlScore
description: Этот ресурс содержит оценку клиента и описание для отдельного управления.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 155b17ed62e3aa61ea523f57ce17fd1ec0df1ee9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049544"
---
#  <a name="controlscore-resource-type"></a>тип ресурса controlScore

Пространство имен: microsoft.graph

Содержит оценку клиента и описание для отдельного управления.

## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|controlName|String|Управление уникальным именем.|
|оценка|Двойное с плавающей точкой|Клиент достиг показателей для управления (он меняется день ото дня в зависимости от операций клиента на контроле).|
|controlCategory|Строка|Категория действия управления (Identity, Data, Device, Apps, Infrastructure).|
|description|Строка| Описание управления.|

## <a name="json-representation"></a>Представление в формате JSON

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

