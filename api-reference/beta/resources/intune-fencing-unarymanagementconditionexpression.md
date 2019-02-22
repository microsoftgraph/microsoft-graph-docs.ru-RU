---
title: Тип ресурса Унариманажементкондитионекспрессион
description: Выражение условия управления, вычисляемое с использованием унарной операции.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9802cb8162973ecdaa387a29c70d1baa7aec4b8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164220"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>Тип ресурса Унариманажементкондитионекспрессион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Выражение условия управления, вычисляемое с использованием унарной операции.


НаСледуется от [манажементкондитионекспрессионмодел](../resources/intune-fencing-managementconditionexpressionmodel.md)

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




