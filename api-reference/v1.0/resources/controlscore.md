---
title: Тип ресурса Контролскоре
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc3de6363784f62792d7c4e56906c79ed1be0c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531767"
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
