---
title: Тип ресурса Девицеманажементсеттингрежексконстраинт
description: Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bb05c0f58d3c30b18bd240c8047d34a3977e85b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943309"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттингрежексконстраинт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения


Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|выражений|Строка|Шаблон регулярного выражения, с которым выполняется сравнение|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```




