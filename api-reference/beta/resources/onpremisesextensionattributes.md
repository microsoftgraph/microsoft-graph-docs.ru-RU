---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: d4fb2ca7361234abd5128ed331f1d0c3a9e13420
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766364"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **onPremisesExtensionAttributes** объекта пользователя содержит [15](user.md) пользовательских свойств атрибута расширения. Для **пользователя onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения. Для облачного пользователя (где **находится onPremisesSyncEnabled)** эти свойства можно задать при создании `false` или [обновлении.](../api/user-update.md) [](../api/user-post-users.md) Если ранее пользователь с облачным интерфейсом синхронизировался с локальной службой Active Directory, управлять этими свойствами с помощью API microsoft Graph невозможно. Вместо этого ими можно управлять через центр администрирования Exchange или Exchange Online V2 в PowerShell.


> **Примечание:** Эти атрибуты расширения также известны как Exchange пользовательские атрибуты 1-15.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|extensionAttribute1|String| Первый настраиваемый атрибут расширения. |
|extensionAttribute2|String| Второй настраиваемый атрибут расширения. |
|extensionAttribute3|String| Третий настраиваемый атрибут расширения. |
|extensionAttribute4|String| Четвертый настраиваемый атрибут расширения. |
|extensionAttribute5|Строка| Пятый настраиваемый атрибут расширения. |
|extensionAttribute6|String| Шестой настраиваемый атрибут расширения. |
|extensionAttribute7|String| Седьмой настраиваемый атрибут расширения. |
|extensionAttribute8|Строка| Восьмой настраиваемый атрибут расширения. |
|extensionAttribute9|String| Девятый настраиваемый атрибут расширения. |
|extensionAttribute10|String| Десятый настраиваемый атрибут расширения. |
|extensionAttribute11|Строка| Одиннадцатый настраиваемый атрибут расширения. |
|extensionAttribute12|String| Двенадцатый настраиваемый атрибут расширения. |
|extensionAttribute13|String| Тринадцатый настраиваемый атрибут расширения. |
|extensionAttribute14|Строка| Четырнадцатый настраиваемый атрибут расширения. |
|extensionAttribute15|Строка| Пятнадцатый настраиваемый атрибут расширения. |

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


