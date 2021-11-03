---
title: тип ресурса safeguardProfile
description: Описывает проблему(ы), от которой служба защищает устройства.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d6df910ceff9e726c9a6aae3b847aa0478a7b107
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697396"
---
# <a name="safeguardprofile-resource-type"></a>тип ресурса safeguardProfile

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает проблему(ы), от которой служба защищает устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|category|microsoft.graph.windowsUpdates.safeguardCategory|Указывает категорию гарантий. Возможные значения: `likelyIssues` .|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.safeguardProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.safeguardProfile",
  "category": "String"
}
```

