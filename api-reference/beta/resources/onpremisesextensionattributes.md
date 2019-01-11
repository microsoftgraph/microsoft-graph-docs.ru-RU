---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** удостоверение пользователя содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения. Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.
localization_priority: Normal
ms.openlocfilehash: 44589338e25e01cb483df6bfa3c1e078e352f5ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868161"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Свойство **onPremisesExtensionAttributes** удостоверение [пользователя](user.md) содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения. Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|extensionAttribute1|Строка| Первый атрибут настраиваемые расширения. |
|extensionAttribute2|Строка| Второй атрибут настраиваемые расширения. |
|extensionAttribute3|Строка| Третий атрибут настраиваемые расширения. |
|extensionAttribute4|Строка| Четвертая атрибут настраиваемые расширения. |
|extensionAttribute5|Строка| Атрибут пятый настраиваемые расширения. |
|extensionAttribute6|Строка| Атрибут шестой настраиваемые расширения. |
|extensionAttribute7|Строка| Атрибут седьмой настраиваемые расширения. |
|extensionAttribute8|Строка| Атрибут восьмому настраиваемые расширения. |
|extensionAttribute9|Строка| Атрибут девятого настраиваемые расширения. |
|extensionAttribute10|Строка| Десятое атрибут настраиваемые расширения. |
|extensionAttribute11|Строка| Атрибут eleventh настраиваемые расширения. |
|extensionAttribute12|Строка| Атрибут twelfth настраиваемые расширения. |
|extensionAttribute13|Строка| Атрибут thirteenth настраиваемые расширения. |
|extensionAttribute14|Строка| Атрибут fourteenth настраиваемые расширения. |
|extensionAttribute15|Строка| Атрибут пятнадцатого настраиваемые расширения. |

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
