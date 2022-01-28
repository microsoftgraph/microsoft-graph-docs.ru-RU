---
title: тип ресурса teamworkConnection
description: Представляет сведения о состоянии подключения устройства с Microsoft Teams и его периферийных устройств.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a02096ce1a807d4d75db5ba12b40488ef268bb36
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262504"
---
# <a name="teamworkconnection-resource-type"></a>тип ресурса teamworkConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о состоянии подключения устройства с Microsoft Teams и его периферийных устройств.[](../resources/teamworkdevice.md)
Состояние подключения полезно при расчете состояния устройства, когда необходимое периферийное устройство не подключено должным образом, состояние здоровья устройства меняется до критического состояния.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|connectionStatus|teamworkConnectionStatus|Указывает, подключен ли компонент или периферийное устройство или его состояние неизвестно. Допустимые значения: `unknown`, `connected`, `disconnected`, `unknownFutureValue`.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения состояния. Например, указывает _на подключение с_ момента отключения `connected`  `disconnected`и отключения состояния.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConnection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConnection",
  "connectionStatus": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

