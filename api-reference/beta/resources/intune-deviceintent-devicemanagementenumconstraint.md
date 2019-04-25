---
title: Тип ресурса Девицеманажементенумконстраинт
description: Ограничение, которое задает значение параметра, из разрешенного набора строк
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 457582a5160aa9e17beb06d3b169c3817d216e4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523303"
---
# <a name="devicemanagementenumconstraint-resource-type"></a>Тип ресурса Девицеманажементенумконстраинт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, которое задает значение параметра, из разрешенного набора строк


НаСледуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|values|Коллекция [девицеманажементенумвалуе](../resources/intune-deviceintent-devicemanagementenumvalue.md)|Список допустимых значений для этой строки|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumConstraint",
  "values": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumValue",
      "value": "String",
      "displayName": "String"
    }
  ]
}
```





