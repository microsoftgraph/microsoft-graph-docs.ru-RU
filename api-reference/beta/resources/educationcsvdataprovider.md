---
title: Тип ресурса Едукатионксвдатапровидер
description: 'Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60377b1761bcb5c672ae42f3067bb20d41325e9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095536"
---
# <a name="educationcsvdataprovider-resource-type"></a>Тип ресурса Едукатионксвдатапровидер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.

Производный от [едукатионсинчронизатиондатапровидер].

## <a name="properties"></a>Свойства

| Свойство       | Тип                                     | Описание                                                           |
| :------------- | :--------------------------------------- | :-------------------------------------------------------------------- |
| настроек | [едукатионсинчронизатионкустомизатионс] | Необязательные настройки, которые необходимо применить к профилю синхронизации. |

[едукатионсинчронизатиондатапровидер]: educationsynchronizationdataprovider.md
[едукатионсинчронизатионкустомизатионс]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationCsvDataProvider",
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```


