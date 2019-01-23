---
title: Тип ресурса variableManagementConditionExpression
description: Оценивает условие состояние управления как логическое выражение.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5e7efd0c8213f40d1dfb5f86d2f86c999069d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399628"
---
# <a name="variablemanagementconditionexpression-resource-type"></a>Тип ресурса variableManagementConditionExpression

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Оценивает условие состояние управления как логическое выражение.


Наследуется от [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managementConditionId|String|Идентификатор условия управления, которая используется для оценки выражения.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```




