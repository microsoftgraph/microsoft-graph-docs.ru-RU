---
title: параметр типа ресурса
description: Представляет параметр, используемый в базовой линии.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 53eaf2dd4c3e97e183083f1a6c0d127ffbaefafd
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861296"
---
# <a name="setting-resource-type"></a>параметр типа ресурса

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметр, используемый в базовой линии.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя отображения для параметра. Обязательный. Только для чтения.|
|jsonValue|String|Значение для параметра, сериализированного как строка JSON. Обязательное. Только для чтения.|
|overwriteAllowed|Логический|Флаг, указывающий, можно ли переопредить существующие конфигурации при применении. Обязательный. Только для чтения.|
|valueType|managementParameterValueType|Тип данных для параметра. Возможные значения: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`. Обязательное. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.setting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.setting",
  "displayName": "String",
  "overwriteAllowed": "Boolean",
  "valueType": "String",
  "jsonValue": "String"
}
```
