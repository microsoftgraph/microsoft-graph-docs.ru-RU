---
title: тип ресурсов stsPolicy
description: Представляет абстрактный базовый тип для типов политик, которые контролируют платформа удостоверений Майкрософт поведение.
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04ab6b06bbe099759802a57b6bbfdc337a233ef6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59122966"
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
|displayName|Строка| Отображение имени для этой политики. Унаследованный от [policyBase](policyBase.md).|
|определение|Коллекция String| Коллекция строк, содержащая строку JSON, определяемую правилами и настройками политики. Синтаксис определения отличается для каждого типа политики. Обязательное.|
|isOrganizationDefault|Логический|Если заданной для true, активирует эту политику. Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации. Необязательный, значение по умолчанию является ложным.|

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
