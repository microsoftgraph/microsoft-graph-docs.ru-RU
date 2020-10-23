---
title: Тип ресурса Девицехеалсскриптпараметер
description: Базовые свойства параметра скрипта.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a11915af80b10944fe6a3573d5293c19e3fc0357
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729350"
---
# <a name="devicehealthscriptparameter-resource-type"></a>Тип ресурса Девицехеалсскриптпараметер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовые свойства параметра скрипта.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Имя параметра|
|description|Строка|Описание параметра|
|isRequired|Boolean|Является ли параметр обязательным|
|апплидефаултвалуевхеннотассигнед|Логический|Применяется ли значение DefaultValue при отсутствии назначения|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true
}
```





