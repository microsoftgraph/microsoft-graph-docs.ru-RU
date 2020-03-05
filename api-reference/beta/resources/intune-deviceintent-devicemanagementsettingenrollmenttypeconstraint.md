---
title: Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт
description: Ограничение, которое применяет типы регистрации, примененные к параметру
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfea5505dc05ac037ced5d9b714edb53ed6f768d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528792"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттинженроллменттипеконстраинт

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, которое применяет типы регистрации, примененные к параметру


Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|енроллменттипес|Коллекция String|Список типов регистрации|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint",
  "enrollmentTypes": [
    "String"
  ]
}
```



