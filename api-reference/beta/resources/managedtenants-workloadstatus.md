---
title: тип ресурса workloadStatus
description: Представляет состояние рабочей нагрузки.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 50cbd9cdc59426f413333835c4418112401d8038
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403132"
---
# <a name="workloadstatus-resource-type"></a>тип ресурса workloadStatus

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние рабочей нагрузки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя отображения рабочей нагрузки. Обязательный. Только для чтения.|
|offboardedDateTime|DateTimeOffset|Дата и время отключения рабочей нагрузки. Необязательно. Только для чтения.|
|onboardedDateTime|DateTimeOffset|Дата и время загрузки. Необязательно. Только для чтения.|
|onboardingStatus|workloadOnboardingStatus|Состояние onboarding для рабочей нагрузки. Возможные значения: `notOnboarded`, `onboarded`, `unknownFutureValue`. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadStatus",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "displayName": "String",
  "offboardedDateTime": "String (timestamp)"
}
```
