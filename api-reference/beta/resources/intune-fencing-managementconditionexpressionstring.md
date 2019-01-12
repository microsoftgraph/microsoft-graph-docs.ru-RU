---
title: Тип ресурса managementConditionExpressionString
description: Строковое выражение условия управления является представлением строковое выражение условия управления.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 872282914dc57be4e8e9bc7d476e7767907ec913
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968850"
---
# <a name="managementconditionexpressionstring-resource-type"></a>Тип ресурса managementConditionExpressionString

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Строковое выражение условия управления является представлением строковое выражение условия управления.

Наследуется от [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|value|Строка|Управление условие оператора выражения строковое значение.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```





