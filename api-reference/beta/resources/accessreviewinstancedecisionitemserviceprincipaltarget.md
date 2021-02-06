---
title: Тип ресурса accessReviewInstanceDecisionItemServicePrincipalTarget
description: Представляет целевой объект проверки в качестве основного целевого объекта службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ef944fdd1b8dbe989b1ad92e3d49b1b057fdef74
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133499"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>Тип ресурса accessReviewInstanceDecisionItemServicePrincipalTarget

Пространство имен: microsoft.graph

Представляет проверяемую службу в [accessReviewInstance.](accessreviewinstance.md)

Наследуется [от accessReviewInstanceDecisionItemTarget.](../resources/accessreviewinstancedecisionitemtarget.md)

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | Строка | Идентификатор основного службы, доступ которого просматривается. |
| servicePrincipalDisplayName | Строка | Отображаемого имени основного службы, доступ которого просматривается. |
| appId | String | AppId для проверяемого объекта субъекта-службы. |

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
