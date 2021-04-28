---
title: обновляет тип ресурса
description: Объект, который выступает в качестве контейнера для всех функций Windows обновления для службы развертывания бизнеса.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0306dbadd815bdd8ff0ffde5719a950bcdff4683
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067484"
---
# <a name="updates-resource-type"></a>обновляет тип ресурса

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект, который выступает в качестве контейнера для всех функций Windows обновления для службы развертывания бизнеса.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Только для чтения. Унаследованный от [сущности](../resources/entity.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|каталог|[microsoft.graph.windowsUpdates.catalog](../resources/windowsupdates-catalog.md)|Каталог контента, который может быть утвержден для развертывания службой развертывания. Только для чтения.|
|развертывания|[коллекция microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|Развертывания, созданные с помощью службы развертывания. Только для чтения.|
|updatableAssets|[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Активы, зарегистрированные в службе развертывания, которые могут получать обновления. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updates",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updates",
  "id": "String (identifier)"
}
```

