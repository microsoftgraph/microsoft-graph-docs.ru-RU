---
title: Тип ресурса deviceDetail
description: Указывает сведения об устройстве, связанные с устройством, используемым для регистрации.
localization_priority: Normal
author: spunukol
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 00859ab80f022464be57b38cc62e9ab1a6c1b5a4444f7d066ffd7c06d84a63e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213440"
---
# <a name="devicedetail-resource-type"></a>Тип ресурса deviceDetail

Пространство имен: microsoft.graph указывает сведения об устройстве, связанном с устройством, используемым для регистрации. Включает сведения, такие как браузер устройства и сведения об ОС, если устройство управляется Azure AD.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Обозреватель|String|Указывает сведения браузера, используемые для регистрации.|
|deviceId|String|Относится к UniqueID устройства, используемого для регистрации.|
|displayName|Строка|Ссылается на имя устройства, используемого для регистрации.|
|isCompliant|Boolean|Указывает, является ли устройство совместимым или нет.|
|isManaged|Boolean|Указывает, управляется устройство или нет.|
|operatingSystem|String|Указывает имя и версию ОС, используемые для регистрации.|
|trustType|String|Указывает сведения о том, присоединилось ли устройство к рабочему месту, к AzureAD присоединились, к домену присоединились. |

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


