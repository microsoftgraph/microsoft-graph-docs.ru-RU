---
title: Тип ресурса Едукатионидентитиматчингконфигуратион
description: Определяет параметры для согласованных удостоверений профиля данных учебного заведения. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: da1c5fa65305e23b8483825103117c523c51edd7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435035"
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
