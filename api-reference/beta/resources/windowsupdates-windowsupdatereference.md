---
title: тип ресурса windowsUpdateReference
description: Представляет конкретные Windows 10 обновления.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a25cc6995979922ed2e7a8fb8e7f74350dec71c5
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791996"
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

