---
title: тип ресурса cloudPcSourceDeviceImage
description: 'Исходный образ, связанный с подпиской на Azure. '
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 9bfdb8240d72a9b97f8b4dc89844734416576021
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723571"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a>тип ресурса cloudPcSourceDeviceImage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Исходный образ, связанный с подпиской на Azure.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Код исходных изображений.|
|displayName|String|Имя отображения для исходных изображений.|
|subscriptionId|String|ID подписки, на котором размещено исходный образ.|
|subscriptionDisplayName|String|Отображает имя подписки, на котором размещено исходный образ.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "subscriptionId": "String",
  "subscriptionDisplayName": "String"
}
```
