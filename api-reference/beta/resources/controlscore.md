---
title: " Тип ресурса controlScore"
description: Этот ресурс содержит счета клиента и описание для отдельного элемента управления.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891471"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса controlScore

Этот ресурс содержит счета клиента и описание для отдельного элемента управления.

|Имя |Тип |Описание |
|:--|:--|:--|
|   ИмяЭлементаУправления |   Строка  |   Уникальное имя элемента управления |
|   score   |   Double  |  Клиент достичь счета для элемента управления (он зависит от дня операций клиента в элементе управления). |
|   controlCategory |   Строка  |  Категория действие элемента управления (удостоверения, данные, устройства, приложения, инфраструктуры). |
|   описание |   Строка  |  Описание элемента управления. |

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
