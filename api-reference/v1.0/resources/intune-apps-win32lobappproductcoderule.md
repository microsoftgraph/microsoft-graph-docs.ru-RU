---
title: Тип ресурса win32LobAppProductCodeRule
description: Сложный тип для хранения кода продукта и данных правила версий для бизнес-приложения Win32. Это правило не поддерживается в качестве правила для требования.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 101818fdea0dd87966abdd08d4cfbbffd1a81680
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080124"
---
# <a name="win32lobappproductcoderule-resource-type"></a>Тип ресурса win32LobAppProductCodeRule

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения кода продукта и данных правила версий для бизнес-приложения Win32. Это правило не поддерживается в качестве правила для требования.


Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|Тип правила, указывающий назначение правила. Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Возможные значения: `detection`, `requirement`.|
|productCode|String|Код продукта приложения.|
|продуктверсионоператор|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|Оператор сравнения версий продукта. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|productVersion|String|Значение сравнения версий продукта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeRule",
  "ruleType": "String",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```





