---
title: тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 39e679da134120377f17dab520c332dc54aab328ef924b65212f5145279a8402
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176325"
---
# <a name="office365activationcounts-resource-type"></a>тип ресурса office365ActivationCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата контента.          |
| productType       | Строка | Тип продукта, например "Microsoft 365 ProPlus" или "Project клиент". |
| Windows           | Int64  | Активация рассчитывается на Windows. Этот номер включает каждую активацию на любом Windows компьютере. |
| mac               | Int64  | Активация рассчитывается на ОС Mac.          |
| Android           | Int64  | Активация рассчитывается на устройстве Android.  |
| ios               | Int64  | Активация рассчитывается на iOS.             |
| windows10Mobile   | Int64  | Активация рассчитывается на Windows 10 мобильном телефоне. |

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


