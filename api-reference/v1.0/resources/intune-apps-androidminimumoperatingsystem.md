---
title: Тип ресурса androidMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2402ad007b794e7d6824e52cce8ff7144c6c33b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560874"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>Тип ресурса androidMinimumOperatingSystem

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения Android.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v4_0|Логический|Версия 4.0 или выше.|
|v4_0_3|Логический|Версия 4.0.3 или выше.|
|v4_1|Логический|Версия 4.1 или выше.|
|v4_2|Логический|Версия 4.2 или выше.|
|v4_3|Логический|Версия 4.3 или выше.|
|v4_4|Логический|Версия 4.4 или выше.|
|v5_0|Логический|Версия 5.0 или выше.|
|v5_1|Boolean|Версия 5.1 или выше.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true
}
```



