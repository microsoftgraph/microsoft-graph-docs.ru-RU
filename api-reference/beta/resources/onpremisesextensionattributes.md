---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта user содержит пятнадцать свойств настраиваемого атрибута расширения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 2729d6d624f1bde304425229ccf4ae7df8ddf781
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052600"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **onPremisesExtensionAttributes** объекта [User](user.md) содержит пятнадцать свойств настраиваемого атрибута расширения. Для пользователя **onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальный каталог Active Directory, который синхронизируется с Azure AD и доступен только для чтения. Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.

> **Примечание:** Эти атрибуты расширения также называются пользовательскими атрибутами Exchange 1-15.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|extensionAttribute1|String| Первый настраиваемый атрибут расширения. |
|extensionAttribute2|String| Второй настраиваемый атрибут расширения. |
|extensionAttribute3|String| Третий настраиваемый атрибут расширения. |
|extensionAttribute4|String| Четвертый настраиваемый атрибут расширения. |
|extensionAttribute5|String| Пятый настраиваемый атрибут расширения. |
|extensionAttribute6|String| Шестой настраиваемый атрибут расширения. |
|extensionAttribute7|String| Седьмой настраиваемый атрибут расширения. |
|extensionAttribute8|String| Восьмой настраиваемый атрибут расширения. |
|extensionAttribute9|String| Девятый атрибут расширения. |
|extensionAttribute10|String| Десятый атрибут расширенной настройки. |
|extensionAttribute11|String| Одиннадцатый атрибут настраиваемого расширения. |
|extensionAttribute12|String| Двенадцатый настраиваемый атрибут расширения. |
|extensionAttribute13|String| Настраиваемый атрибут расширения сиртинс. |
|extensionAttribute14|String| Настраиваемый атрибут расширения фауртинс. |
|extensionAttribute15|String| Пятнадцатый настраиваемый атрибут расширения. |

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
  "suppressions": []
}
-->


