---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30683c35ae92cd1172fd3a83ab8110b3b07c7afb53a33686db27911678441717
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243562"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>Тип ресурса iosMinimumOperatingSystem

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v8_0|Boolean|Версия 8.0 или выше.|
|v9_0|Boolean|Версия 9.0 или выше.|
|v10_0|Boolean|Версия 10.0 или выше.|
|v11_0|Boolean|Версия 11.0 или выше.|
|v12_0|Логический|Версия 12.0 или более поздней версии.|
|v13_0|Логическое|Версия 13.0 или более поздней версии.|
|v14_0|Логический|Версия 14.0 или более поздней версии.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true,
  "v13_0": true,
  "v14_0": true
}
```




