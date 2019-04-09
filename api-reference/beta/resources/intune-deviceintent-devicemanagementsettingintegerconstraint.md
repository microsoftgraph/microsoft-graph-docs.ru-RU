---
title: Тип ресурса Девицеманажементсеттингинтежерконстраинт
description: Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f67e3507d58e2208c7f0022724516f1646ad0fd
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523639"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a>Тип ресурса Девицеманажементсеттингинтежерконстраинт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ограничение, ограничивающее диапазон допустимых значений для параметра целого числа


НаСледуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Минимумвалуе|Int32|Минимально допустимое значение|
|Максимумвалуе|Int32|Максимальное разрешенное значение|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```







