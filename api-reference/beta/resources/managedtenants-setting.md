---
title: параметр типа ресурса
description: Представляет параметр, используемый в базовой линии.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2545dc6aa11668359fa9dda636412d36f8d92de1
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403164"
---
# <a name="setting-resource-type"></a>параметр типа ресурса

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметр, используемый в базовой линии.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя отображения для параметра. Обязательный. Только для чтения.|
|jsonValue|String|Значение для параметра, сериализированного как строка JSON. Обязательный. Только для чтения.|
|overwriteAllowed|Boolean|Флаг, указывающий, можно ли переопредить существующие конфигурации при применении. Обязательный. Только для чтения.|
|valueType|managementParameterValueType|Тип данных для параметра. Возможные значения: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`. Обязательный. Только для чтения.|

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
