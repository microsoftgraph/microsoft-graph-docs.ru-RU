---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователей и групп сущностей при синхронизации каталогов в локальной для Azure Active Directory.
ms.openlocfilehash: 7d5b15d99559ddf5b7692b7eac9664de7ec50f1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028387"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Тип ресурса onPremisesProvisioningError

Представляет ошибок синхронизации службы каталогов для [пользователей](user.md) и [групп](group.md) сущностей при синхронизации локальных каталогов в Azure Active Directory.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория Ошибка подготовки. Примечание: В настоящее время доступно только один значений. Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным. Такое же значение для свойства содержат другие объекты. |
|occurredDateTime|DateTimeOffset| Дата и время, в котором возникла ошибка. |
|propertyCausingError|String| Имя свойства каталогов, вызывает ошибку. Текущий возможные значения: *UserPrincipalName* или *ProxyAddress* |
|value|String| Значение свойства, вызывая ошибки. |

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