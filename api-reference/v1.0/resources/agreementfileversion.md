---
title: тип ресурса agreementFileVersion
description: Представляет настраиваемую версию локализованных файлов политик условий соглашения об использовании в Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: rajadineshmurugesan-microsoft
ms.openlocfilehash: c590736ea50f589e3f2d87b8d9e0269580f34810
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761739"
---
# <a name="agreementfileversion-resource-type"></a>тип ресурса agreementFileVersion

Пространство имен: microsoft.graph

Представляет настраиваемую версию файла соглашений об использовании, который клиент управляет с Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли это файл по умолчанию).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|Данные, которые представляют условия использования документа PDF. Только для чтения.|
|fileName|String|Имя файла соглашения (например, TOU.pdf). Только для чтения.|
|id|String|Идентификатор объекта AgreementFileVersion. Только для чтения.|
|isDefault|Boolean|Если ни один из языков не соответствует предпочтениям клиента, указывает, является ли это файл соглашения по умолчанию. Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как по умолчанию. Только для чтения.|
|language|String|Язык файла соглашения в формате languagecode2-country/regioncode2. languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1. country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US). Только для чтения.|
|isMajorVersion|Boolean|Указывает, является ли файл соглашения основным обновлением версии. Обновления основных версий недействительны для принятия соглашения на соответствующем языке. |
|createdDateTime|DateTimeOffset|Время даты, представляющее момент создания файла. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
|displayName|String|Локализованное отображение имени файла политики соглашения. Локализованное имя отображения отображается конечным пользователям, которые просматривают соглашение.

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
