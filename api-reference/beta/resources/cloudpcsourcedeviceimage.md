---
title: Тип ресурса Клаудпксаурцедевицеимаже
description: 'Исходное изображение, связанное с вашей подпиской Azure. '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c944ab1a634d10e978c6ce1620ebe1accc5e4359
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563746"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>Тип ресурса Клаудпксаурцедевицеимаже

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Исходное изображение, связанное с вашей подпиской Azure.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор исходного изображения.|
|displayName|String|Отображаемое имя исходного изображения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage",
  "baseType": "microsoft.graph.entity"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
