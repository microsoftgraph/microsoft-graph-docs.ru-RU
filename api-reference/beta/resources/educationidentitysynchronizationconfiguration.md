---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e282a9701eaae04aae33d9fd9efc9b86f7df3635
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972679"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>Тип ресурса Едукатионидентитисинчронизатионконфигуратион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.

## <a name="derived-types"></a>Производные типы
| Тип | Описание |
|:-|:-|
| [**Едукатионидентитиматчингконфигуратион**](educationidentitymatchingconfiguration.md) | Используйте этот тип для согласования с существующими учетными записями пользователей в Azure Active Directory (Azure AD). |
| [**Едукатионидентитикреатионконфигуратион**](educationidentitycreationconfiguration.md) | Используйте этот тип для создания новых учетных записей пользователей в Azure AD. |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

