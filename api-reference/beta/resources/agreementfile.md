---
title: Тип ресурса agreementFile
description: Представляет настраиваемое условия использования соглашения файл, который управляет клиента с помощью Azure Active Directory (Azure AD). Содержит метаданные о файле соглашения (например, имя, язык, и его файл по умолчанию).
ms.openlocfilehash: f099715fd25fbae9d7b2a94d6de841b8766c30e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078613"
---
# <a name="agreementfile-resource-type"></a>Тип ресурса agreementFile

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
| Свойство     | Тип        | Description |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|Данные, представляющие условия использования PDF-документа. Только для чтения.|
|fileName|String|Имя файла соглашения (например, TOU.pdf). Только для чтения.|
|id|String|Только для чтения.|
|isDefault|Логический|Указывает, является ли файл соглашения по умолчанию Если ни одна из культур совпадает с клиентом. Если ни один из файлов помечены как по умолчанию, первый будет рассматриваться как значение по умолчанию. Только для чтения.|
|language|String|Язык и региональные параметры соглашения файла в формате languagecode2-страны/regioncode2. languagecode2 — это строчная двухбуквенный код, производный от ISO 639-1. Страна/regioncode2 является производным от ISO 3166 и обычно состоит из двух прописных букв или тег языка BCP 47 (например, en US). Только для чтения.|

## <a name="relationships"></a>Связи
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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
