---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d396ee84e4af6606cfde3e5fc17ef02c0a9594f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966582"
---
# <a name="office365activationcounts-resource-type"></a>Тип ресурса office365ActivationCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| Репортрефрешдате | Дата   | Самая поздняя дата контента.          |
| Продукттипе       | String | Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365". |
| под           | Int64  | Счетчик активаций в Windows. Это число включает все активации на любом компьютере с Windows. |
| mac               | Int64  | Число активаций в Mac OS.          |
| ОС           | Int64  | Счетчик активаций на устройстве с Android.  |
| модуле               | Int64  | Счетчик активаций на iOS.             |
| windows10Mobile   | Int64  | Счетчик активаций для Windows 10 Mobile. |

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
