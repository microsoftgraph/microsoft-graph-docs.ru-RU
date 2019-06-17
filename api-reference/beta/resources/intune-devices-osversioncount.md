---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b8987017012d4db0756fc3d8a78efe99319d68
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963914"
---
# <a name="osversioncount-resource-type"></a>Тип ресурса Осверсионкаунт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество устройств с вредоносной программой для каждой версии ОС

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|osVersion|String|Версия ОС|
|deviceCount|Int32|Количество устройств с вредоносной программой для версии ОС|
|lastUpdateDateTime|DateTimeOffset|Метка времени последнего обновления числа устройств в формате UTC|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```





