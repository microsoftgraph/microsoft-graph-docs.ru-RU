---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8d19eefbc9ca7f9a750ddf5ebe231cf57366d765
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472147"
---
# <a name="devicedetail-resource-type"></a>Тип ресурса Девицедетаил

Пространство имен: Microsoft. Graph указывает сведения о устройстве, связанные с устройством, используемом для входа. Содержит такие сведения, как браузер устройств и сведения о ОС, если устройство управляется службой Azure AD.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Обозреватель|String|Указывает сведения, используемые для входа в браузер.|
|deviceId|String|Уникальный идентификатор устройства, используемого для входа.|
|displayName|String|Указывает имя устройства, используемого для входа.|
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
