---
title: Тип ресурса accessReviewInstanceDecisionItemUserTarget
description: Представляет цель проверки в качестве пользователя.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 73fba5b7329a6dd13ddc455b9ba327467dde9016
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133471"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItemUserTarget

Пространство имен: microsoft.graph

Представляет удостоверение пользователя, проверяемого в [accessReviewInstance.](accessreviewinstance.md)

Наследуется [от accessReviewInstanceDecisionItemTarget.](../resources/accessreviewinstancedecisionitemtarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
| userDisplayName | String | Имя пользователя. |
| userId | String | Идентификатор пользователя. |
| userPrincipalName | String | Имя участника-пользователя. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemUserTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
