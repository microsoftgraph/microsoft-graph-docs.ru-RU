---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff87c376bd88e49d8dc2c3d4657607e7bddcb503
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783279"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>Тип ресурса Бинариманажементкондитионекспрессион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Выражение условия управления, вычисляемое с помощью бинарной операции.


Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[бинариманажементкондитионекспрессионоператортипе](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|Оператор, используемый для оценки бинарной операции. Возможные значения: `or`, `and`.|
|фирстоперанд|[манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)|Первый операнд бинарной операции.|
|секондоперанд|[манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)|Второй операнд бинарной операции.|

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



