---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для сущностей пользователей и групп при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3fd16b43d35cb12e7b9c7f82dc59f940994bc1b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035750"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Тип ресурса onPremisesProvisioningError

Представляет ошибки синхронизации каталогов для сущностей [пользователей](user.md) и [групп](group.md) при синхронизации локальных каталогов с Azure Active Directory.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория ошибки подготовки. Примечание. в настоящее время существует только одно возможное значение. Возможное значение: *пропертиконфликт* — указывает, что значение свойства не является уникальным. Другие объекты содержат одно и то же значение свойства. |
|Оккурреддатетиме|DateTimeOffset| Дата и время возникновения ошибки. |
|Пропертикаусинжеррор|String| Имя свойства каталога, вызвавшего ошибку. Текущие возможные значения: *userPrincipalName* или *proxyAddress* |
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
