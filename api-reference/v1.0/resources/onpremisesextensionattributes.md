---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения. Для **пользователя onPremisesSyncEnabled** этот набор свойств освоен в локальном Active Directory и синхронизирован с Azure AD и является только для чтения. Для облачного пользователя (где **onPremisesSyncEnabled** является ложным), эти свойства могут быть заданы во время создания или обновления.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c8e44879b3248cab502ee2aeabdaa732a2b35e1f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718959"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

Пространство имен: microsoft.graph

Свойство **onPremisesExtensionAttributes** объекта пользователя содержит [15](user.md) пользовательских свойств атрибута расширения. Для **пользователя onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения. Для облачного пользователя (где **onPremisesSyncEnabled** является ложным), эти свойства могут быть заданы во время создания или обновления.

> **Примечание:** Эти атрибуты расширения также известны как пользовательские атрибуты Exchange 1-15.

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
|extensionAttribute9|String| Девятый настраиваемый атрибут расширения. |
|extensionAttribute10|String| Десятый настраиваемый атрибут расширения. |
|extensionAttribute11|String| Одиннадцатый настраиваемый атрибут расширения. |
|extensionAttribute12|String| Двенадцатый настраиваемый атрибут расширения. |
|extensionAttribute13|String| Тринадцатый настраиваемый атрибут расширения. |
|extensionAttribute14|String| Четырнадцатый настраиваемый атрибут расширения. |
|extensionAttribute15|String| Пятнадцатый настраиваемый атрибут расширения. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

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

