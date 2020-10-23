---
title: Тип ресурса Девицехеалсскриптбулеанпараметер
description: Свойства параметра скрипта Буолеан.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87822b0e526a9101efc2317bce38b65909af3f25
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728190"
---
# <a name="devicehealthscriptbooleanparameter-resource-type"></a>Тип ресурса Девицехеалсскриптбулеанпараметер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Свойства параметра скрипта Буолеан.


Наследуется от [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя параметра, унаследованного от [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)|
|description|Строка|Описание параметра, унаследованного от [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)|
|isRequired|Boolean|Является ли параметр должен наследоваться от [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)|
|апплидефаултвалуевхеннотассигнед|Логический|Применяется ли значение DefaultValue при отсутствии назначенного наследования от [девицехеалсскриптпараметер](../resources/intune-devices-devicehealthscriptparameter.md)|
|Значение|Логический|Значение по умолчанию для параметра Boolean|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptBooleanParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptBooleanParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": true
}
```





