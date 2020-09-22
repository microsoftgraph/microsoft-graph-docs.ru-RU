---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 964de9f9567c419b4e14d38e79cdff92867fb5ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016809"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса Контролскоре

Пространство имен: microsoft.graph

Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.

|Имя |Тип |Описание |
|:--|:--|:--|
|   контролнаме |   String  |   Уникальное имя элемента управления |
|   коэффициент   |   Двойное с плавающей точкой  |  Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления). |
|   контролкатегори |   String  |  Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура). |
|   description |   String  |  Описание элемента управления. |

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


