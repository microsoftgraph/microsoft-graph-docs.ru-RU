---
title: Тип ресурса agreementFile
description: Представляет настраиваемый файл соглашения об условиях использования, управляемый клиентом с Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: a48fa216ff9051e04bf57046387fd3e94619f7b2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314952"
---
# <a name="agreementfile-resource-type"></a>Тип ресурса agreementFile

Пространство имен: microsoft.graph

Представляет настраиваемый файл соглашения об условиях использования, управляемый клиентом с Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).

Наследуется [от agreementFileProperties](agreementfileproperties.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Дата и время создания файла. Тип метки времени представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|displayName|String|Локализованное отображаемое имя файла политики соглашения. Локализованное отображаемое имя отображается пользователям, просматривая соглашение. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|fileData|[agreementFileData](agreementfiledata.md)|Данные, которые представляют условия использования PDF-документа. Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|fileName|String|Имя файла соглашения (например, TOU.pdf). Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|id|String|Идентификатор объекта agreementFileVersion. Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|isDefault|Boolean|Если ни один из языков не соответствует предпочтениям клиента, указывает, является ли это файл соглашения по умолчанию. Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как файл по умолчанию. Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|isMajorVersion|Boolean|Указывает, является ли файл соглашения основным обновлением версии. Обновления основных версий недействительны для принятия условий соглашения на соответствующем языке. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|language|String|Язык файла соглашения в формате languagecode2-country/regioncode2. Languagecode2 — это двухбуквенный код в нижнем регистре, производный от ISO 639-1, а "country/regioncode2" является производным от ISO 3166 и обычно состоит из двух прописных букв или языкового тега BCP-47. Например, английский (США) — `en-US`. Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Локализации|[Коллекция agreementFileLocalization](agreementfilelocalization.md)|Локализованная версия файлов соглашения об условиях использования, вложенных в соглашение.|


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


