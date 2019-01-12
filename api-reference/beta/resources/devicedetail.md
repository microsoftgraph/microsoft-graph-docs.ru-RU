---
title: Тип ресурса deviceDetail
description: Указывает, связанные с устройства, используемый для подписи сведений об устройстве. Включает в себя данные о браузере устройства и сведения о операционной системы, если устройство является управляемым Azure AD.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d55e397cf6c892cd37aea930d446c630017a92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971363"
---
# <a name="devicedetail-resource-type"></a>Тип ресурса deviceDetail
Указывает, связанные с устройства, используемый для подписи сведений об устройстве. Включает в себя данные о браузере устройства и сведения о операционной системы, если устройство является управляемым Azure AD.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Обозреватель|String|Указывает информацию браузеров, используемых для вход в систему.|
|deviceId|String|Ссылается на уникальный идентификатор устройства, используемого для подписи в.|
|displayName|String|— Имя устройства, используемый для подписи в.|
|isCompliant|Boolean|Указывает, является ли устройство совместимым.|
|isManaged|Boolean|Указывает, если устройство является управляемым или нет.|
|operatingSystem|String|Указывает имя операционная система и версия, используемый для подписи в.|
|trustType|String|Указывает сведения о того, является ли устройство выполнил вход присоединился к месту в состав AzureAD, присоединенный к домену. |

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
