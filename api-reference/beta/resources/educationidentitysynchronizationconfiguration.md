---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e193c798f1f3fbc5d4d1c9d8c7b96eed7d39cf9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095361"
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


