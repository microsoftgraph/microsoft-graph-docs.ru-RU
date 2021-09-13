---
title: тип ресурса conditionalAccessRoot
description: Ресурс conditionalAccessRoot является точкой входа для объектной модели условного доступа (CA). Он не содержит никаких полезных свойств.
ms.localizationpriority: medium
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 739b02a5bf06c7ac742b524e406145c29bb40aa3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59110542"
---
# <a name="conditionalaccessroot-resource-type"></a>тип ресурса conditionalAccessRoot

Пространство имен: microsoft.graph

Ресурс **conditionalAccessRoot** является точкой входа для объектной модели условного доступа (CA). Он не содержит никаких полезных свойств.

Дополнительные сведения о условном доступе в Azure Active Directory см. в дополнительных сведениях [о условном доступе?](/azure/active-directory/conditional-access/overview)

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|namedLocations|[коллекция namedLocation](namedlocation.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных именных местоположений.|
|политики|Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных политик условного доступа (CA).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessRoot"
}-->

```json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot"
}
```