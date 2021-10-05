---
title: тип ресурса softwareUpdateReference
description: Представляет определенный контент обновления.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 13e71a5b08100a74884ae0f4f69b69b86bec9b2c
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115314"
---
# <a name="softwareupdatereference-resource-type"></a>тип ресурса softwareUpdateReference

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный контент обновления.

В развертывании одно и то же **программное обеспечениеUpdateReference** может привести к тому, что устройства получают различные изменения обновления, но контент считается контекстуальным эквивалентом для всех устройств в развертывании.

Все ссылки на обновление программного обеспечения существуют как один из следующих производных типов: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) и [speededQualityUpdateReference.](../resources/windowsupdates-expeditedqualityupdatereference.md)

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

