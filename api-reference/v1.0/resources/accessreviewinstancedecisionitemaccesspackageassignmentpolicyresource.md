---
title: accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource type
description: Представляет политику назначения пакета доступа, для которой доступ представлен с помощью объекта accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3dfb5c9a42e9b807b802ff1e1ef24b2533388db4
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162153"
---
# <a name="accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource-resource-type"></a>accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource type

Пространство имен: microsoft.graph

Представляет политику назначения пакета доступа, для которой доступ представлен с помощью [объекта accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) **accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource** — открытый тип, который позволяет передавать другие свойства.

Наследует [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessPackageDisplayName|Строка| Отображение имени пакета доступа, доступ к которому был предоставлен. |
|accessPackageId|Строка| Идентификатор пакета доступа, доступ к которому был предоставлен. |
| displayName | Строка | Отображение имени пакета доступа. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | Строка | Идентификатор ресурса элемента решения. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Строка | Тип ресурса. Тип всегда будет `AccessPackageAssignmentPolicy` .  Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |



## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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


