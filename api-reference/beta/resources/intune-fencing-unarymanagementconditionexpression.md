---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5eb5e7ed67b0731cc795ab791c2463294764ead6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990108"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>Тип ресурса Унариманажементкондитионекспрессион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Выражение условия управления, вычисляемое с использованием унарной операции.


Наследуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[Унариманажементкондитионекспрессионоператортипе](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|Оператор, используемый в оценке унарной операции. Возможные значения: `not`.|
|начинается|[Манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)|Операнд унарной операции.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





