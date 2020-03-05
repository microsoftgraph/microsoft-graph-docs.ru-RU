---
title: Тип ресурса Девицеманажементсеттингстрингленгсконстраинт
description: Ограничение, ограничивающее заданный диапазон длины строки
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f78206495b4694b19a7558df4ab790c24b8f658b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528774"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттингстрингленгсконстраинт

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, ограничивающее заданный диапазон длины строки


Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|минимумленгс|Int32|Минимальная разрешенная длина строки|
|максимумленгс|Int32|Максимально допустимая длина строки|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```



