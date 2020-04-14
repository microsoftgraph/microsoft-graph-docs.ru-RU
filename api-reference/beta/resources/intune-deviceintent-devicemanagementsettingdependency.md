---
title: Тип ресурса Девицеманажементсеттингдепенденци
description: Сведения о зависимостях для параметра
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9014b3618562717c2cc9522c388034ad81213a4c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420124"
---
# <a name="devicemanagementsettingdependency-resource-type"></a>Тип ресурса Девицеманажементсеттингдепенденци

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о зависимостях для параметра

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|дефинитионид|String|Идентификатор определения параметра зависит от|
|провероч|Коллекция [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)|Коллекция ограничений для значения параметра зависимости|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ]
}
```



