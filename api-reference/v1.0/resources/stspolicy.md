---
title: Тип ресурса Стсполици
description: Представляет абстрактный базовый тип для типов политики, которые управляют поведением платформы Microsoft Identity.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb43f538fe961af85c1a92f5e853ae8bca44b418
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581906"
---
# <a name="stspolicy-resource-type"></a>Тип ресурса Стсполици

Пространство имен: microsoft.graph

Представляет абстрактный базовый тип для типов политики, которые управляют поведением [платформы Microsoft Identity](/azure/active-directory/develop/) .

Наследуется от [основы](policyBase.md).

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения. Наследуется от [основы](policyBase.md).|
|description|String| Описание для этой политики. Наследуется от [основы](policyBase.md).|
|displayName|String| Отображаемое имя для этой политики. Наследуется от [основы](policyBase.md).|
|RDLC|Коллекция String| Коллекция String, содержащая строку JSON, определяющую правила и параметры политики. Синтаксис определения отличается для каждого производного типа политики. Обязательно.|
|исорганизатиондефаулт|Boolean|Если задано значение true, активируется эта политика. Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию. Необязательное значение по умолчанию — false.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stsPolicy",
  "baseType": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": ["String"],
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->