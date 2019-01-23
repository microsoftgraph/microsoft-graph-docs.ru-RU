---
title: Тип ресурса iosMinimumOperatingSystem
description: Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4a97932c76a737aa1a98321feb429244228c97d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406943"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>Тип ресурса iosMinimumOperatingSystem

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v8_0|Boolean|Версия 8.0 или выше.|
|v9_0|Boolean|Версия 9.0 или выше.|
|v10_0|Boolean|Версия 10.0 или выше.|
|v11_0|Boolean|Версия 11.0 или выше.|
|v12_0|Логический|12.0 или более поздняя версия.|

## <a name="relationships"></a>Отношения
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
  "v12_0": true
}
```




