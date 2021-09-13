---
title: тип ресурса assignmentFilterSupportedProperty
description: Представляет сведения о свойстве, поддерживаемом при разработке правила AssignmentFilter.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 339f220b9508487735e2473133e61c2682263c05
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074950"
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
|supportedValues|Коллекция объектов string|Список всех поддерживаемых значений для этого правильного, пустого, если все поддерживается.|

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



