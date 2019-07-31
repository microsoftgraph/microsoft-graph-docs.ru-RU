---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: be4b03b28c80e07a5a05e1131c557d1abc643824
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999670"
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





