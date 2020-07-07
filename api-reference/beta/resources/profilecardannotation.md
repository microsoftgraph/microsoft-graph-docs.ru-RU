---
title: Тип ресурса Профилекарданнотатион
description: Позволяет администратору настраивать внешний вид выбранных полей в карточке профиля Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 973732dc92527dcf3795b8796e1c817ba880836c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051062"
---
# <a name="profilecardannotation-resource-type"></a>Тип ресурса Профилекарданнотатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для задания настраиваемого отображаемого имени для полей, которые находятся в общей программе Microsoft 365 People експериинце. Администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для языков, которые они поддерживают в Организации.

## <a name="properties"></a>Свойства

| Свойство     | Тип                                                            | Описание                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|displayName   |String                                                           | Если этот параметр задан, значение этого поля используется картой профиля в качестве метки свойства по умолчанию (например, "центр затрат"). |
|Локализация |Коллекция [дисплайнамелокализатион](displaynamelocalization.md) | Каждый ресурс в этой коллекции представляет локализованное значение имени атрибута для определенного языка, используемого в качестве метки по умолчанию для этого языкового стандарта. Например, пользователь с `no-NB` клиентом получает значение "Костнадс Sent" в качестве метки атрибута, а не "центр затрат".|

## <a name="json-representation"></a>Представление в формате JSON

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
