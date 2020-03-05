---
title: Тип ресурса Девицеманажементексчанжедевицекласс
description: Класс устройства в Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4304fb138ede5cf35db07bbb08814f3d8fcf532f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527745"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>Тип ресурса Девицеманажементексчанжедевицекласс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс устройства в Exchange.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя класса устройств, на который влияет это правило.|
|type|[девицеманажементексчанжеакцессрулетипе](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|Тип устройства, на которое влияет это правило, например Model, Family. Возможные значения: `family`, `model`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```



