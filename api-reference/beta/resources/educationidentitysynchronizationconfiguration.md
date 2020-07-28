---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c3531999065abc22cc0ecb1870b4bd1bb5f45b7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435021"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>Тип ресурса Едукатионидентитисинчронизатионконфигуратион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.

## <a name="derived-types"></a>Производные типы

| Тип                                                                                | Описание                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [едукатионидентитиматчингконфигуратион](educationidentitymatchingconfiguration.md) | Используйте этот тип для **согласования с существующими** учетными записями пользователей в Azure Active Directory. |
| [едукатионидентитикреатионконфигуратион](educationidentitycreationconfiguration.md) | Используйте этот тип для **создания новых** учетных записей пользователей в Azure Active Directory.                              |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{}
```
