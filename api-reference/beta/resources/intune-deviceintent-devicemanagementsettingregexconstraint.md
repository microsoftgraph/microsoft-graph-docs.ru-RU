---
title: Тип ресурса Девицеманажементсеттингрежексконстраинт
description: Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0f9a04583bfb9b28546e9057f0530f72558a0be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364637"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттингрежексконстраинт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения


Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|выражений|String|Шаблон регулярного выражения, с которым выполняется сравнение|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```



