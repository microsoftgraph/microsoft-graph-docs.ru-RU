---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации службы каталогов для контактных сущностями пользователя, группы или организации при синхронизации локального каталога с Azure Active Directory.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: japere
ms.openlocfilehash: e4e3469ae371568ac9010d1d3879f68c92340460
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133982"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Тип ресурса onPremisesProvisioningError

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибки синхронизации службы каталогов для [](orgcontact.md) пользовательских, [](user.md)групповых или организационных контактных сущностями при синхронизации локального каталога с Azure Active Directory. [](group.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория ошибки при предоставлении. Примечание. В настоящее время существует только одно возможное значение. Возможное *значение: PropertyConflict* — указывает, что значение свойства не уникально. Другие объекты содержат такое же значение свойства. |
|occurredDateTime|DateTimeOffset| Дата и время, когда произошла ошибка. |
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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


