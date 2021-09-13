---
title: " тип ресурса controlScore"
description: Этот ресурс содержит оценку клиента и описание для отдельного управления.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 347e7830239f5bf04f0c8611c955173bdda0f18d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146816"
---
#  <a name="controlscore-resource-type"></a>тип ресурса controlScore

Пространство имен: microsoft.graph

Этот ресурс содержит оценку клиента и описание для отдельного управления.

|Имя |Тип |Описание |
|:--|:--|:--|
|   controlName |   String  |   Управление уникальным именем |
|   оценка   |   Двойное с плавающей точкой  |  Клиент достиг показателей для управления (он меняется день ото дня в зависимости от операций клиента на контроле). |
|   controlCategory |   String  |  Категория действия управления (Identity, Data, Device, Apps, Infrastructure). |
|   description |   String  |  Описание управления. |

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


