---
title: Тип ресурса educationIdentityDomain
description: 'Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя. Домен ресурсов является частью конфигурации создания удостоверений. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4eb9e5b58f62a23dbe1b450c2ec6b9d2f94970ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395652"
---
# <a name="educationidentitydomain-resource-type"></a>Тип ресурса educationIdentityDomain

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет сопоставление между тип образования пользователя и домен, к которому принадлежит учетная запись пользователя. Домен ресурсов является частью [удостоверения Создание конфигурации](educationidentitycreationconfiguration.md). 

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **appliesTo** | string |  Тип роли пользователя для назначения лицензий. Возможные значения: `student`, `teacher`.      |
| **name** | строка |  Представляет учетную запись пользователя домена.         |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
