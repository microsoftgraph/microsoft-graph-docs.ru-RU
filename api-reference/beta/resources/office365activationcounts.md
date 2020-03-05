---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 1a45aa058a5186e87d11eed5199b51abf709879b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522493"
---
# <a name="office365activationcounts-resource-type"></a>Тип ресурса office365ActivationCounts

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| репортрефрешдате | Дата   | Самая поздняя дата контента.          |
| продукттипе       | String | Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365". |
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
