---
title: onPremisesProvisioningError resource type
description: Представляет ошибки синхронизации каталогов для группы пользователей и контактных ресурсов при синхронизации локального каталога с Azure Active Directory.
ms.localizationpriority: medium
author: japere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f95b454b37913c407e949cc76cd01e48299e785
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071996"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError resource type

Пространство имен: microsoft.graph

Представляет ошибки синхронизации каталогов для [](group.md) ресурсов [пользователя,](user.md)группы и [orgContact](orgcontact.md) при синхронизации локального каталога с Azure Active Directory.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория ошибки подготовка. Примечание. В настоящее время существует только одно возможное значение. Возможное значение: *PropertyConflict* — указывает, что значение свойства не является уникальным. Другие объекты содержат такое же значение для свойства. |
|occurredDateTime|DateTimeOffset| Дата и время, в которые произошла ошибка. |
|propertyCausingError|Строка| Имя свойства каталога, вызываемого ошибкой. Текущие возможные значения: *UserPrincipalName или* *ProxyAddress* |
|value|String| Значение свойства, вызываемого ошибкой. |

## <a name="json-representation"></a>Представление в формате JSON
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

