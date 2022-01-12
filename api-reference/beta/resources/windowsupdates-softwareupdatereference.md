---
title: тип ресурса softwareUpdateReference
description: Представляет определенный контент обновления.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 9278900d85bc1ec6fc626200f0bf814dd3097b34
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860427"
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

