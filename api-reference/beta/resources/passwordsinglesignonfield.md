---
title: Тип ресурса Пассвордсинглесигнонфиелд
description: Поля для записи учетных данных для единого входа паролей
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d79f2347acabae0323e008a43adb7938d70d3768
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998196"
---
# <a name="passwordsinglesignonfield-resource-type"></a>Тип ресурса Пассвордсинглесигнонфиелд

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит поля для заполнения, используемые для заполнения учетных данных для единого входа на основе пароля.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|кустомизедлабел|String|Переопределение названий и подписей для настройки.|
|дефаултлабел|String|Метка, которая будет использоваться, если Кустомизедлабел не указан. Только для чтения.|
|fieldId|String|Идентификатор, используемый для идентификации типа поля. Это внутренний идентификатор, и возможные значения: `param_1` ,, `param_2` `param_userName` , `param_password` .|
|type|String|   Тип учетных данных. Возможные значения `text` : `password` .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnField",
  "baseType": null
}-->

```json
{
  "customizedLabel": "String",
  "defaultLabel": "String",
  "fieldId": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

