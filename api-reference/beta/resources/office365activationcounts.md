---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac3b6bb14b347f4ab273bbf65ce767f1ae6e1a2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983205"
---
# <a name="office365activationcounts-resource-type"></a>Тип ресурса office365ActivationCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата содержимого.          |
| productType       | String | Тип продукта, например "Microsoft 365 профессиональныйplus" или "Project Client". |
| windows           | Int64  | Количество активаций в Windows. Это число включает каждую активацию на любом компьютере с Windows. |
| mac               | Int64  | Количество активаций для Mac OS.          |
| android           | Int64  | Количество активаций на устройстве с Android.  |
| ios               | Int64  | Количество активаций для iOS.             |
| windows10Mobile   | Int64  | Количество активаций в Windows 10 Mobile. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```


