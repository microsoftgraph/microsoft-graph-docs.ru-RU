---
title: тип ресурса updateManagementEnrollment
description: Представляет регистрацию в управлении службой определенной категории обновлений.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 992cfc8ebf53db3b1f3aad7c3c997d02344a503b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861585"
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

