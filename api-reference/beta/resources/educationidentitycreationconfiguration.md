---
title: Тип ресурса Едукатионидентитикреатионконфигуратион
description: Определяет параметры создания удостоверений профиля School Data. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут созданы в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4dc03514e3d62f0dca096b0e669ada9247ff39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095403"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a>Тип ресурса Едукатионидентитикреатионконфигуратион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет параметры создания удостоверений профиля School Data. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут созданы в каталоге.

> [!WARNING]
> Если вы включили синхронизацию каталогов для синхронизации между локальной службой Active Directory и Azure Active Directory (Azure AD), используйте вместо этого ресурс [едукатионидентитиматчингконфигуратион](educationidentitymatchingconfiguration.md) .

Производный от [едукатионидентитисинчронизатионконфигуратион](educationidentitysynchronizationconfiguration.md).

## <a name="properties"></a>Свойства

| Свойство    | Тип                                                             | Описание                                    |
| :---------- | :--------------------------------------------------------------- | :--------------------------------------------- |
| усердомаинс | Коллекция [едукатионидентитидомаин](educationidentitydomain.md) | Задает список доменов для использования по типам пользователей. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
  "userDomains": [
    {
      "@odata.type": "microsoft.graph.educationIdentityDomain"
    }
  ]
}
```


