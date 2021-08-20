---
title: " тип ресурса controlScore"
description: Этот ресурс содержит оценку клиента и описание для отдельного управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7f5306f88f2ed14ae13cb95cee7cdb3cfe2ad569405062fe6524b8b747940b9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54190782"
---
#  <a name="controlscore-resource-type"></a>тип ресурса controlScore

Пространство имен: microsoft.graph

Этот ресурс содержит оценку клиента и описание для отдельного управления.

|Имя |Тип |Описание |
|:--|:--|:--|
|   controlName |   Строка  |   Управление уникальным именем |
|   оценка   |   Двойное с плавающей точкой  |  Клиент достиг показателей для управления (он меняется день ото дня в зависимости от операций клиента на контроле). |
|   controlCategory |   String  |  Категория действия управления (Identity, Data, Device, Apps, Infrastructure). |
|   description |   Строка  |  Описание управления. |

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


