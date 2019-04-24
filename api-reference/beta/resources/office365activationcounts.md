---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7bc21be693a5c68ecd5c6a1e4e44d53c9261acdb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505468"
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
