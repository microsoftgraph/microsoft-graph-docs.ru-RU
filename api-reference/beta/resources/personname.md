---
title: Тип ресурса personName
description: Тип ресурса personName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6212721774b9b7bc47a4e312d438f1b001a90bef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521906"
---
# <a name="personname-resource-type"></a>Тип ресурса personName

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о расширенных именах, предоставленных пользователем или связанными с их учетной записью.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод                                     | Возвращаемый тип                 | Описание                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [Получение personName](../api/personname-get.md) | [personName](personname.md) | Чтение свойств и связей объекта personName. |
| [обновление](../api/personname-update.md).      | [personName](personname.md) | Обновление объекта personName.                               |
| [удаление](../api/personname-delete.md);      | Нет                        | Удаление объекта personName.                               |

## <a name="properties"></a>Свойства

| Свойство     | Тип                              | Описание |
|:-------------|:----------------------------------|:------------|
|displayName   |Строка                             | Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства. |
|первыми         |String                             | Имя пользователя.                                                                                      |
|initials      |String                             | Инициалы пользователя.                                                                                        |
|лангуажетаг   |String                             | Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.                        |
|Фамили          |String                             | Фамилия пользователя.                                                                                       |
|маиден        |String                             | Маиден имя пользователя.                                                                                     |
|назван        |String                             | Миддлие имя пользователя.                                                                                    | 
|прозвищ      |String                             | Псевдоним пользователя.                                                                                        |
|произношение |[йомиперсоннаме](yomipersonname.md)| Руководство по произношению имени пользователя.                                                                 |
|суффикс        |String                             | Обозначения, используемые после имени пользователя (например, "доктор").                                                             |
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