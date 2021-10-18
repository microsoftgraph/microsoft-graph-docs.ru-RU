---
title: Тип ресурса dataSubject
description: Содержит сведения, связанные с темой поиска контента.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: cefcd13dbd36c23cd014979fedce118861b58632
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457741"
---
# <a name="datasubject-resource-type"></a>Тип ресурса dataSubject

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, связанные с темой поиска контента. Этот ресурс является открытым типом и поддерживает добавление свойств добавления; например, ID клиента.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|email|String|Электронная почта субъекта данных.|
|firstName|String|Имя субъекта данных.|
|lastName|String|Фамилия субъекта данных.|
|место жительства|String|Страна или регион проживания. Сведения о проживании высчитываться только для внутренней отчетности, но не для поиска контента.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dataSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSubject",
  "email": "String",
  "firstName": "String",
  "lastName": "String",
  "residency": "String",
  "SSN": "String"
}
```

