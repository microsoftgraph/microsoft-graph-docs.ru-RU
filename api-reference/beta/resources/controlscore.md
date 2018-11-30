---
title: " Тип ресурса controlScore"
description: Этот ресурс содержит счета клиента и описание для отдельного элемента управления.
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076142"
---
#  <a name="controlscore-resource-type"></a>Тип ресурса controlScore

Этот ресурс содержит счета клиента и описание для отдельного элемента управления.

|Имя |Тип |Description |
|:--|:--|:--|
|   ИмяЭлементаУправления |   String  |   Уникальное имя элемента управления |
|   score   |   Double  |  Клиент достичь счета для элемента управления (он зависит от дня операций клиента в элементе управления). |
|   controlCategory |   String  |  Категория действие элемента управления (удостоверения, данные, устройства, приложения, инфраструктуры). |
|   описание |   String  |  Описание элемента управления. |

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
