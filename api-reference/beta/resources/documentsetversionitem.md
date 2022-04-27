---
title: Тип ресурса documentSetVersionItem
description: Представляет элемент, который является частью записанной версии набора документов.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: ab6bc8f0084935e66d8fd772c6e1d13b59841012
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061234"
---
# <a name="documentsetversionitem-resource-type"></a>Тип ресурса documentSetVersionItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элемент [,](../resources/listitem.md) который является частью записанного [documentSetVersion](../resources/documentsetversion.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Itemid|String| Уникальный идентификатор элемента. |
|title|String| Заголовок элемента. |
|идентификатор версии|String| Идентификатор версии элемента.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.documentSetVersionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.documentSetVersionItem",
  "itemId": "String",
  "title": "String",
  "versionId": "String"
}
```

