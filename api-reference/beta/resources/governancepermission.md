---
title: Тип ресурса governancePermission
description: 'Представляет, governanceSubject имеет разрешение на доступ к определенным governanceResource.  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643785"
---
# <a name="governancepermission-resource-type"></a>Тип ресурса governancePermission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет, [governanceSubject](../resources/governancesubject.md) имеет разрешение на доступ к определенным [governanceResource](../resources/governanceresource.md).  


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accessLevel|String|Уровень доступа. Допустимые значения: ``None``, ``UserRead``, ``AdminRead``, и ``AdminReadWrite``.|
|isActive|Boolean|Указывает, если инициатора запроса имеет назначения активная роль на уровне доступа.|
|isEligible|Boolean|Указывает, имеет ли инициатора запроса все назначения ролей право на уровне доступа.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
