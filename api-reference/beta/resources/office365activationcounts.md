---
title: тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 33a39a394b5b82bfb3ba0b5d33dc91320307bb73
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115151"
---
# <a name="office365activationcounts-resource-type"></a>тип ресурса office365ActivationCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата контента.          |
| productType       | String | Тип продукта, например "Microsoft 365 ProPlus" или "Project клиент". |
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


