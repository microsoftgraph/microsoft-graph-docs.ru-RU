---
title: тип ресурса templateParameter
description: Представляет параметр, использованный в шаблоне управления.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a2fe8cc543f60e2e862af65b9e47f6a84389e453
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791877"
---
# <a name="templateparameter-resource-type"></a>тип ресурса templateParameter

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметр, использованный в шаблоне управления.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|String|Описание параметра шаблона. Необязательно. Только для чтения.|
|displayName|String|Имя отображения параметра шаблона. Обязательное. Только для чтения.|
|jsonAllowedValues|String|Допустимые значения параметра шаблона, представленные сериализированной строкой JSON. Необязательно. Только для чтения.|
|jsonDefaultValue|String|Значение по умолчанию для параметра шаблона, представленное последовательной строкой JSON. Обязательное. Только для чтения.|
|valueType|managementParameterValueType|Тип данных для параметра шаблона.. Возможные значения: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`. Обязательное. Только для чтения.|

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
