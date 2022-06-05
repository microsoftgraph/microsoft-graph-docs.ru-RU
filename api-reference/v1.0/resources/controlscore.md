---
title: Тип ресурса controlScore
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 393f1323c72d6755b2947188dfcefe472b39b4ce
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898247"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса controlScore

Пространство имен: microsoft.graph

Содержит оценку и описание клиента для отдельного элемента управления.

## <a name="properties"></a>Свойства

|Имя |Тип |Описание |
|:--|:--|:--|
|controlName|Строка|Управление уникальным именем.|
|Оценка по|Двойное с плавающей точкой|Клиент достигает оценки для элемента управления (он изменяется день за днем в зависимости от операций клиента в элементе управления).|
|controlCategory|Строка|Категория действий управления (удостоверение, данные, устройство, приложения, инфраструктура).|
|description|Строка| Описание элемента управления.|

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

