---
title: тип ресурса deviceHealthScriptStringParameter
description: Свойства параметра скрипта String.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6b96f7eb1796ce170c8334fc653b1565f716cad
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785404"
---
# <a name="devicehealthscriptstringparameter-resource-type"></a>тип ресурса deviceHealthScriptStringParameter

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Свойства параметра скрипта String.


Наследует от [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя парама, унаследованной от [устройстваHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|description|Строка|Описание парама, унаследованной от [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|isRequired|Boolean|Требуется ли перенаследование парама с [устройстваHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|applyDefaultValueWhenNotAssigned|Boolean|Применение defaultValue при не назначении унаследованных от [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|defaultValue|Строка|Значение параметра строки по умолчанию|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptStringParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": "String"
}
```



