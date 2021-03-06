---
title: тип ресурса agreementFile
description: Представляет настраиваемый файл соглашений об использовании, который клиент управляет с Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 843870db12d9cdec518c18288adce76ea4b2dcf5
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761746"
---
# <a name="agreementfile-resource-type"></a>тип ресурса agreementFile

Пространство имен: microsoft.graph

Представляет настраиваемый файл соглашений об использовании, который клиент управляет с Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли это файл по умолчанию).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|Данные, которые представляют условия использования документа PDF. Только для чтения.|
|fileName|String|Имя файла соглашения (например, TOU.pdf). Только для чтения.|
|id|String|Идентификатор файла соглашения. Только для чтения.|
|isDefault|Boolean|Если ни один из языков не соответствует предпочтениям клиента, указывает, что это файл соглашения по умолчанию. Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как по умолчанию. Только для чтения.|
|language|String|Язык файла соглашения в формате languagecode2-country/regioncode2. languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1. country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US). Только для чтения.|
|isMajorVersion|Boolean|Указывает, является ли файл соглашения основным обновлением версии. Обновления основных версий недействительны для принятия соглашения на соответствующем языке. |
|createdDateTime|DateTimeOffset|Время даты, представляющее момент создания файла. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
|displayName|String|Локализованное отображение имени файла политики соглашения. Локализованное имя отображения отображается конечным пользователям, которые просматривают соглашение.

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.agreementFile",
  "keyProperty": "id"
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


