---
title: Тип ресурса onPremisesExtensionAttributes
description: 'Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения. '
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: d43bcc3e838a9d7955954127dbc5960f45b60b15
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335936"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

Пространство имен: microsoft.graph

Возвращаемого типа **свойства onPremisesExtensionAttributes** объекта пользователя и [](user.md) **свойства extensionAttributes** [объекта устройства](device.md). Возвращает пятнадцать пользовательских свойств атрибута расширения.

В сущности [](user.md) пользователя и для пользователя **onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения. Для облачного пользователя (где **находится или находится onPremisesSyncEnabled** `false` `null`) эти свойства можно задать во время [создания](../api/user-post-users.md) или [обновления](../api/user-update.md). Если ранее пользователь с облачным интерфейсом синхронизировался с локальной службой Active Directory, управлять этими свойствами с помощью API microsoft Graph невозможно. Вместо этого ими можно управлять с помощью центра администрирования Exchange центра администрирования или Exchange Online V2 в PowerShell.

Свойство **extensionAttributes** объекта [устройства](device.md) управляется только в Azure AD во время [создания или](../api/device-post-devices.md) [обновления устройства](../api/device-update.md).

> **Примечание:** Эти атрибуты расширения также известны как Exchange пользовательские атрибуты 1-15.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|extensionAttribute1|Строка| Первый настраиваемый атрибут расширения. |
|extensionAttribute2|Строка| Второй настраиваемый атрибут расширения. |
|extensionAttribute3|String| Третий настраиваемый атрибут расширения. |
|extensionAttribute4|String| Четвертый настраиваемый атрибут расширения. |
|extensionAttribute5|String| Пятый настраиваемый атрибут расширения. |
|extensionAttribute6|Строка| Шестой настраиваемый атрибут расширения. |
|extensionAttribute7|Строка| Седьмой настраиваемый атрибут расширения. |
|extensionAttribute8|String| Восьмой настраиваемый атрибут расширения. |
|extensionAttribute9|Строка| Девятый настраиваемый атрибут расширения. |
|extensionAttribute10|String| Десятый настраиваемый атрибут расширения. |
|extensionAttribute11|Строка| Одиннадцатый настраиваемый атрибут расширения. |
|extensionAttribute12|String| Двенадцатый настраиваемый атрибут расширения. |
|extensionAttribute13|String| Тринадцатый настраиваемый атрибут расширения. |
|extensionAttribute14|Строка| Четырнадцатый настраиваемый атрибут расширения. |
|extensionAttribute15|String| Пятнадцатый настраиваемый атрибут расширения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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