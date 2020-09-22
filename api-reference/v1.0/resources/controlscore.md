---
title: Тип ресурса Контролскоре
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e4470d1ce22f5ffbf3c805adc5328398d57d9fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056926"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса Контролскоре

Пространство имен: microsoft.graph

Содержит оценку и описание клиента для отдельного элемента управления.

## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|контролнаме|String|Уникальное имя элемента управления.|
|коэффициент|Двойное с плавающей точкой|Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления).|
|контролкатегори|String|Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).|
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

