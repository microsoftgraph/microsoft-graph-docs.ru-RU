---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4787672df6462e8d1f343e4dace43ede7c79ff37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991183"
---
# <a name="office365activationcounts-resource-type"></a>Тип ресурса office365ActivationCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | Последняя дата контента.          |
| productType       | String | Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365". |
| Windows           | Int64  | Число активации в Windows. Эта цифра включает в себя каждые активации на компьютерах под управлением Windows. |
| mac               | Int64  | Число активации на Mac OS.          |
| Android (en)           | Int64  | Число активации на устройстве Android.  |
| операций ввода-вывода               | Int64  | Число активации на операций ввода-вывода.             |
| windows10Mobile   | Int64  | Активация на количество Windows 10 mobile. |

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
