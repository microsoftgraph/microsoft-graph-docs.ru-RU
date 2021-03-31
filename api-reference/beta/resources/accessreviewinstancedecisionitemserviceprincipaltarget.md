---
title: accessReviewInstanceDecisionItemServicePrincipalTarget type
description: Представляет цель проверки в качестве основной целевой задачи службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d8032282d7ddaf41779b73f707b0749e3c82dd0
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469229"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>accessReviewInstanceDecisionItemServicePrincipalTarget type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет главу службы, на рассмотрении в [accessReviewInstance](accessreviewinstance.md).

Наследует [от accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | String | Идентификатор директора службы, доступ к которой пересматривается. |
| servicePrincipalDisplayName | String | Отображает имя директора службы, доступ к которой пересматривается. |
| appId | String | AppId для проверяемого основного объекта службы. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget",
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String"
}
```
