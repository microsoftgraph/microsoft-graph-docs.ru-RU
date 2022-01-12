---
title: monitoringSettings resource type
description: Параметры автоматизированного мониторинга и реагирования в развертывании.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: c00f7e714b68595ce1debbf155ec802f0f579f23
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61810439"
---
# <a name="monitoringsettings-resource-type"></a>monitoringSettings resource type

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры автоматизированного мониторинга и реагирования в развертывании.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|monitoringRules|[коллекция microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md)|Указывает правила, по которым сигналы мониторинга могут вызывать действия при развертывании. Правила объединяются с помощью "или".|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringSettings",
  "monitoringRules": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
    }
  ]
}
```

