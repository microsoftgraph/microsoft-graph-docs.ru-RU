---
title: тип ресурса assignmentFilterSupportedProperty
description: Представляет сведения о свойстве, поддерживаемом при разработке правила AssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed8ec505d314207a57fe3b743357e4217255db0d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265636"
---
# <a name="assignmentfiltersupportedproperty-resource-type"></a>тип ресурса assignmentFilterSupportedProperty

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет сведения о свойстве, поддерживаемом при разработке правила AssignmentFilter.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dataType|String|Тип данных указанного свойства.|
|isCollection|Логический|Указывает, является ли свойство типом коллекции или нет.|
|name|String|Имя свойства.|
|propertyRegexConstraint|String|Строка Regex для проверки значения свойства.|
|supportedOperators|[коллекция assignmentFilterOperator](../resources/intune-policyset-assignmentfilteroperator.md)|Список всех поддерживаемых операторов в этом свойстве.|
|supportedValues|Коллекция String|Список всех поддерживаемых значений для этого правильного, пустого, если все поддерживается.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterSupportedProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterSupportedProperty",
  "dataType": "String",
  "isCollection": true,
  "name": "String",
  "propertyRegexConstraint": "String",
  "supportedOperators": [
    "String"
  ],
  "supportedValues": [
    "String"
  ]
}
```




