---
title: тип ресурса teamworkPeripheral
description: Представляет сведения о периферийных устройствах, присоединенных к устройству с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 645cf2d64e50d4d46fe2e76ff8c92dcdf948c74f
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262626"
---
# <a name="teamworkperipheral-resource-type"></a>тип ресурса teamworkPeripheral

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о периферийных устройствах, присоединенных к устройству с Microsoft Teams [включенной поддержкой](../resources/teamworkdevice.md).

Наследуется [от сущности](../resources/entity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображение имени периферийного устройства.|
|id|String|Уникальный идентификатор для определенного периферийного устройства. Наследуется [от сущности](../resources/entity.md).|
|productId|String|ID продукта устройства. Каждый продукт от поставщика имеет свой собственный ID.|
|vendorId|String|Уникальный идентификатор для поставщика устройства. Каждый поставщик имеет уникальный ID.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkPeripheral",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheral",
  "displayName": "String",
  "id": "String (identifier)",
  "productId": "String",
  "vendorId": "String"
}
```

