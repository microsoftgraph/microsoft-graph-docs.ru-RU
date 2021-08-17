---
title: тип ресурса win32LobAppProductCodeRule
description: Сложный тип для хранения данных правил кода продукта и версии для приложения LOB Win32. Это правило не поддерживается в качестве правила требования.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54e910a8df3da47e1452fa8492e45c3f9c642c78808cde77ef901174df70c07d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224903"
---
# <a name="win32lobappproductcoderule-resource-type"></a>тип ресурса win32LobAppProductCodeRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения данных правил кода продукта и версии для приложения LOB Win32. Это правило не поддерживается в качестве правила требования.


Наследует [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|Тип правила, указывающий цель правила. Унаследованный от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Возможные значения: `detection`, `requirement`.|
|productCode|String|Код продукта приложения.|
|productVersionOperator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|Оператор сравнения версий продукта. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|productVersion|String|Значение сравнения версии продукта.|

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




