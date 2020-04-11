---
title: Тип ресурса Стсполици
description: Представляет абстрактный базовый тип для типов политики, которые управляют поведением платформы Microsoft Identity.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ae84fae2df06ddb2911f6462d644f522510ed89c
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229586"
---
# <a name="policybase-resource-type"></a>Тип ресурса основы

Пространство имен: microsoft.graph

Представляет абстрактный базовый тип для типов политики, которые управляют поведением [платформы Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/) .

Наследуется от [основы](policyBase.md).

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения. Наследуется от [основы](policyBase.md).|
|description|String| Описание для этой политики. Наследуется от [основы](policyBase.md).|
|displayName|Строка| Отображаемое имя для этой политики. Наследуется от [основы](policyBase.md).|
|RDLC|Коллекция String| Коллекция String, содержащая строку JSON, определяющую правила и параметры политики. Синтаксис определения отличается для каждого производного типа политики. Обязательно.|
|исорганизатиондефаулт|Логический|Если задано значение true, активируется эта политика. Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию. Необязательное значение по умолчанию — false.|

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