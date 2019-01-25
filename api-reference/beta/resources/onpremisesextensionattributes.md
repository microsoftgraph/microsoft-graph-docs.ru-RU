---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** удостоверение пользователя содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя onPremisesSyncEnabled этот набор свойств управляется в локальной службе Active Directory, синхронизирован с Azure AD и доступен только для чтения. Для исключительно облачных пользователей (где значением для onPremisesSyncEnabled является false) эти свойства можно задать при создании или обновлении.
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518242"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **onPremisesExtensionAttributes** удостоверение [пользователя](user.md) содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя onPremisesSyncEnabled этот набор свойств управляется в локальной службе Active Directory, синхронизирован с Azure AD и доступен только для чтения. Для исключительно облачных пользователей (где значением для onPremisesSyncEnabled является false) эти свойства можно задать при создании или обновлении.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|extensionAttribute1|String| Первый атрибут настраиваемые расширения. |
|extensionAttribute2|String| Второй атрибут настраиваемые расширения. |
|extensionAttribute3|String| Третий атрибут настраиваемые расширения. |
|extensionAttribute4|String| Четвертая атрибут настраиваемые расширения. |
|extensionAttribute5|String| Атрибут пятый настраиваемые расширения. |
|extensionAttribute6|String| Атрибут шестой настраиваемые расширения. |
|extensionAttribute7|String| Атрибут седьмой настраиваемые расширения. |
|extensionAttribute8|String| Атрибут восьмому настраиваемые расширения. |
|extensionAttribute9|String| Атрибут девятого настраиваемые расширения. |
|extensionAttribute10|String| Десятое атрибут настраиваемые расширения. |
|extensionAttribute11|String| Атрибут eleventh настраиваемые расширения. |
|extensionAttribute12|String| Атрибут twelfth настраиваемые расширения. |
|extensionAttribute13|String| Атрибут thirteenth настраиваемые расширения. |
|extensionAttribute14|String| Атрибут fourteenth настраиваемые расширения. |
|extensionAttribute15|String| Атрибут пятнадцатого настраиваемые расширения. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
