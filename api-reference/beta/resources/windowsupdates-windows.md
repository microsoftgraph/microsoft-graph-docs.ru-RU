---
title: Тип ресурса Windows
description: Объект, который выступает в качестве контейнера для Windows функций.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8033e9a349be7aafa584d6ab2e5e69bdab66eeb7
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861492"
---
# <a name="windows-resource-type"></a>Тип ресурса Windows

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект, который выступает в качестве контейнера для Windows функций.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Только для чтения. Унаследованный от [сущности](../resources/entity.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|обновления|[microsoft.graph.windowsUpdates.updates](../resources/windowsupdates-updates.md)|Объект, который выступает в качестве контейнера для функциональных возможностей службы Windows обновления для бизнеса. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.windows",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windows",
  "id": "String (identifier)"
}
```

