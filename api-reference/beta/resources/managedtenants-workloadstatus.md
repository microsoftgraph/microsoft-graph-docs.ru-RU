---
title: тип ресурса workloadStatus
description: Представляет состояние рабочей нагрузки.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d85d7fd60a269c360185d8d4ffb5952a71bdd628
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792269"
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
