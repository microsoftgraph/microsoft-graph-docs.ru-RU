---
title: " Тип ресурса Контролскоре"
description: Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543380"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса Контролскоре

Этот ресурс содержит оценку и описание клиента для отдельного элемента управления.

|Имя |Тип |Описание |
|:--|:--|:--|
|   Контролнаме |   String  |   Уникальное имя элемента управления |
|   score   |   Двойное  |  Оценка, полученная клиентом для элемента управления (она варьируется по дням, в зависимости от операций клиента в элементе управления). |
|   Контролкатегори |   String  |  Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура). |
|   description |   String  |  Описание элемента управления. |

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
  "score": "String",
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
