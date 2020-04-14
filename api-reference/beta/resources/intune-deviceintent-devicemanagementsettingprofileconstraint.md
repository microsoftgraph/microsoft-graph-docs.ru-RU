---
title: Тип ресурса Девицеманажементсеттингпрофилеконстраинт
description: Ограничение на применение заданной метаданных профиля
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b181760ea01b1fc46437ba67f295e50138ef12d3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420117"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттингпрофилеконстраинт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение на применение заданной метаданных профиля


Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|source|String|Источник объекта|
|types|Коллекция объектов string|Коллекция типов, которые несет данный объект|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingProfileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingProfileConstraint",
  "source": "String",
  "types": [
    "String"
  ]
}
```



