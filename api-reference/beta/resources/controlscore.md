---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 89e448d828f1f7caef73b14586b06d1df238f100
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973935"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса Контролскоре

Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.

|Имя |Тип |Описание |
|:--|:--|:--|
|   Контролнаме |   String  |   Уникальное имя элемента управления |
|   score   |   Двойное  |  Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления). |
|   Контролкатегори |   String  |  Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура). |
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
