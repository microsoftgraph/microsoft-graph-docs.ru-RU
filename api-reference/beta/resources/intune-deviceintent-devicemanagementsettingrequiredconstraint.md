---
title: Тип ресурса Девицеманажементсеттингрекуиредконстраинт
description: Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd70066465fcde31ba12ff1a7deb96a41a6786e9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420087"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттингрекуиредконстраинт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, которое применяет определенный обязательный параметр, отличный от NULL/undefine/пустая строка/не настроен


Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|нотконфигуредвалуе|String|Список значений, которые не настроены для параметра|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRequiredConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRequiredConstraint",
  "notConfiguredValue": "String"
}
```



