---
title: accessReviewInstanceDecisionItemResource type
description: Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. accessReviewInstanceDecisionItemResource представляет ресурс, связанный с элементом решения.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 879a0b1f74fa08e0ae66e5aaf5ab45b9d96de397
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469791"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>accessReviewInstanceDecisionItemResource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. accessReviewInstanceDecisionItemResource представляет ресурс, связанный с элементом решения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображение имени ресурса|
|id|String|ИД ресурса|
|type|String|Тип ресурса. Типы включают: Group, ServicePrincipal, DirectoryRole, AzureRole, AccessPackageAssignmentPolicy.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
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
