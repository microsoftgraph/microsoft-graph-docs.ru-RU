---
title: тип ресурса win32LobAppRegistryRule
description: Сложный тип для хранения данных правил реестра для приложения LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c88346a755174af041e716c92e2d88e13d63d6463dd9b732e8ee6647e455e995
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152609"
---
# <a name="win32lobappregistryrule-resource-type"></a>тип ресурса win32LobAppRegistryRule

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения данных правил реестра для приложения LOB Win32.


Наследует [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|Тип правила, указывающий цель правила. Унаследованный от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Возможные значения: `detection`, `requirement`.|
|check32BitOn64System|Логический|Значение, указывающее, следует ли искать 32-битный реестр в 64-битных системах.|
|keyPath|String|Полный путь записи реестра, содержащей значение для обнаружения.|
|valueName|String|Имя значения реестра для обнаружения.|
|operationType|[win32LobAppRegistryRuleOperationType](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|Тип операции реестра. Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|Оператор обнаружения реестра. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|String|Значение сравнения реестра.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRule",
  "ruleType": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




