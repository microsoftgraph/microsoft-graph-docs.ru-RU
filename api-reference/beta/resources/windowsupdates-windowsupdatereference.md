---
title: тип ресурса windowsUpdateReference
description: Представляет конкретные Windows 10 обновления.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a75f1afe1c2689760848283bf078b957bb8739ba
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067480"
---
# <a name="windowsupdatereference-resource-type"></a>тип ресурса windowsUpdateReference

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет конкретные Windows 10 обновления.

В развертывании одно и то же Windows обновления может привести к тому, что устройства получают различные изменения, но содержимое считается контекстуальным эквивалентом для всех устройств в развертывании.

Все Windows обновления существуют как один из следующих производных типов: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) и [speededQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).

Наследует от [softwareUpdateReference](../resources/windowsupdates-softwareupdatereference.md). Базовый тип [для featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) и [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).

Это абстрактный тип.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsUpdateReference"
}
```

