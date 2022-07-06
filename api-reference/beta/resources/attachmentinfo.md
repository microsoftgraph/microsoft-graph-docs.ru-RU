---
title: Тип ресурса attachmentInfo
description: Представляет атрибуты вложения.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: af43c3e53dd41a28f9e123912bf6153679500f00
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645719"
---
# <a name="attachmentinfo-resource-type"></a>Тип ресурса attachmentInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет атрибуты вложения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|AttachmentType|AttachmentType|Тип вложения. Допустимые значения: `file`, `item`, `reference`. Обязательный.|
|contentType|String|Характер данных во вложении. Необязательное.|
|name|String|Отображаемое имя вложения. Это может быть описательная строка, которая не обязательно должна быть фактическим именем файла. Обязательный.|
|size|Int64|Размер вложения в байтах. Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attachmentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attachmentInfo",
  "attachmentType": "String",
  "contentType": "String",
  "name": "String",
  "size": "Int64"
}
```

