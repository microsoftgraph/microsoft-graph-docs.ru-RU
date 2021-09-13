---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения. Для **пользователя onPremisesSyncEnabled** этот набор свойств освоен в локальном Active Directory и синхронизирован с Azure AD и является только для чтения. Для облачного пользователя (где **onPremisesSyncEnabled** является ложным), эти свойства можно Exchange Online. Атрибуты читают только в Microsoft Graph.
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 5b1ef010abec3ab0e3e4c5279654603faed4e220
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072010"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

Пространство имен: microsoft.graph

Свойство **onPremisesExtensionAttributes** объекта пользователя содержит [15](user.md) пользовательских свойств атрибута расширения. Для **пользователя onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения. Для облачного пользователя (где **находится onPremisesSyncEnabled)** эти свойства можно задать при создании `false` или [обновлении.](../api/user-update.md) [](../api/user-post-users.md)

> **Примечание:** Эти атрибуты расширения также известны как Exchange пользовательские атрибуты 1-15.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|extensionAttribute1|Строка| Первый настраиваемый атрибут расширения. |
|extensionAttribute2|String| Второй настраиваемый атрибут расширения. |
|extensionAttribute3|String| Третий настраиваемый атрибут расширения. |
|extensionAttribute4|String| Четвертый настраиваемый атрибут расширения. |
|extensionAttribute5|Строка| Пятый настраиваемый атрибут расширения. |
|extensionAttribute6|String| Шестой настраиваемый атрибут расширения. |
|extensionAttribute7|Строка| Седьмой настраиваемый атрибут расширения. |
|extensionAttribute8|Строка| Восьмой настраиваемый атрибут расширения. |
|extensionAttribute9|Строка| Девятый настраиваемый атрибут расширения. |
|extensionAttribute10|Строка| Десятый настраиваемый атрибут расширения. |
|extensionAttribute11|String| Одиннадцатый настраиваемый атрибут расширения. |
|extensionAttribute12|Строка| Двенадцатый настраиваемый атрибут расширения. |
|extensionAttribute13|Строка| Тринадцатый настраиваемый атрибут расширения. |
|extensionAttribute14|String| Четырнадцатый настраиваемый атрибут расширения. |
|extensionAttribute15|String| Пятнадцатый настраиваемый атрибут расширения. |

## <a name="json-representation"></a>Представление в формате JSON

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

