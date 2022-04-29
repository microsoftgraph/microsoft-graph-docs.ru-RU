---
title: Тип ресурса cloudPcLaunchInfo
description: Содержит сведения для подключения облачного компьютера.
author: andrewku0409
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 546bd11263c3bdb9ac4421eb8f9eb3580e6af255
ms.sourcegitcommit: 4ef29d4a2cfa1ccc4a3da649e683377b17b90108
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65126362"
---
# <a name="cloudpclaunchinfo-resource-type"></a>Тип ресурса cloudPcLaunchInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения для подключения [cloudPC](../resources/cloudpc.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|cloudPcId|String|Уникальный идентификатор облачного компьютера.|
|cloudPcLaunchUrl|String|URL-адрес подключения облачного компьютера.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcLaunchInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcLaunchInfo",
  "cloudPcId": "String",
  "cloudPcLaunchUrl": "String"
}
```

