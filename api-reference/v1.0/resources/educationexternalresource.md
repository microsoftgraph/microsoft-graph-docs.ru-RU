---
title: Тип ресурса educationExternalResource
description: Подкласс educationResource. Это служба назначений типов ресурсов по умолчанию, используемая для сопоставления всех ресурсов, которые не доступны для графа. Это позволяет всем вызывающим абонентам пакета SDK работать без проблем.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a692ff228b8df5543b94acb340d215b57912762a
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684874"
---
# <a name="educationexternalresource-resource-type"></a>Тип ресурса educationExternalResource

Пространство имен: microsoft.graph

Представляет универсальный тип для сопоставления ресурсов, которые не предоставляются в Microsoft Graph.

Наследуется от [educationResource](educationresource.md).

Этот сложный тип позволяет всем вызывающим абонентам пакета SDK работать без проблем.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|webUrl|String|Расположение ресурса. Обязательный|
|createdBy|String|Отображаемое имя пользователя, создавшего этот объект.|
|createdDateTime|DateTimeOffset|Дата, когда была добавлена повторная ошибка.|
|displayName|string|Отображаемое имя ресурса.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменяет ресурс.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения ресурса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationExternalResource"
}-->

```json
{
  "webUrl": "String",
  "createdBy": "String (User)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": "String (User)",
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-09-21 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExternalResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
