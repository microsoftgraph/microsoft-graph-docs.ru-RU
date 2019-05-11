---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eee7a423ca412eb4ee86e3f0b5a5f13ec786a690
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941201"
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

## <a name="relationships"></a>Связи
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




