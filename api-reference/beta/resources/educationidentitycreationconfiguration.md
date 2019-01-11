---
title: Тип ресурса educationIdentityCreationConfiguration
description: Задает параметры, при создании школа данных профиля удостоверений. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут создаваться в каталоге.
localization_priority: Normal
ms.openlocfilehash: 86624c7203dc6425372556572c40efda2bc1a53f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858865"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>Тип ресурса educationIdentityCreationConfiguration

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Задает параметры, при создании школа данных профиля удостоверений. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут создаваться в каталоге.

> **Примечание:** Если у вас есть синхронизации каталогов, включенным для синхронизации между локальной службы каталогов Active Directory и Azure Active Directory (Azure AD), используйте [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) ресурсов.

На основе [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **userDomains** | [educationIdentityDomain](educationidentitydomain.md) коллекции |  Задает список доменов для использования каждого типа пользователя.  |


## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
