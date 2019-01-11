---
title: Тип ресурса educationIdentityMatchingConfiguration
description: Задает параметры для сопоставления школа данных профиля удостоверения. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут обновлены в каталоге.
localization_priority: Normal
ms.openlocfilehash: 807029f45875bdcf7691a112d515831f2f2283dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877940"
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
