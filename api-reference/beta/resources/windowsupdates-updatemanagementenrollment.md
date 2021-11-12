---
title: тип ресурса updateManagementEnrollment
description: Представляет регистрацию в управлении службой определенной категории обновлений.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8d780894e90a1f6eec748a9f62f486b39d3c6cfb
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890187"
---
# <a name="updatemanagementenrollment-resource-type"></a>тип ресурса updateManagementEnrollment

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет регистрацию в управлении службой определенной категории обновлений.

Наследует [от updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|Категория обновлений, управляемых службой. Поддерживает подмножество значений **для updateCategory.** Возможные значения: `feature`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updateManagementEnrollment",
  "updateCategory": "String"
}
```

