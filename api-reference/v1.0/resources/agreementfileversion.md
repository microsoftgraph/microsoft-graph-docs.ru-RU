---
title: тип ресурса agreementFileVersion
description: Представляет настраиваемую версию локализованных файлов политик условий соглашения об использовании в Azure Active Directory Azure AD.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rajadineshmurugesan-microsoft
ms.openlocfilehash: 4942e920d273d950a2fd4cff412619f4eec5fed1
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651269"
---
# <a name="agreementfileversion-resource-type"></a>тип ресурса agreementFileVersion

Пространство имен: microsoft.graph

Представляет настраиваемую версию файла соглашений об использовании, который клиент управляет Azure Active Directory Azure AD. Он содержит метаданные о файле соглашения (например, имя, язык и является ли это файл по умолчанию).

Наследует от [agreementFileProperties](agreementfileproperties.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Время даты, представляющее момент создания файла. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|displayName|Строка|Локализованное отображение имени файла политики соглашения. Локализованное имя отображения отображается конечным пользователям, которые просматривают соглашение. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|fileData|[agreementFileData](agreementfiledata.md)|Данные, которые представляют условия использования документа PDF. Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|fileName|String|Имя файла соглашения (например, TOU.pdf). Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|id|String|Идентификатор объекта AgreementFileVersion. Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|isDefault|Boolean|Если ни один из языков не соответствует предпочтениям клиента, указывает, является ли это файл соглашения по умолчанию. Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как по умолчанию. Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|isMajorVersion|Boolean|Указывает, является ли файл соглашения основным обновлением версии. Обновления основных версий недействительны для принятия соглашения на соответствующем языке. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|
|language|String|Язык файла соглашения в формате "languagecode2-country/regioncode2". "languagecode2" — это код из двух букв нижнего уровня, полученный из ISO 639-1, в то время как "country/regioncode2" является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47. Например, американский английский язык `en-US` . Только для чтения. Наследуется [от agreementFileProperties](../resources/agreementfileproperties.md).|

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
