---
title: Тип ресурса educationIdentityMatchingConfiguration
description: Задает параметры для сопоставления школа данных профиля удостоверения. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут обновлены в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ee9f58c2f69882361ee105a1d7531bb5756e165
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977551"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>Тип ресурса educationIdentityMatchingConfiguration

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Задает параметры для сопоставления школа данных профиля удостоверения. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут обновлены в каталоге.

> **Примечание:** Пользователи не создаются при выборе этого ресурса.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **matchingOptions** | [educationIdentityMatchingOptions](educationidentitymatchingoptions.md) коллекции | Сопоставление учетной записи пользователя и параметры, используемые для уникальной идентификации пользователя для обновления. |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
