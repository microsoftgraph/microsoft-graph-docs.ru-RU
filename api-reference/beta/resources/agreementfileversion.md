---
title: Тип ресурса Агриментфилеверсион
description: Представляет настраиваемую версию локализованных файлов политик условий соглашения об использовании в Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: rajadineshmurugesan-microsoft
ms.openlocfilehash: 04adb9f549fd7bbad2a628bbc2d205f9dd10e240
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2020
ms.locfileid: "49555670"
---
# <a name="agreementfileversion-resource-type"></a>Тип ресурса Агриментфилеверсион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемую версию условий файла соглашений об использовании, которую клиент управляет с помощью Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Create agreementFileLocalization](../api/agreementfilelocalization-post-agreementfilelocalizations.md) | [agreementfilelocalization](agreementfilelocalization.md) | Create a new agreementFileLocalization. |
| [List agreementFileLocalizations](../api/agreementfilelocalization-list.md) | [agreementfilelocalization](agreementfilelocalization.md) collection | Get an agreementFileLocalization object collection. |
| [Get agreementFileLocalization](../api/agreementfilelocalization-get.md) | [agreementfilelocalization](agreementfilelocalization.md) | Read properties and relationships of an agreementFileLocalization object. |
| [List agreementFileVersions](../api/agreementfileversion-list.md) | [agreementfileversion](agreementfileversion.md) collection | Get an agreementFileVersion object collection. |
| [Get agreementFileVersion](../api/agreementfileversion-get.md) | [agreementfileversion](agreementfileversion.md) | Read properties and relationships of an agreementFileVersion object. |
-->

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fileData|[агриментфиледата](agreementfiledata.md)|Данные, представляющие условия использования PDF-документа. Только для чтения.|
|fileName|String|Имя файла соглашения (например, TOU.pdf). Только для чтения.|
|id|String|Только для чтения.|
|isDefault|Boolean|Указывает, является ли этот файл соглашением по умолчанию, если ни одна из культур не соответствует параметрам клиента. Если ни один из файлов не помечен как используемый по умолчанию, первый из них будет считаться используемым по умолчанию. Только для чтения.|
|language|String|Язык и региональные параметры файла соглашения в формате languagecode2-Country/regioncode2. languagecode2 это код из двух букв в нижнем регистре, производный от стандарта ISO 639-1. страна или regioncode2 является производной от стандарта ISO 3166 и обычно состоит из двух прописных букв или тега языка BCP-47 (например, EN-US). Только для чтения.|
|исмажорверсион|Логический|Указывает, является ли файл соглашения основным обновлением версии. Основные обновления версий делают недействительными принятие соглашений на соответствующем языке. |
|createdDateTime|DateTimeOffset|Дата и время создания файла. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|versions|[agreementFileVersion](agreementfileversion.md) collection|The version history for the localized agreement file.|
-->

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileVersion"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": "Boolean",
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
