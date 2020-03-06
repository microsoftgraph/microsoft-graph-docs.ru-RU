---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа. Сюда входят такие сведения, как браузер устройств и операционная система, а также, является ли устройство управляемым Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8730c6fefebadbd2c64937366c7b7de41537b11c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531674"
---
# <a name="devicedetail-resource-type"></a>Тип ресурса Девицедетаил

Пространство имен: microsoft.graph

Показывает сведения о устройствах, связанных с устройством, используемом для входа. Сюда входят такие сведения, как браузер устройств и операционная система, а также, является ли устройство управляемым Azure AD.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Обозреватель|Строка|Указывает сведения о браузере, используемом для входа.|
|deviceId|String|Указывает уникальный идентификатор устройства, используемого для входа.|
|displayName|Строка|Указывает на имя устройства, используемого для входа.|
|isCompliant|Boolean|Указывает, является ли устройство совместимым.|
|isManaged|Boolean|Указывает, является ли устройство управляемым.|
|operatingSystem|Строка|Указывает имя и версию операционной системы, используемую для входа.|
|trustType|Строка|Сведения о том, является ли устройство, на котором выполнен вход, присоединено к рабочему месту, AzureAD присоединено к домену. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
