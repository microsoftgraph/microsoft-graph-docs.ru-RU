---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 713bb285e739d9182a982f02975a9b9f46761e3a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736518"
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

