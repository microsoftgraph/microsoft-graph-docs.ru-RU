---
title: Тип ресурса Агриментфиле
description: Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ea78059ecf29f1cadb9634492ced726775f5614d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508375"
---
# <a name="agreementfile-resource-type"></a>Тип ресурса Агриментфиле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fileData|[агриментфиледата](agreementfiledata.md)|Данные, представляющие условия использования PDF-документа. Только для чтения.|
|fileName|String|Имя файла соглашения (например, Тау. PDF). Только для чтения.|
|id|String|Только для чтения.|
|isDefault|Boolean|Указывает, является ли этот файл соглашением по умолчанию, если ни одна из культур не соответствует параметрам клиента. Если ни один из файлов не помечен как используемый по умолчанию, первый из них будет считаться используемым по умолчанию. Только для чтения.|
|language|String|Язык и региональные параметры файла соглашения в формате languagecode2-Country/regioncode2. languagecode2 это код из двух букв в нижнем регистре, производный от стандарта ISO 639-1. страна или regioncode2 является производной от стандарта ISO 3166 и обычно состоит из двух прописных букв или тега языка BCP-47 (например, EN-US). Только для чтения.|

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
