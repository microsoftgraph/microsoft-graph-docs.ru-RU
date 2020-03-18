---
title: Тип ресурса Девицеманажементексчанжедевицекласс
description: Класс устройства в Exchange.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 384fa172c255ec3f21ec0088c2b9f4ab025768ce
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779032"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a>Тип ресурса Девицеманажементексчанжедевицекласс

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



