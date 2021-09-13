---
title: Тип ресурса deviceDetail
description: Указывает сведения об устройстве, связанные с устройством, используемым для регистрации. Это включает сведения о браузере устройства и операционной системе, а также об управляемом устройстве Azure AD.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 91710dc5079bc879b8b23a8a3f5b621f4ecc1968
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089825"
---
# <a name="devicedetail-resource-type"></a>Тип ресурса deviceDetail

Пространство имен: microsoft.graph

Указывает сведения об устройстве, связанные с устройством, используемым для регистрации. Это включает сведения о браузере устройства и операционной системе, а также об управляемом устройстве Azure AD.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Обозреватель|Строка|Указывает сведения браузера, используемые для регистрации.|
|deviceId|String|Ссылается на UniqueID устройства, используемого для регистрации.|
|displayName|Строка|Ссылается на имя устройства, используемого для регистрации.|
|isCompliant|Boolean|Указывает, соответствует ли устройство.|
|isManaged|Boolean|Указывает, управляется ли устройство.|
|operatingSystem|String|Указывает имя операционной системы и версию, используемую для регистрации.|
|trustType|String|Предоставляет сведения о том, является ли подписанное устройство рабочим местом, AzureAD Joined, Domain Joined. |

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

