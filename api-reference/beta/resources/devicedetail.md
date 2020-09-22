---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 69d8d1e2314021752a5f1a0ab3650d8176ecc8dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049851"
---
# <a name="devicedetail-resource-type"></a>Тип ресурса Девицедетаил

Пространство имен: Microsoft. Graph указывает сведения о устройстве, связанные с устройством, используемом для входа. Содержит такие сведения, как браузер устройств и сведения о ОС, если устройство управляется службой Azure AD.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Обозреватель|Строка|Указывает сведения, используемые для входа в браузер.|
|deviceId|String|Уникальный идентификатор устройства, используемого для входа.|
|displayName|Строка|Указывает имя устройства, используемого для входа.|
|isCompliant|Boolean|Указывает, является ли устройство совместимым.|
|isManaged|Boolean|Указывает, является ли устройство управляемым.|
|operatingSystem|String|Указывает имя и версию операционной системы, которые используются для входа в систему.|
|trustType|String|Указывает, является ли устройство, на который выполнен вход, подключен к рабочему месту, AzureAD присоединен, присоединен к домену. |

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


