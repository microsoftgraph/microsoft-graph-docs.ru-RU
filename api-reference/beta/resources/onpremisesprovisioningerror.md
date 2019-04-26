---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибки синхронизации каталогов для сущностей контактов пользователя, группы или организации при синхронизации локальных каталогов с Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568852"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Тип ресурса onPremisesProvisioningError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибки синхронизации каталогов для сущностей контактов [пользователя](user.md), [группы](group.md)или [Организации](orgcontact.md) при синхронизации локальных каталогов с Azure Active Directory.

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
