---
title: Тип ресурса Профилекарданнотатион
description: Позволяет администратору настраивать внешний вид выбранных полей в карточке профиля Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 57b6378c811727676f7b34c1812955639598054b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973732"
---
# <a name="profilecardannotation-resource-type"></a>Тип ресурса Профилекарданнотатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для задания настраиваемого отображаемого имени для полей, которые находятся в общей программе Microsoft 365 People експериинце. Администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для языков, которые они поддерживают в Организации.

## <a name="properties"></a>Свойства

| Свойство     | Тип                                                            | Описание                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|displayName   |String                                                           | Если этот параметр задан, значение этого поля используется картой профиля в качестве метки свойства по умолчанию (например, "центр затрат"). |
|Локализация |Коллекция [дисплайнамелокализатион](displaynamelocalization.md) | Каждый ресурс в этой коллекции представляет локализованное значение имени атрибута для определенного языка, используемого в качестве метки по умолчанию для этого языкового стандарта. Например, пользователь с `no-NB` клиентом получает значение "Костнадс Sent" в качестве метки атрибута, а не "центр затрат".|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardAnnotation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "localizations": [
    {
      "displayName": "String",
      "languageTag": "String"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardAnnotation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


