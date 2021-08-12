---
title: onPremisesProvisioningError resource type
description: Представляет ошибки синхронизации каталогов для группы пользователей и контактных ресурсов при синхронизации локального каталога с Azure Active Directory.
localization_priority: Normal
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7c3e50469b9625c62d587f75fa778a3408699952eda4a204b8aaccbb73a80e2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216674"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError resource type

Пространство имен: microsoft.graph

Представляет ошибки синхронизации каталогов для [](group.md) ресурсов [пользователя,](user.md)группы и [orgContact](orgcontact.md) при синхронизации локального каталога с Azure Active Directory.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория ошибки подготовка. Примечание. В настоящее время существует только одно возможное значение. Возможное значение: *PropertyConflict* — указывает, что значение свойства не является уникальным. Другие объекты содержат такое же значение для свойства. |
|occurredDateTime|DateTimeOffset| Дата и время, в которые произошла ошибка. |
|propertyCausingError|String| Имя свойства каталога, вызываемого ошибкой. Текущие возможные значения: *UserPrincipalName или* *ProxyAddress* |
|value|String| Значение свойства, вызываемого ошибкой. |

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

