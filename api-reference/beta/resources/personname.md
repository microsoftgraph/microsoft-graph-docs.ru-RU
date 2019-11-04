---
title: Тип ресурса personName
description: Тип ресурса personName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aad97177a06933d2dd98c5cc94744450197f7dcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939602"
---
# <a name="personname-resource-type"></a>Тип ресурса personName

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о расширенных именах, предоставленных пользователем или связанными с их учетной записью.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод                                     | Возвращаемый тип                 | Описание                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [Получение personName](../api/personname-get.md) | [personName](personname.md) | Чтение свойств и связей объекта personName. |
| [Update](../api/personname-update.md)      | [personName](personname.md) | Обновление объекта personName.                               |
| [Delete](../api/personname-delete.md)      | Нет.                        | Удаление объекта personName.                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип                              | Описание |
|:-------------|:----------------------------------|:------------|
|displayName   |Строка                             | Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства. |
|первыми         |Строка                             | Имя пользователя.                                                                                      |
|initials      |String                             | Инициалы пользователя.                                                                                        |
|лангуажетаг   |Строка                             | Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.                        |
|Фамили          |Строка                             | Фамилия пользователя.                                                                                       |
|маиден        |Строка                             | Маиден имя пользователя.                                                                                     |
|назван        |Строка                             | Миддлие имя пользователя.                                                                                    | 
|прозвищ      |Строка                             | Псевдоним пользователя.                                                                                        |
|произношение |[йомиперсоннаме](yomipersonname.md)| Руководство по произношению имени пользователя.                                                                 |
|суффикс        |Строка                             | Обозначения, используемые после имени пользователя (например, "доктор").                                                             |
|title         |String                             | Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).                                            |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personName",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "initials": "String",
  "languageTag": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String",
  "nickname": "String",
  "pronunciation": {"@odata.type": "microsoft.graph.yomiPersonName"},
  "suffix": "String",
  "title": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->