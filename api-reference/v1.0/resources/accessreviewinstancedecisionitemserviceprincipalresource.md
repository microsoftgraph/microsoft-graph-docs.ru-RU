---
title: accessReviewInstanceDecisionItemServicePrincipalResource type
description: Представляет директоров служб, доступ к ресурсу которых представлен через объект accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e71aacd0ac0876ed7ec9fc0fdc70b8f136831092
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162148"
---
# <a name="accessreviewinstancedecisionitemserviceprincipalresource-resource-type"></a>accessReviewInstanceDecisionItemServicePrincipalResource type

Пространство имен: microsoft.graph

Представляет директоров служб, доступ к ресурсу которых представлен через [объект accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) **accessReviewInstanceDecisionItemServicePrincipalResource** — это открытый тип, который позволяет передавать другие свойства.

Наследует [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| appId | String | Глобальный уникальный идентификатор приложения, к которому был предоставлен доступ. |
| displayName | Строка | Отображение имени ресурса. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md).|
| id | Строка | Идентификатор ресурса элемента решения. Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |
| type | Строка | Тип ресурса. Тип всегда будет `ServicePrincipal` .  Наследуется [от accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionItemresource.md). |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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
