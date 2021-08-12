---
title: тип ресурсов stsPolicy
description: Представляет абстрактный базовый тип для типов политик, которые контролируют платформа удостоверений Майкрософт поведение.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8c36121274a3e1d1b6f574a7256b869fe94c7ea5d0fd9db8067ddd78a7d0bdb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184482"
---
# <a name="stspolicy-resource-type"></a>тип ресурсов stsPolicy

Пространство имен: microsoft.graph

Представляет абстрактный базовый тип для типов политик, [которые контролируют платформа удостоверений Майкрософт](/azure/active-directory/develop/) поведение.

Наследует [от policyBase](policyBase.md).

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения. Унаследованный от [policyBase](policyBase.md).|
|description|String| Описание этой политики. Унаследованный от [policyBase](policyBase.md).|
|displayName|String| Отображение имени для этой политики. Унаследованный от [policyBase](policyBase.md).|
|определение|Коллекция String| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками политики. Синтаксис определения отличается для каждого типа политики. Обязательный элемент.|
|isOrganizationDefault|Логический|Если заданной для true, активирует эту политику. Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации. Необязательный, значение по умолчанию является ложным.|

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