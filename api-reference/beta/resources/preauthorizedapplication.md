---
title: Тип ресурса preAuthorizedApplication
description: Представляет приложение и запрашиваемые разрешения для неявного согласия. Необходимо, чтобы администратор предоставил согласие на применение приложения. Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями. Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя. Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: 22945589341066f4609d47773cb04426774648fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563632"
---
# <a name="preauthorizedapplication-resource-type"></a>Тип ресурса preAuthorizedApplication

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложение и запрашиваемые разрешения для неявного согласия. Необходимо, чтобы администратор предоставил согласие на применение приложения. Преаусоризедаппликатионс не требуют от пользователя согласия с запрошенными разрешениями. Разрешения, перечисленные в Преаусоризедаппликатионс, не требуют согласия пользователя. Однако все дополнительные запрошенные разрешения, не указанные в Преаусоризедаппликатионс, требуют согласия пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|appId|String| Уникальный идентификатор приложения. |
|Пермиссионидс|Коллекция String| Уникальный идентификатор для [публишедпермиссионскопе](permissionscope.md) или [аппроле](approle.md) , необходимых для приложения. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/preauthorizedapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
