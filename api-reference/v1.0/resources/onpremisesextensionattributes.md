---
title: Тип ресурса onPremisesExtensionAttributes
description: 'Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения. '
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 36388026cdce3b11a7ccdbf32b94d76b19d2a68e
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560760"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Тип ресурса onPremisesExtensionAttributes

Пространство имен: microsoft.graph

Возвращаемого типа **свойства onPremisesExtensionAttributes** объекта пользователя и **свойства extensionAttributes** [объекта устройства.](device.md) [](user.md) Возвращает пятнадцать пользовательских свойств атрибута расширения.

В [](user.md) сущности пользователя и для пользователя **onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения. Для облачного пользователя (где **находится onPremisesSyncEnabled)** эти свойства можно задать при создании `false` или [обновлении.](../api/user-update.md) [](../api/user-post-users.md) Если ранее пользователь с облачным интерфейсом синхронизировался с локальной службой Active Directory, управлять этими свойствами с помощью API microsoft Graph невозможно. Вместо этого ими можно управлять через центр администрирования Exchange или Exchange Online V2 в PowerShell.

Свойство **extensionAttributes** объекта [устройства](device.md) управляется только в Azure AD во время [создания](../api/device-post-devices.md) или [обновления устройства.](../api/device-update.md)

> **Примечание:** Эти атрибуты расширения также известны как Exchange пользовательские атрибуты 1-15.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|extensionAttribute1|Строка| Первый настраиваемый атрибут расширения. |
|extensionAttribute2|Строка| Второй настраиваемый атрибут расширения. |
|extensionAttribute3|Строка| Третий настраиваемый атрибут расширения. |
|extensionAttribute4|Строка| Четвертый настраиваемый атрибут расширения. |
|extensionAttribute5|Строка| Пятый настраиваемый атрибут расширения. |
|extensionAttribute6|Строка| Шестой настраиваемый атрибут расширения. |
|extensionAttribute7|Строка| Седьмой настраиваемый атрибут расширения. |
|extensionAttribute8|Строка| Восьмой настраиваемый атрибут расширения. |
|extensionAttribute9|Строка| Девятый настраиваемый атрибут расширения. |
|extensionAttribute10|Строка| Десятый настраиваемый атрибут расширения. |
|extensionAttribute11|Строка| Одиннадцатый настраиваемый атрибут расширения. |
|extensionAttribute12|Строка| Двенадцатый настраиваемый атрибут расширения. |
|extensionAttribute13|Строка| Тринадцатый настраиваемый атрибут расширения. |
|extensionAttribute14|Строка| Четырнадцатый настраиваемый атрибут расширения. |
|extensionAttribute15|Строка| Пятнадцатый настраиваемый атрибут расширения. |

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