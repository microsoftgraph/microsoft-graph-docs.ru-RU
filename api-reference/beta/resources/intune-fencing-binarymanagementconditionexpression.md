---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a5384a2f5b830323aaf89f2b29e0377c9199d8b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941333"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>Тип ресурса Бинариманажементкондитионекспрессион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Выражение условия управления, вычисляемое с помощью бинарной операции.


Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[Бинариманажементкондитионекспрессионоператортипе](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|Оператор, используемый для оценки бинарной операции. Возможные значения: `or`, `and`.|
|Фирстоперанд|[Манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)|Первый операнд бинарной операции.|
|Секондоперанд|[Манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)|Второй операнд бинарной операции.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```




