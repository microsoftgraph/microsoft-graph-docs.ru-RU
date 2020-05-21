---
title: Тип ресурса Едукатионидентитиматчингконфигуратион
description: Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fd42bc30a1cc1cee34685bc0f33815f3a00d0120
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336029"
---
# <a name="educationidentitymatchingconfiguration-resource-type"></a>Тип ресурса Едукатионидентитиматчингконфигуратион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.

> **Примечание:** При выборе этого ресурса пользователи не создаются.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **матчингоптионс** | Коллекция [Microsoft. Graph. едукатионидентитиматчингоптионс](educationidentitymatchingoptions.md) | Сопоставление между учетной записью пользователя и параметрами, которые необходимо использовать для уникальной идентификации пользователя, для которого необходимо выполнить обновление. |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
