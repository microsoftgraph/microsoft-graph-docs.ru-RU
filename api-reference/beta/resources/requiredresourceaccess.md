---
title: Тип ресурса Рекуиредресаурцеакцесс
description: Задает набор областей разрешений OAuth 2,0 и ролей приложения в указанном ресурсе, к которому приложение требует доступ. Указанные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** ) при вызове приложения-ресурса. Свойство **рекуиредресаурцеакцесс** объекта Application представляет собой коллекцию **рекиредресаурцеакцесс**.
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563182"
---
# <a name="requiredresourceaccess-resource-type"></a>Тип ресурса Рекуиредресаурцеакцесс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает набор областей разрешений OAuth 2,0 и ролей приложения в указанном ресурсе, к которому приложение требует доступ. Указанные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** ) при вызове приложения-ресурса. Свойство **рекуиредресаурцеакцесс** объекта [Application](application.md) представляет собой коллекцию **рекиредресаурцеакцесс**.


## <a name="json-representation"></a>Описание в формате JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|resourceAccess|Коллекция [ресаурцеакцесс](resourceaccess.md)|Список областей разрешений OAuth 2.0 и ролей приложений, которые требуются приложению из указанного ресурса.|
|Ресаурцеаппид|String|Уникальный идентификатор ресурса, доступ к которому требуется приложению.  Он должен быть равен **AppID** , объявленному в целевом приложении ресурсов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
