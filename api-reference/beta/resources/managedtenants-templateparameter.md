---
title: тип ресурса templateParameter
description: Представляет параметр, использованный в шаблоне управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f533bc375e2d7e4a1e4ef2f7f801f248c1801c4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403160"
---
# <a name="templateparameter-resource-type"></a>тип ресурса templateParameter

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметр, использованный в шаблоне управления.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание параметра шаблона. Необязательно. Только для чтения.|
|displayName|String|Имя отображения параметра шаблона. Обязательный. Только для чтения.|
|jsonAllowedValues|String|Допустимые значения параметра шаблона, представленные сериализированной строкой JSON. Необязательно. Только для чтения.|
|jsonDefaultValue|String|Значение по умолчанию для параметра шаблона, представленное последовательной строкой JSON. Обязательный. Только для чтения.|
|valueType|managementParameterValueType|Тип данных для параметра шаблона.. Возможные значения: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`. Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.templateParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.templateParameter",
  "displayName": "String",
  "description": "String",
  "valueType": "String",
  "jsonDefaultValue": "String",
  "jsonAllowedValues": "String"
}
```
