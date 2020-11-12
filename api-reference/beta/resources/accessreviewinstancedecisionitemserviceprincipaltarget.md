---
title: Тип ресурса АкцессревиевинстанцедеЦисионитемсервицепринЦипалтаржет
description: Представляет целевой объект проверки в качестве целевого объекта участника службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e9943a287dd28a44f3b36eae1a92d1b2c385496c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001066"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>Тип ресурса АкцессревиевинстанцедеЦисионитемсервицепринЦипалтаржет

Пространство имен: microsoft.graph

Представляет участника службы в разделе "Обзор" в [акцессревиевинстанце](accessreviewinstance.md).

Наследуется от [акцессревиевинстанцедеЦисионитемтаржет](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :--------------------------- | :------------------------ | :---------- |
| сервицепринЦипалид | Строка | Идентификатор субъекта-службы, доступ к которому просматривается. |
| сервицепринЦипалдисплайнаме | Строка | Отображаемое имя субъекта-службы, доступ к которому просматривается. |
| appId | String | AppId для анализируемого объекта участника службы. |

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
