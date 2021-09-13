---
title: тип ресурса deviceHealthScriptIntegerParameter
description: Свойства параметра скрипта Integer.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de488a0a84b94f554863d63bbc80482d9ce6da2f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59144324"
---
# <a name="devicehealthscriptintegerparameter-resource-type"></a>тип ресурса deviceHealthScriptIntegerParameter

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Свойства параметра скрипта Integer.


Наследует от [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя парама, унаследованной от [устройстваHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|description|String|Описание парама, унаследованной от [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|isRequired|Boolean|Требуется ли перенаследование парама с [устройстваHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|applyDefaultValueWhenNotAssigned|Логический|Применение defaultValue при не назначении унаследованных от [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|
|defaultValue|Int32|Значение по умолчанию параметра Integer. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptIntegerParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptIntegerParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": 1024
}
```



