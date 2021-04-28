---
title: тип ресурса softwareUpdateReference
description: Представляет определенный контент обновления.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 66f7f895bd3d7556ad5e3d35066236663b474f41
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068203"
---
# <a name="softwareupdatereference-resource-type"></a>тип ресурса softwareUpdateReference

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный контент обновления.

В развертывании одно и то же **программное обеспечениеUpdateReference** может привести к тому, что устройства получают различные изменения обновления, но контент считается контекстуальным эквивалентом для всех устройств в развертывании.

Все ссылки на обновление программного обеспечения существуют как один из следующих производных типов: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md).

Наследуется [от deployableContent](../resources/windowsupdates-deployablecontent.md). Базовый тип [для windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).

Это абстрактный тип.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateReference"
}
```

