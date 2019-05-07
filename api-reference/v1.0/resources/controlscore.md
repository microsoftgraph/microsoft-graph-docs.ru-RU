---
title: Тип ресурса Контролскоре
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 64b5377fce01273ab31d7ec293f5dc7a6e1342ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629287"
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
