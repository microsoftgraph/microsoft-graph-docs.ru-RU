---
title: Тип ресурса Бинариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с помощью бинарной операции.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50092f7031719fb1050706ed81280a347638117d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568803"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>Тип ресурса Бинариманажементкондитионекспрессион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Выражение условия управления, вычисляемое с помощью бинарной операции.


НаСледуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[Бинариманажементкондитионекспрессионоператортипе](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|Оператор, используемый для оценки бинарной операции. Возможные значения: `or`, `and`.|
|Фирстоперанд|[Манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)|Первый операнд бинарной операции.|
|Секондоперанд|[Манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)|Второй операнд бинарной операции.|

## <a name="relationships"></a>Отношения
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





