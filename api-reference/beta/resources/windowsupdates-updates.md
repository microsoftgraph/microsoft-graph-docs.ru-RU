---
title: обновляет тип ресурса
description: Объект, который выступает в качестве контейнера для всех функций Windows обновления для службы развертывания бизнеса.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 748ef5c6e8e334b2e1c311c07617c181490f4f39
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861542"
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

