---
title: Тип ресурса agreementFile
description: Представляет настраиваемое условия использования соглашения файл, который управляет клиента с помощью Azure Active Directory (Azure AD). Содержит метаданные о файле соглашения (например, имя, язык, и его файл по умолчанию).
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511431"
---
# <a name="agreementfile-resource-type"></a>Тип ресурса agreementFile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемое условия использования соглашения файл, который управляет клиента с помощью Azure Active Directory (Azure AD). Содержит метаданные о файле соглашения (например, имя, язык, и его файл по умолчанию).

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
|fileData|[agreementFileData](agreementfiledata.md)|Данные, представляющие условия использования PDF-документа. Только для чтения.|
|fileName|String|Имя файла соглашения (например, TOU.pdf). Только для чтения.|
|id|Строка|Только для чтения.|
|isDefault|Boolean|Указывает, является ли файл соглашения по умолчанию Если ни одна из культур совпадает с клиентом. Если ни один из файлов помечены как по умолчанию, первый будет рассматриваться как значение по умолчанию. Только для чтения.|
|language|String|Язык и региональные параметры соглашения файла в формате languagecode2-страны/regioncode2. languagecode2 — это строчная двухбуквенный код, производный от ISO 639-1. Страна/regioncode2 является производным от ISO 3166 и обычно состоит из двух прописных букв или тег языка BCP 47 (например, en US). Только для чтения.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
