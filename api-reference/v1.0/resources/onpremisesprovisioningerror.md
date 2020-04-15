---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для группы пользователей и контактных ресурсов при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e170fa0e86cfb6ebfcdf63b371c6a67bb8766b80
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468341"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Тип ресурса onPremisesProvisioningError

Пространство имен: microsoft.graph

Представляет ошибки синхронизации каталогов для [пользователей](user.md), [групп](group.md) и [orgContact](orgcontact.md) ресурсов при синхронизации локальных каталогов с Azure Active Directory.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория ошибки подготовки. Примечание. в настоящее время существует только одно возможное значение. Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным. Другие объекты содержат одно и то же значение свойства. |
|оккурреддатетиме|DateTimeOffset| Дата и время возникновения ошибки. |
|пропертикаусинжеррор|String| Имя свойства каталога, вызвавшего ошибку. Текущие возможные значения: *userPrincipalName* или *proxyAddress* |
|value|String| Значение свойства, вызвавшего ошибку. |

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
