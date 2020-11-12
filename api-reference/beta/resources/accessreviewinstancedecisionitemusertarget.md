---
title: Тип ресурса АкцессревиевинстанцедеЦисионитемусертаржет
description: Представляет целевой объект проверки от имени пользователя.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aa2117895599ba1d2c4b9829b7cad22b581f2055
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001063"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>Тип ресурса АкцессревиевинстанцедеЦисионитемусертаржет

Пространство имен: microsoft.graph

Представляет удостоверение пользователя в ходе рецензирования в [акцессревиевинстанце](accessreviewinstance.md).

Наследуется от [акцессревиевинстанцедеЦисионитемтаржет](../resources/accessreviewinstancedecisionitemtarget.md).

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
