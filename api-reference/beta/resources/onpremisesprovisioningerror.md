---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователя, группы или организационной сущностей для контактов, при синхронизации локальных каталогов в Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512733"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Тип ресурса onPremisesProvisioningError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ошибок синхронизации службы каталогов для объектов [пользователей](user.md), [группы](group.md)или [организации контакта](orgcontact.md) при синхронизации локальных каталогов в Azure Active Directory.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория Ошибка подготовки. Примечание: В настоящее время доступно только один значений. Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным. Такое же значение для свойства содержат другие объекты. |
|occurredDateTime|DateTimeOffset| Дата и время, в котором возникла ошибка. |
|propertyCausingError|String| Имя свойства каталогов, вызывает ошибку. Текущий возможные значения: *UserPrincipalName* или *ProxyAddress* |
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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesprovisioningerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
