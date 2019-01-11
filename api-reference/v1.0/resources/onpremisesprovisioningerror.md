---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователей и групп сущностей при синхронизации каталогов в локальной для Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830669"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Тип ресурса onPremisesProvisioningError

Представляет ошибок синхронизации службы каталогов для [пользователей](user.md) и [групп](group.md) сущностей при синхронизации локальных каталогов в Azure Active Directory.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория Ошибка подготовки. Примечание: В настоящее время доступно только один значений. Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным. Такое же значение для свойства содержат другие объекты. |
|occurredDateTime|DateTimeOffset| Дата и время, в котором возникла ошибка. |
|propertyCausingError|Строка| Имя свойства каталогов, вызывает ошибку. Текущий возможные значения: *UserPrincipalName* или *ProxyAddress* |
|value|Строка| Значение свойства, вызывая ошибки. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
