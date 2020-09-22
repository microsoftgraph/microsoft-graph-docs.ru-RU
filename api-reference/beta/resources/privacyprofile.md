---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: ab8d1d3282e3ebcc899e89701ab812e18c403e18
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070641"
---
# <a name="privacyprofile-resource-type"></a>Тип ресурса privacyProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.

## <a name="properties"></a>Свойства
| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|contactEmail|String| Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности. Не обязательное.|
|statementUrl|String| Допустимый формат URL-адреса, который начинается с http:// или https://. Максимальная длина составляет 255 символов. URL-адрес заявления о конфиденциальности организации. Не обязательное.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```


