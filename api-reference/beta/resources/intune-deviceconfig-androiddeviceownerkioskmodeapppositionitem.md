---
title: тип ресурса androidDeviceOwnerKioskModeAppPositionItem
description: Элемент в списке позиций приложений, который задает порядок элементов на управляемом домашнем экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4e658e4289f2d08dbb8552bd3496db6d80a9161d5d065d88a11691061340d29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245116"
---
# <a name="androiddeviceownerkioskmodeapppositionitem-resource-type"></a>тип ресурса androidDeviceOwnerKioskModeAppPositionItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Элемент в списке позиций приложений, который задает порядок элементов на управляемом домашнем экране

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|position|Int32|Расположение элемента в сетке. Допустимые значения от 0 до 9999999|
|item|[androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)|Пункт, который нужно расположить|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
  "position": 1024,
  "item": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
    "label": "String",
    "link": "String"
  }
}
```




