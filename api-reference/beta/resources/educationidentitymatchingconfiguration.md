---
title: Тип ресурса Едукатионидентитиматчингконфигуратион
description: Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7c26ef1447272b88c59ec6992e41ae051439645e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095396"
---
# <a name="educationidentitymatchingconfiguration-resource-type"></a>Тип ресурса Едукатионидентитиматчингконфигуратион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.

> [!NOTE]
> При выборе этого ресурса пользователи не создаются.

## <a name="properties"></a>Свойства

| Свойство        | Тип                                                                                               | Описание                                                                                      |
| :-------------- | :------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------- |
| матчингоптионс | Коллекция [Microsoft. Graph. едукатионидентитиматчингоптионс](educationidentitymatchingoptions.md) | Сопоставление между учетной записью пользователя и параметрами, которые необходимо использовать для уникальной идентификации пользователя, для которого необходимо выполнить обновление. |

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
      "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
      "sourcePropertyName": "String",
      "targetPropertyName": "String",
      "targetDomain": "String"
    }
  ]
}
```


