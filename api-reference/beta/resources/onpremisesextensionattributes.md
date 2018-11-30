---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** удостоверение пользователя содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения. Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.
ms.openlocfilehash: 547fc8ac19059611f5983a8b5ee0bd905f130f79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080303"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Свойство **onPremisesExtensionAttributes** удостоверение [пользователя](user.md) содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения. Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->