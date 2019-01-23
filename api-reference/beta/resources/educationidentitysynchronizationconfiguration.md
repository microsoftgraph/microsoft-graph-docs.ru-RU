---
title: Тип ресурса educationIdentitySynchronizationConfiguration
description: Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций. Производные классы определите поведение синхронизации удостоверения. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 59dca28f82de0340aa289c6ea96ef5e252f60e85
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412907"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>Тип ресурса educationIdentitySynchronizationConfiguration

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций. Производные классы определите поведение синхронизации удостоверения. Ниже приведены производные типы.

## <a name="derived-types"></a>Производные типы
| Тип | Описание | 
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Этот тип используется в соответствии с существующим учетным записям пользователей в Azure Active Directory (Azure AD). |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Этот тип используется для создания новых учетных записей пользователей в Azure AD. |

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```
