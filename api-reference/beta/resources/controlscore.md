---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f718e197e690d3779870e5996161461fe8f60915
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507417"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса Контролскоре

Пространство имен: Microsoft. Graph

Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.

|Имя |Тип |Описание |
|:--|:--|:--|
|   контролнаме |   String  |   Уникальное имя элемента управления |
|   score   |   Двойное с плавающей точкой  |  Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления). |
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
