---
title: Тип ресурса Едукатионксвдатапровидер
description: 'Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 33cb0268eeb8c6d6b896dfb8ab02f7bb59b00e98
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434986"
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
