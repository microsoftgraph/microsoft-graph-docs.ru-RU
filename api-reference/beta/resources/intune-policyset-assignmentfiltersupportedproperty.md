---
title: тип ресурса assignmentFilterSupportedProperty
description: Представляет сведения о свойстве, поддерживаемом при разработке правила AssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b8b8a5bc422c2d663d74ea7dc93b7353f10e65d3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786609"
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
|propertyRegexConstraint|Строка|Строка Regex для проверки значения свойства.|
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



