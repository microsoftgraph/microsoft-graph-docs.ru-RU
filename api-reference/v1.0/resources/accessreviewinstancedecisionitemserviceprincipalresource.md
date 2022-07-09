---
title: Тип ресурса accessReviewInstanceDecisionItemServicePrincipalResource
description: Представляет субъекты-службы, доступ к ресурсу которых представлен через объект accessReviewInstanceDecisionItem.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: db28cbe196583af2d7876d56c6b5542a169af90d
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698473"
---
# <a name="accessreviewinstancedecisionitemserviceprincipalresource-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItemServicePrincipalResource

Пространство имен: microsoft.graph

Представляет субъекты-службы, доступ к ресурсу которых представлен через [объект accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . **accessReviewInstanceDecisionItemServicePrincipalResource** — это открытый тип, который позволяет передавать другие свойства.

Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| appId | String | Глобальный уникальный идентификатор приложения, к которому предоставлен доступ. |
| displayName | Строка | Отображаемое имя ресурса. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | String | Идентификатор ресурса элемента принятия решения. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Строка | Тип ресурса. Тип всегда будет иметь значение `ServicePrincipal`.  Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessreviewinstancedecisionitemserviceprincipalresource",
  "baseType": "microsoft.graph.accessReviewInstanceDecisionItemResource",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessreviewinstancedecisionitemserviceprincipalresource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "appId": "String"
}
```
