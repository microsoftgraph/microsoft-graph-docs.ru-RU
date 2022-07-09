---
title: Тип ресурса accessReviewInstanceDecisionItemServicePrincipalTarget
description: Представляет целевой объект проверки в качестве целевого объекта субъекта-службы.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dafb1cde55fe510edcff89bd5497997d136a12a9
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698144"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItemServicePrincipalTarget

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет проверяемый субъект-службу в [accessReviewInstance](accessreviewinstance.md).

Наследуется [от accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | Строка | Идентификатор субъекта-службы, доступ к которому проверяется. |
| servicePrincipalDisplayName | String | Отображаемое имя субъекта-службы, доступ к которому просматривается. |
| appId | String | AppId для проверяемой сущности субъекта-службы. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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
