---
title: Тип ресурса Контролскоре
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 68e4bf278b7d1b6ea6f00f75192847abab1ae3a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032846"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса Контролскоре

Содержит оценку и описание клиента для отдельного элемента управления.

## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|Контролнаме|String|Уникальное имя элемента управления.|
|score|Двойное|Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).|
|Контролкатегори|String|Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).|
|description|String| Описание элемента управления.|

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
