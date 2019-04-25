---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа. Содержит такие сведения, как браузер устройств и сведения о ОС, если устройство управляется службой Azure AD.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d55e397cf6c892cd37aea930d446c630017a92
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543172"
---
# <a name="devicedetail-resource-type"></a>Тип ресурса Девицедетаил
Показывает сведения о устройствах, связанных с устройством, используемом для входа. Содержит такие сведения, как браузер устройств и сведения о ОС, если устройство управляется службой Azure AD.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Обозреватель|String|Указывает сведения, используемые для входа в браузер.|
|deviceId|String|Уникальный идентификатор устройства, используемого для входа.|
|displayName|String|Указывает имя устройства, используемого для входа.|
|isCompliant|Логический|Указывает, является ли устройство совместимым.|
|isManaged|Boolean|Указывает, является ли устройство управляемым.|
|operatingSystem|String|Указывает имя и версию операционной системы, которые используются для входа в систему.|
|trustType|String|Указывает, является ли устройство, на который выполнен вход, подключен к рабочему месту, AzureAD присоединен, присоединен к домену. |

## <a name="json-representation"></a>Представление в формате JSON

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
