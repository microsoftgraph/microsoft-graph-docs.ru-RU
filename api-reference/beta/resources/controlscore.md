---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
ms.openlocfilehash: 34e94128ff3993a01d37770bea1ad046f936405f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341185"
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
