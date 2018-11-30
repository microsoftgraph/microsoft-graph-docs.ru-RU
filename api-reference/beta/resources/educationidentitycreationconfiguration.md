---
title: Тип ресурса educationIdentityCreationConfiguration
description: Задает параметры, при создании школа данных профиля удостоверений. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут создаваться в каталоге.
ms.openlocfilehash: edbfa03bb574a1d8d9d4faaa2032ec82f6d20f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081829"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>Тип ресурса educationIdentityCreationConfiguration

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Задает параметры, при создании школа данных профиля удостоверений. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут создаваться в каталоге.

> **Примечание:** Если у вас есть синхронизации каталогов, включенным для синхронизации между локальной службы каталогов Active Directory и Azure Active Directory (Azure AD), используйте [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) ресурсов.

На основе [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
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