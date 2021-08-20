---
title: accessReviewInstanceDecisionItemResource type
description: Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. accessReviewInstanceDecisionItemResource представляет ресурс, связанный с элементом решения.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4560882d117bde86da96a0d0d887fc7e2960b13d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264369"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>accessReviewInstanceDecisionItemResource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Каждый элемент решения в обзоре доступа представляет доступ к ресурсу, который определен объектом accessReviewInstanceDecisionItemResource. accessReviewInstanceDecisionItemResource — это открытый тип, который позволяет передавать другие свойства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображение имени ресурса|
|id|String|ИД ресурса|
|type|Строка|Тип ресурса. Типы включают: `Group` , , , , `ServicePrincipal` `DirectoryRole` `AzureRole` `AccessPackageAssignmentPolicy` .|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String"
}
```
