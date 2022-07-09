---
title: Тип ресурса accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource
description: Представляет политику назначения пакетов доступа, для которой доступ представлен через объект accessReviewInstanceDecisionItem.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 40cbb74fd9a9801b62f4a98809d28c56dbc86b2e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698305"
---
# <a name="accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource

Пространство имен: microsoft.graph

Представляет политику назначения пакетов доступа, для которой доступ представлен через объект [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . **accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource** — это открытый тип, который позволяет передавать другие свойства.

Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessPackageDisplayName|Строка| Отображаемое имя пакета доступа, к которому предоставлен доступ. |
|accessPackageId|Строка| Идентификатор пакета доступа, к которому предоставлен доступ. |
| displayName | Строка | Отображаемое имя пакета доступа. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | Строка | Идентификатор ресурса элемента принятия решения. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Строка | Тип ресурса. Тип всегда будет иметь значение `AccessPackageAssignmentPolicy`.  Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |



## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "accessPackageId": "String",
  "accessPackageDisplayName": "String"
}
```


