---
title: тип ресурсов stsPolicy
description: Представляет абстрактный базовый тип для типов политик, которые контролируют поведение платформы удостоверений Майкрософт.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 362b0ec08cfc7b3fe96b67baf4e8ed4aa2b86495
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761565"
---
# <a name="stspolicy-resource-type"></a>тип ресурсов stsPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет абстрактный базовый тип для типов политик, которые контролируют [поведение платформы удостоверений](/azure/active-directory/develop/) Майкрософт.

Наследует [от policyBase](policyBase.md).

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения. Унаследованный от [policyBase](policyBase.md).|
|description|String| Описание этой политики. Унаследованный от [policyBase](policyBase.md).|
|displayName|String| Отображение имени для этой политики. Унаследованный от [policyBase](policyBase.md).|
|определение|Коллекция String| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками политики. Синтаксис определения отличается для каждого типа политики. Обязательный.|
|isOrganizationDefault|Boolean|Если заданной для true, активирует эту политику. Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации. Необязательный, значение по умолчанию является ложным.|

## <a name="relationships"></a>Отношения

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